# TS-Start-Here

## Current flagship: TS-Reasoner v3.5.0

TS-Reasoner v3.5.0 is the current verifier-first reasoning flagship.

Release: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v3.5.0

Core line:

    LLMs propose.
    TS verifies.
    Confidence is not proof.
    Typed traces show why.

v3.5.0 adds the public surface, cold-reader demo, external mini-benchmark adapter, verifier-first draft, and TensionLM proposer-boundary smoke.

Boundary: this is not a broad NLP, general theorem-proving, external benchmark victory, live TensionLM runtime, or confidence-as-proof claim.

See: docs/ts_reasoner_v3_5_public_sync.md


**Canonical ecosystem map for the BoggersTheFish TS / Thinking System research stack.**

## Read This First

TS is an engineering framework for modelling information transfer through graph structure, constraint pressure, contradiction handling, provenance, and relaxation.

The current public artifacts are mostly toy-scope or narrow-scope, but they are real, inspectable, runnable, and increasingly receipt-backed. The goal is not to claim a finished general reasoning model. The goal is to make the current systems readable: what exists, what can run, what is still limited, and what would weaken the approach.

Core docs:

- [README First](README_FIRST.md)
- [TS Stack Doctrine](docs/TS_STACK_DOCTRINE.md)
- [Typed Tension Spec](docs/TYPED_TENSION_SPEC.md)
- [TS Receipt Schema](docs/TS_RECEIPT_SCHEMA.md)
- [TS Ecosystem Map](docs/TS_ECOSYSTEM_MAP.md)
- [Credibility Roadmap](docs/CREDIBILITY_ROADMAP.md)
- [First Contact](docs/first_contact.md)
- [Repo Taxonomy](docs/repo_taxonomy.md)
- [Flagship Route](docs/flagship_route.md)
- [20-Minute Technical Tour](docs/technical_tour_20_min.md)
- [Public Signal Reduction Checklist](docs/public_signal_reduction_checklist.md)
- [GitHub Cleanup Plan](docs/github_cleanup_plan.md)
- [Repo Metadata Recommendations](docs/repo_metadata_recommendations.md)

## Fast Route For Researchers

