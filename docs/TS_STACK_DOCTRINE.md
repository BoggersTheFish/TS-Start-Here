# TS Stack Doctrine

TS is not one model. TS is a stack.

The central engineering claim is:

> Intelligence can be built as a graph runtime where incoming signals activate multiple typed tension channels, each channel resolves according to its own rule, and stable output emerges from the coherent settlement of those channels.

## Stack Roles

- **TS-Core:** kernel for graph state, activation, typed tension channels, resolver events, relaxation, Break/Evolve hooks, and receipts.
- **TS-Reasoner:** first cognitive app proving typed channels through runnable reasoning traces.
- **Typed tension channels:** operational constraint routes with their own activation, residual, resolver, failure mode, and trace.
- **Learned calibrators:** cheap training layer that calibrates channel activation, weights, thresholds, and resolver priority after deterministic channels work.
- **TensionLM:** language-signal layer that proposes candidate parses, claims, semantic tension fields, and answer candidates.
- **CIG:** persistent claim/evidence/provenance memory graph.
- **TS-Codex-OS:** project-control layer for repo graph state, release tension, verification, and receipts.
- **Website:** public interface for runnable demos, traces, limitations, and receipts.
- **Benchmarks:** truth surface for answer behavior, channel activation, resolver correctness, and failure decomposition.
- **Receipts:** credibility layer tying claims to commands, artifacts, tests, limitations, and unresolved tensions.

## Shared Terms

- **Node:** stable holder of state.
- **Edge:** typed relation or constraint between states.
- **Activation:** current signal pressure through the graph.
- **Tension:** unresolved pressure in a specific channel.
- **Tension channel:** typed operational route with activation, residual, resolver, and trace.
- **Resolver:** channel-specific update operation.
- **Relaxation:** graph update that reduces unresolved tension.
- **Break/Evolve:** adding, splitting, blocking, or restructuring graph state when relaxation fails.
- **Receipt:** machine-readable trace of what happened, what was verified, and what can honestly be claimed.

## Claim Discipline

Safe claim:

> TS decomposes reasoning into typed operational tension channels.

Stronger bounded claim:

> Typed channels can prevent specific failure modes like reverse inference and identity collapse more transparently than a single scalar score.

Experimental claim:

> Learning channel calibration may reduce sample complexity compared with learning all reasoning behavior from raw text.

Future claim:

> TensionLM plus TS-Core may form a cheaper, more inspectable reasoning-language system.

Do not claim that TS beats transformers generally, is AGI, solves the brain, eliminates training, proves consciousness, or replaces grounded benchmarks.

## Biological Process Framing

TS is inspired by a biological process pattern: signals enter a system, specialised states activate, different pressures resolve by different dynamics, and behavior emerges from the settled state.

The substrate changes; the process pattern remains.

```text
brain:
  sensory signal
  specialised neural systems
  prediction/error/reward/homeostasis pressures
  action/perception/belief

TS:
  data signal
  typed tension channels
  logic/identity/provenance/confidence pressures
  answer/update/abstention/split
```
