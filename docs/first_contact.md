# First Contact

This note is for a skeptical researcher, recruiter, funder, or collaborator who wants the shortest honest read on the BoggersTheFish TS work.

## Core Hypothesis

The core hypothesis is that reasoning systems become easier to inspect and repair when their internal work is represented as graph state plus explicit constraint pressure.

In TS terms:

- claims, evidence, operations, and dependencies are graph nodes and edges,
- uncertainty, contradiction, malformed structure, and task failure show up as tension,
- repair and abstraction are operations over the graph,
- verifier-backed traces make the system's transitions inspectable.

The bet is not that this alone solves reasoning. The bet is that this gives better control surfaces for reasoning systems than opaque answer-only evaluation.

## What Has Been Built

- [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0): a deterministic Python toy reasoner that emits candidate chains, CIG checks, tension issues, repair suggestions, operation loops, and JSON traces.
- [TS-Codex-OS](https://github.com/BoggersTheFish/TS-Codex-OS): a local-first project graph, tension ledger, planner, and release receipt substrate for Codex-driven development.
- [TS-Core](https://github.com/BoggersTheFish/TS-Core): a graph dynamics kernel for propagation, relaxation, stability, and tension experiments.
- [bozo / TensionLM](https://github.com/BoggersTheFish/bozo): language-model mechanism experiments around sigmoid pairwise tension attention.
- [BoggersTheCIG](https://github.com/BoggersTheFish/BoggersTheCIG) and [cig-ts-engine](https://github.com/BoggersTheFish/cig-ts-engine): provenance-aware claim/evidence graph work.
- [TS-Start-Here](https://github.com/BoggersTheFish/TS-Start-Here): this public map.

## What Is Independently Runnable

The strongest first runnable artifact is TS-Reasoner-v0.

It includes:

- a standard-library Python pipeline,
- unit tests,
- CLI/demo scripts,
- release notes,
- trace artifacts,
- v0.8 externalized small benchmark harness.

The current v0.8 receipt reports:

- `26` unit tests passing,
- `10` curated externalized benchmark tasks,
- `direct`: `4/10` correct,
- `random_selector`: `5/10` correct,
- `ranker_only`: `8/10` correct,
- `full_control_loop`: `8/10` correct, `10/10` settled, mean final tension `0.0`.

That is not a broad benchmark claim. It is a small reproducible receipt.

## What Is Toy-Scope

The current reasoning systems are narrow.

- TS-Reasoner uses toy claim extraction and heuristic verification.
- The v0.8 benchmark is curated and normalized into relation templates.
- The proof-chain evaluation is small.
- The current model artifacts are experimental mechanism work, not production-grade language models.
- TS-Codex-OS is local file-based project control, not a replacement for Codex or an autonomous engineering system.

## What Would Falsify Or Weaken The Approach

The approach would be weakened if:

- tension telemetry repeatedly fails to predict useful repair operations,
- verifier-backed traces become too expensive or noisy to inspect,
- low-tension states routinely hide wrong answers or unsupported abstentions,
- learned tension fields do not outperform simpler baselines on external tasks,
- graph/provenance structure adds complexity without improving debugging, repair, or evaluation,
- stronger benchmarks show no benefit over conventional verifier/ranker baselines.

These are useful failure modes. TS should make them easier to see, not hide them.

## Next Benchmark

The next benchmark target is TS-Reasoner v0.9:

```text
Transitive proof-chain support
```

v0.8 exposed the exact failure: settlement is not the same as proof completion. The full control loop can settle into a low-tension abstention on small proof-chain tasks.

v0.9 should test whether explicit transitive bridge construction can convert those failures into completed proof paths:

```text
small_proof_chain failure
  -> detect unresolved transitive edge
  -> propose bridge candidate
  -> verify bridge against premises
  -> rerun control loop
  -> score whether abstention converts into valid proof
```

The required telemetry distinction is:

```text
settled_abstention
settled_answer
settled_proof_complete
settled_invalid
```

That distinction keeps the system from treating "I do not know" as a perfect relaxation when the task requires a proof.
