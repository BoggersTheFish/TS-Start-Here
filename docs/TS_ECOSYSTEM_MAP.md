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

## Public Golden Path

```text
TS-Start-Here
-> TS-Reasoner-v0: reasoning trace contract
-> TS-Codex-OS: project-control substrate
-> TS-Benchmarks: falsification and scaling harness
-> TensionLM: model substrate experiment
```

## 1. TS-Reasoner

Repo:

- https://github.com/BoggersTheFish/TS-Reasoner-v0

Current releases:

- v0.1.0 deterministic trace contract: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v0.1.0
- v0.2.0 learned tension-ranker: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v0.2.0
- v0.3.0 learned candidate proposal: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v0.3.0

Current active release:

- v1.6.0 TensionLM export set receipt: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v1.6.0

What it is:

TS-Reasoner is a small Python reasoning telemetry repo. It now exposes TS-Core-backed typed tension channels, learned channel calibration, candidate containment, exported TensionLM-style ingestion, messy candidate stress, real exported TensionLM-side sample receipts, export set failure preservation, and JSON release receipts.

What it proves:

- Reasoning failures can be separated into typed operational channels.
- The public output schema can stay stable while internal components evolve.
- Learned calibration can target channel activation and resolver priority without replacing deterministic channel semantics.
- Release claims can stay sober: typed substrate first, exported candidate data second, model confidence never proof.

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
TS-Reasoner v1.0.0 -> TS-Core-backed typed channels, learned calibration, stress, structural repair, and unified receipt
TS-Reasoner v1.1.0 -> candidate bridge with adversarial containment
TS-Reasoner v1.2.0 -> exported TensionLM-style adapter
TS-Reasoner v1.3.0 -> messy language candidate stress
TS-Reasoner v1.4.0 -> exported-output smoke boundary
TS-Reasoner v1.5.0 -> real exported TensionLM-side sample crosses into TS-Reasoner as candidate data
TS-Reasoner v1.6.0 -> exported TensionLM-side sample set with preserved failure reasons
```

Important caveat:

TS-Reasoner is not a full LLM, theorem prover, or benchmark-grade reasoning system. The current tasks and metrics are toy-scope receipts. They show the interface and release discipline, not robust general reasoning.

Current v1.6.0 claim:

> TS-Reasoner can evaluate multiple exported TensionLM-side candidate samples through a typed verification boundary where malformed, unsupported, contradictory, reverse, and deeper-chain current-limit cases are preserved as failure reasons instead of hidden.

v1.6.0 release receipts report:

- `67` unit tests passing in the local final pass before release.
- `export_set_read_success_rate`: `1.0`.
- `candidate_parse_success_rate`: `0.8889`.
- `candidate_parse_expectation_rate`: `1.0`.
- `provenance_preservation_rate`: `1.0`.
- `accepted_outputs_typed_support_rate`: `1.0`.
- `bad_candidate_rejection_rate`: `1.0`.
- `verifier_beats_confidence_rate`: `1.0`.
- `candidate_graph_contamination_count`: `0`.
- `trace_schema_validity`: `1.0`.

v1.0.0 release receipts established the typed-channel base:

- `45` unit tests passing at release time.
- Scoped calibrator eval: `1.0` answer accuracy, channel activation accuracy, resolver accuracy, abstention correctness, and trace schema validity.
- Generalization stress: Outcome B, exposing depth, distractor, quantifier, and contradiction-placement failures.
- Structural repair: depth and distractor robustness move from `0.0` to `1.0`; quantifier trap failures and contradiction misses move from `1` to `0`.
- Trace schema validity remains `1.0`.

Current technical step:

```text
TS-Reasoner v1.6.0 = TensionLM export set under typed verification
```

The v1.6.0 claim stays narrow: small exported sample set, parser-controlled verifier, not live model integration into TS-Reasoner. The `0.8889` parse success is intentional because a malformed export is preserved and rejected; `candidate_parse_expectation_rate` remains `1.0`.

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

- TS-Reasoner has public releases with stable JSON traces and machine-readable receipts.
- TS-Reasoner v1.6.0 has a receipt-backed cross-repo boundary where a small exported TensionLM-side candidate set enters TS-Reasoner without becoming proof.
- TS-Codex-OS has a public release that can ingest repos, score tensions, propose actions, suggest verification, write receipts, and produce project graph artifacts.
- TS-Codex-OS has already been used to guide a TS-Reasoner release.

What remains scoped:

- Current TS-Reasoner tasks are toy tasks.
- Current learned components are channel calibrators and smoke-test experiments.
- Current TS-Codex-OS ingestion is local and file-based.
- Current claims are release-engineering claims, not general reasoning claims.

Current best public sentence:

> TS is becoming a versioned research stack: typed tension traces, learned channel calibration, exported model-side candidate data, project-control receipts, and typed verification boundaries.

What should happen next:

1. Keep TS-Reasoner v1.6.0 stable unless there is a bug.
2. Build TS-Reasoner v1.7.0 as a deeper-chain support repair.
3. Keep TensionLM in the proposer role and TS-Reasoner in the verifier role.
4. Use the v1.6 deeper-chain current-limit case as the repair target.

## 5. TS-Benchmarks

Repo:

- https://github.com/BoggersTheFish/TS-Benchmarks
- `/home/boggersthefish/BoggersSpace/TS-Benchmarks`

What it is:

TS-Benchmarks is the new audit-first benchmark harness for scaling, reasoning, hardware, and hybrid Graph+LLM evidence.

Current implemented slice:

- deterministic synthetic graph scaling harness
- TS-Core-style sparse active-frontier relaxation reference
- degree, PageRank-like, and random residual contradiction localization baselines
- benchmark receipt schema
- JSON result receipts, schema validation, plots, and markdown/CSV report generation

Important caveat:

The first scaling harness is not a capability claim. The initial local sweep already exposed a failure mode: scale-free graphs retained high final tension and zero contradiction-localization F1 under the first reference config. That should be treated as a high-tension engineering node, not hidden.

Public framing:

> v0.1 does not claim TS-Core scales cleanly. It shows where reference TS relaxation succeeds, where it fails, and which diagnostics will drive the next implementation.

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
TS-Reasoner v1.0.0 -> typed reasoning substrate with channel calibration, stress, repair, and release receipt
TS-Reasoner v1.1.0 -> candidate bridge with adversarial containment
TS-Reasoner v1.2.0 -> exported TensionLM-style adapter
TS-Reasoner v1.3.0 -> messy language candidate stress
TS-Reasoner v1.4.0 -> exported-output smoke boundary
TS-Reasoner v1.5.0 -> real exported TensionLM-side sample under typed verification
TS-Reasoner v1.6.0 -> TensionLM export set under typed verification with preserved failures
```

Every release should answer:

- What changed?
- What artifact proves it?
- What verification ran?
- What tension remains?
- What claim is explicitly not being made?
