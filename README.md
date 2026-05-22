# TS-Start-Here

**Public map for the BoggersTheFish Thinking System / TS research stack.**

This repo is the public orientation map for BoggersTheFish Thinking System work.

## Read This First

TS is being developed as an engineering framework for inspectable reasoning
systems: constraint graphs, tension telemetry, provenance-aware claim graphs,
verifier-backed traces, and small reproducible reasoning/model artifacts.

The goal is not to claim a finished general reasoning model. The goal is to make the current TS artifacts readable: what exists, what each repo proves, what is still toy-scope, and what the next technical step is.

Start here:

- [TS Ecosystem Map](docs/TS_ECOSYSTEM_MAP.md)
- [First Contact](docs/first_contact.md)
- [Repo Taxonomy](docs/repo_taxonomy.md)

## Fast Route For Researchers

1. Read [First Contact](docs/first_contact.md) for the hypothesis, runnable artifacts, current limits, and falsification points.
2. Read [TS Ecosystem Map](docs/TS_ECOSYSTEM_MAP.md) for the repo ladder and current release receipts.
3. Inspect [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0), especially the v0.8 external benchmark harness and proof-chain failure.
4. Inspect [bozo / TensionLM](https://github.com/BoggersTheFish/bozo) for the sigmoid pairwise tension-attention experiment.

## Fast Route For Builders

1. Start with [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0) if you want runnable reasoning traces.
2. Start with [TS-Core](https://github.com/BoggersTheFish/TS-Core) if you want the graph dynamics substrate.
3. Start with [TS-Codex-OS](https://github.com/BoggersTheFish/TS-Codex-OS) if you want the project graph, tension ledger, and release receipt workflow.
4. Start with [BoggersTheCIG](https://github.com/BoggersTheFish/BoggersTheCIG) or [cig-ts-engine](https://github.com/BoggersTheFish/cig-ts-engine) if you want provenance-aware claim/evidence graph work.

## Current Honest Status

- TS-Reasoner has versioned public releases and a stable JSON trace contract.
- TS-Reasoner v0.8 runs a curated externalized small benchmark harness, not a broad reasoning benchmark.
- The v0.8 result is useful because it exposes a concrete failure: the loop can settle into low-tension abstention instead of completing a transitive proof chain.
- TS-Codex-OS is a local file-based project-control substrate, not an autonomous agent runtime.
- TensionLM / bozo contains language-model mechanism experiments, not a proven replacement for transformer language models.

## Flagship Repo Ladder

```text
TS-Start-Here
  -> TS-Reasoner-v0
  -> TS-Codex-OS
  -> TS-Core
  -> TensionLM / bozo
  -> BoggersTheCIG / cig-ts-engine
```

## Known Limitations

- Current reasoning tasks are narrow and toy-scope unless a repo states otherwise with receipts.
- Current benchmark harnesses are small and curated.
- Current learned components are smoke-test experiments, not production models.
- Some older repos have chaotic names because they were exploratory prototypes.
- Public claims should stay tied to runnable artifacts, tests, traces, and release receipts.

## Next Technical Step

The next TS-Reasoner milestone is v0.9:

```text
Transitive proof-chain support
```

v0.9 should test whether explicit bridge construction can reduce proof-chain failures without letting low-tension abstention count as proof completion.

## Links

- Website: https://www.boggersthefish.com/
- GitHub: https://github.com/BoggersTheFish
- Hugging Face: https://huggingface.co/BoggersTheFish
