# TS-Start-Here

**Canonical ecosystem map for the BoggersTheFish TS / Thinking System research stack.**

## Read This First

TS is an engineering framework for modelling information transfer through graph structure, constraint pressure, contradiction handling, provenance, and relaxation.

The current public artifacts are mostly toy-scope or narrow-scope, but they are real, inspectable, runnable, and increasingly receipt-backed. The goal is not to claim a finished general reasoning model. The goal is to make the current systems readable: what exists, what can run, what is still limited, and what would weaken the approach.

Core docs:

- [TS Ecosystem Map](docs/TS_ECOSYSTEM_MAP.md)
- [First Contact](docs/first_contact.md)
- [Repo Taxonomy](docs/repo_taxonomy.md)
- [Flagship Route](docs/flagship_route.md)
- [20-Minute Technical Tour](docs/technical_tour_20_min.md)
- [Public Signal Reduction Checklist](docs/public_signal_reduction_checklist.md)
- [GitHub Cleanup Plan](docs/github_cleanup_plan.md)
- [Repo Metadata Recommendations](docs/repo_metadata_recommendations.md)

## Fast Route For Researchers

1. Read [First Contact](docs/first_contact.md) for the core hypothesis, concrete artifacts, reproducibility route, limits, and falsification points.
2. Inspect [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0) for verifier-backed traces, release receipts, and the v0.9 proof-chain receipt.
3. Inspect [TensionLM](https://github.com/BoggersTheFish/TensionLM) for sigmoid pairwise tension-attention mechanism experiments and the public Hugging Face runner.
4. Inspect [BoggersTheCIG](https://github.com/BoggersTheFish/BoggersTheCIG) or [cig-ts-engine](https://github.com/BoggersTheFish/cig-ts-engine) for provenance-aware claim/evidence graph work.

## Fast Route For Builders

1. Start with [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0) if you want runnable reasoning traces.
2. Start with [TS-Core](https://github.com/BoggersTheFish/TS-Core) if you want graph/tension runtime experiments.
3. Start with [TS-Codex-OS](https://github.com/BoggersTheFish/TS-Codex-OS) if you want project graph, tension ledger, planner, and release receipts for Codex-driven development.
4. Start with CIG repos if you want provenance-aware claim/evidence graph infrastructure.

## Fast Route For Funders / Recruiters

Read this as an independent research stack with a sober receipt path:

- **Research theme:** inspectable reasoning systems through constraint graphs, tension telemetry, provenance, and verifier-backed traces.
- **Best proof of discipline:** TS-Reasoner release receipts and benchmark artifacts.
- **Best public orientation:** this repo and the profile README.
- **Current risk:** the work is early, narrow, and partly toy-scope.
- **Current upside:** the artifacts are concrete enough to inspect, run, criticize, and improve.

## What Exists Now

- TS-Reasoner has versioned public releases, tests, JSON traces, repair telemetry, a v0.8 externalized small benchmark harness, and a v0.9 proof-chain closure receipt.
- TS-Codex-OS exists as a local-first project-control substrate for graphing repo state, tensions, planned actions, and receipts.
- TS-Core exists as a graph/tension runtime kernel.
- TensionLM exists as a model-mechanism experiment around sigmoid pairwise tension attention.
- CIG repos exist as provenance-aware claim/evidence graph infrastructure.
- The public website and profile README now route visitors toward the clean research ladder.

## What Is Still Toy-Scope

- TS-Reasoner is not a broad theorem prover or general reasoning model.
- The v0.9 proof-chain receipt is small, curated, and normalized.
- Current learned components are mechanism experiments, not production models.
- CIG confidence and contradiction handling are heuristic.
- TS-Codex-OS is local project-control infrastructure, not an autonomous engineering agent.

## What Would Weaken The TS Approach

The approach would be weakened if:

- tension telemetry does not improve repair, debugging, or verification over simpler baselines,
- low-tension states routinely hide incomplete proofs or unsupported abstentions,
- provenance graphs add complexity without improving contradiction handling,
- verifier-backed traces become too noisy or expensive to inspect,
- stronger external benchmarks show no advantage over conventional ranker/verifier baselines.

## Current Technical Ladder

```text
TS-Start-Here
  -> TS-Reasoner-v0
  -> TensionLM
  -> TS-Codex-OS / TS-Core / BoggersTheCIG
```

## Current Technical Step

The current TS-Reasoner receipt is v0.9:

```text
Transitive proof-chain support for positive universal all/all chains
```

v0.8 proved the harness works, but exposed the failure mode: settlement is not proof completion. v0.9 closes that narrow gap on the existing two small proof-chain tasks while keeping the benchmark claim toy-scope and normalized.

## Links

- Website: https://www.boggersthefish.com/
- GitHub: https://github.com/BoggersTheFish
- Hugging Face: https://huggingface.co/BoggersTheFish
