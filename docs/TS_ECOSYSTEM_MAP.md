# TS Ecosystem Map

Author: BoggersTheFish

Main site:

- https://www.boggersthefish.com/
- https://www.boggersthefish.com/projects
- https://www.boggersthefish.com/ts-os
- https://www.boggersthefish.com/waves

This map explains the current public Thinking System / TS artifacts in plain engineering terms. It is intentionally conservative: the public systems are real, versioned, and runnable, but the current releases are still small research artifacts and toy-scope evaluation scaffolds.

## Core Framing

Thinking System / TS treats software, reasoning, memory, releases, and claims as graph-like constraint structures.

Basic primitives:

- Node: stable holder of state.
- Edge: relation or constraint.
- Activation: current signal.
- Tension: unresolved constraint pressure.
- Stability: ability to hold under tension.
- Coherence: graph state that holds constraints without lying or collapsing.
- Attractor: state or pattern the graph tends toward.

Engineering loop:

```text
Propagate -> Relax -> Break -> Evolve
```

In the current public repos, this means:

- Propagate: inspect current files, tests, docs, artifacts, releases, claims, and traces.
- Relax: make the smallest useful change that reduces unresolved tension.
- Break: split confused claims, modules, branches, or release scopes when one node carries incompatible demands.
- Evolve: update the structure so future work is more stable and inspectable.

## 1. TS-Reasoner

Repo:

- https://github.com/BoggersTheFish/TS-Reasoner-v0

Current releases:

- v0.1.0 deterministic trace contract: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v0.1.0
- v0.2.0 learned tension-ranker: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v0.2.0
- v0.3.0 learned candidate proposal: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v0.3.0

Current active release:

- v0.9.0 proof-chain support: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v0.9.0

What it is:

TS-Reasoner is a small Python standard-library reasoning telemetry repo. It represents reasoning as candidate chains, checks those chains with a toy Claim-Interaction Graph, scores local/global tension, suggests repairs, selects a low-tension answer, and exports JSON traces.

What it proves:

- Reasoning chains can be made inspectable as graph-like artifacts.
- The public output schema can stay stable while internal components evolve.
- Learned components can be plugged into the trace contract without hiding the verification path.
- Release claims can stay sober: deterministic trace contract first, learned ranker second, learned candidate proposal third.

Current ladder:

```text
TS-Reasoner v0.1.0 -> deterministic inspectable trace contract
TS-Reasoner v0.2.0 -> learned tension-ranker experiment inside the same contract
TS-Reasoner v0.3.0 -> learned candidate proposal, still verified by CIG/tension/repair
TS-Reasoner v0.4.0 -> coordinated tension-state operation engine
TS-Reasoner v0.5.0 -> residual-trained coupling matrix
TS-Reasoner v0.6.0 -> bounded multi-step tension-control loop
TS-Reasoner v0.7.0 -> residual closure with redundant-claim compression
TS-Reasoner v0.8.0 -> externalized small benchmark harness and baseline comparison
TS-Reasoner v0.9.0 -> transitive proof-chain support for positive universal all/all chains
```

Important caveat:

TS-Reasoner is not a full LLM, theorem prover, or benchmark-grade reasoning system. The current tasks and metrics are toy-scope receipts. They show the interface and release discipline, not robust general reasoning.

Current v0.9 claim:

> TS-Reasoner v0.9 closes the proof-chain gap exposed by v0.8 on the existing normalized small benchmark surface, while keeping answer scores, tension telemetry, release receipts, and failure modes inspectable.

v0.9 release receipts report:

- `27` unit tests passing.
- `10` curated externalized benchmark tasks.
- `direct`: `4/10` correct, mean global tension `0.2333`.
- `random_selector`: `6/10` correct, mean global tension `0.1867`.
- `ranker_only`: `10/10` correct, mean global tension `0.0767`.
- `full_control_loop`: `10/10` correct, `10/10` settled, mean global tension `0.0`.
- `small_proof_chain/full_control_loop`: `2/2` correct.

Current technical step:

```text
TS-Reasoner v0.9.0 = narrow transitive proof-chain support
```

The v0.9 claim stays narrow: positive universal all/all chains only, still toy-scope and normalized.

## 2. TS-Codex-OS

Repo:

- https://github.com/BoggersTheFish/TS-Codex-OS

Current release:

- v0.1.0 local TS project substrate: https://github.com/BoggersTheFish/TS-Codex-OS/releases/tag/v0.1.0

What it is:

TS-Codex-OS is a local-first project graph, tension ledger, planner, memory, verifier, and receipt system for Codex-driven development.

Codex remains the coding executor. TS-Codex-OS is the local project-control substrate around Codex.

```text
Codex = hands
TS-Codex-OS = project graph, memory, tension tracker, verifier, receipt layer
```

