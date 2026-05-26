# TS Credibility Roadmap

This roadmap is the current bridge from toy TS receipts toward benchmark and hardware credibility.

## New Benchmark Substrate

Local repo:

- `/home/boggersthefish/BoggersSpace/TS-Benchmarks`

Current implemented slice:

- deterministic TS-Core-style scaling harness
- graph families: random, scale-free, small-world, knowledge-like, provenance, temporal, multi-context
- sparse active-frontier relaxation reference
- degree and PageRank-like localization baselines
- benchmark receipt schema
- JSON result and receipt outputs
- markdown/CSV report generation

Current claim boundary:

> TS-Core-style reference relaxation has been tested on deterministic synthetic graphs with auditable runtime, memory, tension, and localization receipts.

Current forbidden claim:

> TS has proven benchmark superiority, real-world knowledge graph scalability, or transformer replacement capability.

## First Observed Result

The first local 100/1k/10k sweep is intentionally treated as a measurement, not a win. Random and small-world graphs relaxed cleanly in the first run. Scale-free graphs produced high remaining tension and zero contradiction-localization F1 in that configuration, which is a real failure signal to investigate before stronger claims.

## Next Technical Steps

1. Add stronger baselines: NetworkX propagation, belief propagation, Bayesian provenance, vector retrieval.
2. Add noise sweeps and context-splitting metrics.
3. Add 100k-node sparse performance target.
4. Add reasoning benchmark runners for TS-Reasoner variants.
5. Add TensionLM matched softmax controls.
6. Add hardware microbenchmarks and hybrid Graph+LLM contradiction demo.