1. Read [README First](README_FIRST.md) for the current public stack and claim discipline.
2. Run [TS-Reasoner-v0 v2.0.0](https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v2.0.0), inspect the learned candidate model receipt, and verify that typed channels remain proof authority.
3. Inspect [TS-Benchmarks](https://github.com/BoggersTheFish/TS-Benchmarks) for falsification-oriented scaling receipts, diagnostics, and failure reports.
4. Inspect [TensionLM](https://github.com/BoggersTheFish/TensionLM) for controlled sigmoid pairwise tension-attention comparisons and the public runner.
5. Inspect [BoggersTheCIG](https://github.com/BoggersTheFish/BoggersTheCIG) or [cig-ts-engine](https://github.com/BoggersTheFish/cig-ts-engine) for provenance-aware claim/evidence graph work.

## Fast Route For Builders

1. Start with [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0) if you want runnable reasoning traces.
2. Start with [TS-Core](https://github.com/BoggersTheFish/TS-Core) if you want graph/tension runtime experiments.
3. Start with [TS-Benchmarks](https://github.com/BoggersTheFish/TS-Benchmarks) if you want the falsification and scaling harness.
4. Start with [TS-Codex-OS](https://github.com/BoggersTheFish/TS-Codex-OS) if you want project graph, tension ledger, planner, and release receipts for Codex-driven development.
5. Start with CIG repos if you want provenance-aware claim/evidence graph infrastructure.

## Public Golden Path

```text
TS-Start-Here
-> TS-Reasoner-v0: typed tension traces, candidate bridge, export set receipts
-> learned candidate model: proposes/ranks, typed verifier decides
-> limitations: structured synthetic model data, parser-controlled verification, not general reasoning
-> TS-Codex-OS: project-control substrate
-> TS-Benchmarks: falsification and scaling harness
-> TensionLM: model substrate experiment
```

## Fast Route For Funders / Recruiters

Read this as an independent research stack with a sober receipt path:

- **Research theme:** inspectable reasoning systems through constraint graphs, tension telemetry, provenance, and verifier-backed traces.
- **Best proof of discipline:** TS-Reasoner release receipts and benchmark artifacts.
- **Best falsification path:** TS-Benchmarks receipts tied to clean commits, including visible failure cases.
- **Best public orientation:** this repo and the profile README.
- **Current risk:** the work is early, narrow, and partly toy-scope.
- **Current upside:** the artifacts are concrete enough to inspect, run, criticize, and improve.

## What Exists Now

- TS-Reasoner v2.0.0 trains a tiny learned candidate model that ranks/proposes structured candidate claims while typed verifier channels remain proof authority. v1.0.0 established TS-Core-backed typed tension channels, v1.1.0 added candidate containment, v1.2.0 added exported-output ingestion, v1.3.0 stressed messy candidate text, v1.4.0 added an exported-output smoke boundary, v1.5.0 proved one real exported sample could cross the boundary, v1.6.0 preserved export-set failures, and v1.7.0 repaired the deeper-chain support gap exposed by that receipt.
- TS-Benchmarks exists as a falsification-oriented scaling harness with receipts, diagnostics, schema validation, plots, and an explicit scale-free failure issue.
- TS-Codex-OS exists as a local-first project-control substrate for graphing repo state, tensions, planned actions, and receipts.
- TS-Core exists as a graph/tension runtime kernel.
- TensionLM exists as a model-mechanism experiment around sigmoid pairwise tension attention.
- CIG repos exist as provenance-aware claim/evidence graph infrastructure.
- The public website and profile README now route visitors toward the clean research ladder.

## What Is Still Toy-Scope

- TS-Reasoner is not a broad theorem prover or general reasoning model.
- TS-Benchmarks v0.1 is synthetic graph evidence, not real-world knowledge graph scalability.
- TS-Reasoner v2.0.0 is still narrow: the verifier remains parser-controlled, the learned candidate model trains on structured synthetic examples, and this is not a chatbot or live TensionLM integration into the verifier.
- Current learned components are mechanism experiments, not production models.
- CIG confidence and contradiction handling are heuristic.
- TS-Codex-OS is local project-control infrastructure, not an autonomous engineering agent.

## What Would Weaken The TS Approach

The approach would be weakened if:

- tension telemetry does not improve repair, debugging, or verification over simpler baselines,
- low-tension states routinely hide incomplete proofs or unsupported abstentions,
- provenance graphs add complexity without improving contradiction handling,
- verifier-backed traces become too noisy or expensive to inspect,
- scaling diagnostics show the graph substrate fails on common graph families without a bounded fix,
- stronger external benchmarks show no advantage over conventional ranker/verifier baselines.

## Current Technical Ladder

```text
TS-Start-Here
  -> TS-Reasoner-v0
  -> TS-Benchmarks
  -> TensionLM export set boundary
  -> CIG / TS-Codex-OS
```

## Current Technical Step

The current TS-Reasoner release is v2.0.0:

```text
Learned candidate model:
structured reasoning examples
-> tiny pure-Python learned ranker/channel predictor
-> candidate bridge
-> TS-Reasoner typed-channel verification
-> receipt with zero candidate graph contamination
```

The current verifier repair beneath it is v1.7.0:

```text
Deeper-chain support repair:
v1.6 deeper-chain current-limit case
-> structural verifier repair
-> A -> B -> C -> D acceptance tests
-> same candidate containment boundary
```

The current TS-Benchmarks receipt is v0.1:

```text
Synthetic graph scaling harness, clean-commit receipts, plots, baseline comparison, and visible scale-free failure.
```

Lead with bounded artifacts:

```text
Here is a small bounded reasoning system.
Here are the traces.
Here are the failures.
Here is the falsification harness.
Here is what changed from v3 to v10.
```

## Links

- Website: https://www.boggersthefish.com/
- GitHub: https://github.com/BoggersTheFish
- Hugging Face: https://huggingface.co/BoggersTheFish