What it proves:

- Codex/project work can be managed through a graph of project nodes and edges.
- Missing docs, missing release receipts, stale artifacts, overbroad claims, and missing verification can be treated as explicit tensions.
- A repo can ingest itself, detect release-control tensions, apply small relaxations, and re-ingest to confirm stability.
- Release receipts can make public claims auditable.

Observed use:

TS-Codex-OS v0.1.0 inspected TS-Reasoner-v0 before the TS-Reasoner v0.3.0 release. It detected release-control tensions around missing verification receipts and stale artifacts. TS-Reasoner v0.3.0 closed those tensions with regenerated artifacts and release receipts.

Important caveat:

TS-Codex-OS does not replace Codex. It does not run an autonomous agent loop, call LLM APIs, train models, or provide a database. It is a local file-based project substrate.

## 3. TensionLM / Proof-Ranker Ladder

Relevant Hugging Face artifacts:

- https://huggingface.co/BoggersTheFish/ts-proof-ranker-v0
- https://huggingface.co/BoggersTheFish/ts-proof-ranker-v1
- https://huggingface.co/BoggersTheFish/ts-proof-ranker-v2
- https://huggingface.co/BoggersTheFish/ts-proof-ranker-v3
- https://huggingface.co/BoggersTheFish/ts-proof-ranker-v4
- https://huggingface.co/BoggersTheFish/TensionLM-Wave02-22M-H2H
- https://huggingface.co/BoggersTheFish/TensionLM-117M
- https://huggingface.co/BoggersTheFish/TensionLM-117M-Curriculum
- https://huggingface.co/BoggersTheFish/TensionLM-117M-Curriculum-Stage2
- https://huggingface.co/BoggersTheFish/TensionLM-Curriculum-13M
- https://huggingface.co/BoggersTheFish/TensionLM-Phase2-TSNative

What it aims toward:

The TensionLM and proof-ranker ladder aims toward learned tension fields and TS-native reasoning models.

The current public software repos are the control layer around that direction:

- TS-Reasoner defines inspectable reasoning traces and component interfaces.
- TS-Codex-OS defines project-control, release-control, receipts, and memory.
- Proof-ranker and TensionLM artifacts point toward learned scoring, tension fields, and eventually TS-native reasoning behavior.

Important caveat:

The existence of model artifacts does not by itself establish a robust TS-native reasoning model. Stronger benchmark loops, verifier loops, and grounded evaluation are still needed.

## 4. Current Honest Status

What is real now:

- TS-Reasoner has public releases with a stable JSON trace contract.
- TS-Reasoner has learned-ranker and learned-candidate-proposal experiments inside that contract.
- TS-Reasoner v0.9 is published as a narrow proof-chain closure receipt on the existing externalized small benchmark harness.
- TS-Codex-OS has a public release that can ingest repos, score tensions, propose actions, suggest verification, write receipts, and produce project graph artifacts.
- TS-Codex-OS has already been used to guide a TS-Reasoner release.

What remains scoped:

- Current TS-Reasoner tasks are toy tasks.
- Current learned components are smoke-test experiments.
- Current TS-Codex-OS ingestion is local and file-based.
- Current claims are release-engineering claims, not general reasoning claims.

Current best public sentence:

> TS is becoming a versioned research stack: inspectable reasoning traces, learned tension components, project-control receipts, and a path toward stronger verifier-backed reasoning loops.

What should happen next:

1. Keep TS-Reasoner v0.1.0-v0.9.0 stable unless there is a bug.
2. Use TS-Codex-OS to manage future TS-Reasoner release-control tensions.
3. Extend proof-chain tests only after the current v0.9 receipt stays stable.
4. Add broader benchmark/eval loops only after the narrow proof-chain support is audited beyond the tiny fixture.

## Release Discipline

The release pattern should stay boring, sober, and cumulative:

```text
TS-Reasoner v0.1.0 -> trace contract
TS-Reasoner v0.2.0 -> learned ranker
TS-Codex-OS v0.1.0 -> project-control substrate
TS-Reasoner v0.3.0 -> first TS-Codex-guided release
TS-Reasoner v0.4.0 -> coordinated tension-state operation engine
TS-Reasoner v0.5.0 -> residual-trained coupling matrix
TS-Reasoner v0.6.0 -> bounded multi-step control loop
TS-Reasoner v0.7.0 -> residual closure and 4/4 hard-case loop settlement
TS-Reasoner v0.8.0 -> external benchmark harness and proof-chain gap receipt
TS-Reasoner v0.9.0 -> proof-chain gap closure on the tiny normalized fixture
```

Every release should answer:

- What changed?
- What artifact proves it?
- What verification ran?
- What tension remains?
- What claim is explicitly not being made?
