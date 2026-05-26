# Typed Tension Spec

Typed tension replaces one global score with operational channels. A channel exists when a specific failure mode needs its own activation rule, residual measurement, resolver, and trace.

## Kernel Contract

Every channel must answer:

- What activates me?
- What tension do I measure?
- What operation do I perform?
- What failure mode do I protect against?
- What evidence overrides me?
- What trace do I emit?

Canonical interface:

```python
class TensionChannel:
    name: str
    version: str

    def activate(self, graph, context) -> bool:
        ...

    def measure(self, graph, context) -> ChannelResult:
        ...

    def resolve(self, graph, context) -> ResolverEvent:
        ...

    def serialize(self) -> dict:
        ...
```

## Initial Reasoning Channels

- `logic_transitivity`: infers `A -> C` from `A -> B` and `B -> C`.
- `identity_preservation`: blocks relation paths from collapsing `A` and `C` into equality.
- `directionality`: blocks unsupported reverse edges such as `C -> A`.
- `surface_structure`: tags premise, inferred, candidate, rejected, and blocked states separately.
- `confidence_abstention`: answers only when evidence is strong enough; otherwise abstains or requests evidence.
- `contradiction`: detects incompatible claims and rejects, splits context, or abstains.
- `quantifier_scope`: preserves all/some/no/not-all distinctions and blocks overgeneralisation.
- `context_split`: splits representations when one node carries incompatible regimes.
- `provenance`: weights evidence by source, freshness, dependency, and source cluster.

## Trace Shape

Channel-first traces should include:

```json
{
  "settled": true,
  "global_tension": 0.0,
  "tension_channels": {
    "logic_transitivity": {
      "activated": true,
      "initial_tension": 1.0,
      "resolution": "added_inferred_edge",
      "final_tension": 0.0
    }
  }
}
```

Existing app-level traces may keep compatibility fields, but typed channels should be the inspectable substrate.

## Minimum Impressive Demo

Input:

```text
All A are B.
All B are C.
Question: Are all A C?
```

Expected answer:

```text
Yes, inferred by transitivity.
```

Expected trace:

- `logic_transitivity` activated and inferred `A -> C`.
- `surface_structure` tagged `A -> C` as inferred, not stated.
- `identity_preservation` kept `A` and `C` distinct.
- `directionality` blocked `C -> A`.

Follow-up query:

```text
Are all C A?
```

Expected answer:

```text
Unsupported.
```

Expected trace:

- `directionality` activated.
- Reverse edge was blocked.
