# TS Credibility Roadmap

This roadmap is the current bridge from toy TS receipts toward benchmark and hardware credibility.

## New Benchmark Substrate

Local repo:

- https://github.com/BoggersTheFish/TS-Benchmarks
- `/home/boggersthefish/BoggersSpace/TS-Benchmarks`

Current implemented slice:

- deterministic TS-Core-style scaling harness
- graph families: random, scale-free, small-world, knowledge-like, provenance, temporal, multi-context
- sparse active-frontier relaxation reference
- degree, PageRank-like, and random residual localization baselines
- benchmark receipt schema
- JSON result and receipt outputs tied to clean commits
- markdown/CSV report generation and PNG plots

Public golden path:

```text
TS-Start-Here
-> TS-Reasoner-v0: reasoning trace contract
-> TS-Codex-OS: project-control substrate
-> TS-Benchmarks: falsification and scaling harness
-> TensionLM: model substrate experiment
```

Current claim boundary:

> TS-Core-style reference relaxation has been tested on deterministic synthetic graphs with auditable runtime, memory, tension, and localization receipts.

Current forbidden claim:

> TS has proven benchmark superiority, real-world knowledge graph scalability, or transformer replacement capability.

## First Observed Result

The first local 100/1k/10k sweep is intentionally treated as a measurement, not a win. Random and small-world graphs relaxed cleanly in the first run. Scale-free graphs produced high remaining tension and zero contradiction-localization F1 in that configuration, which is a real failure signal to investigate before stronger claims.

Public framing:

> v0.1 does not claim TS-Core scales cleanly. It shows where reference TS relaxation succeeds, where it fails, and which diagnostics will drive the next implementation.

## Next Technical Steps

1. Add stronger baselines: NetworkX propagation, belief propagation, Bayesian provenance, vector retrieval.
2. Add noise sweeps and context-splitting metrics.
3. Add 100k-node sparse performance target.
4. Add reasoning benchmark runners for TS-Reasoner variants.
5. Add TensionLM matched softmax controls.
6. Add hardware microbenchmarks and hybrid Graph+LLM contradiction demo.
