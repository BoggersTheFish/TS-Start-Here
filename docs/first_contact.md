# First Contact

This note is for a skeptical AI researcher who wants the shortest honest read on the BoggersTheFish TS work.

## Core Hypothesis

Reasoning systems become easier to inspect, repair, and falsify when their work is represented as graph state plus explicit constraint pressure.

In TS terms:

- claims, evidence, operations, and dependencies are graph nodes and edges,
- uncertainty, contradiction, malformed structure, and task failure show up as tension,
- repair and abstraction are operations over the graph,
- provenance records make claim state auditable,
- verifier-backed traces make transitions inspectable.

The claim is not that this solves reasoning. The claim is that it creates useful control surfaces for reasoning systems.

## Concrete Artifacts

- [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0): TS-Core-backed typed tension reasoner with learned channel calibration, candidate containment, exported TensionLM-style ingestion, messy candidate stress, real exported TensionLM-side sample receipts, JSON traces, and machine-readable receipts.
- [TensionLM](https://github.com/BoggersTheFish/TensionLM): sigmoid pairwise tension-attention experiments with a public Hugging Face runner.
- [TS-Codex-OS](https://github.com/BoggersTheFish/TS-Codex-OS): local-first project graph, tension ledger, planner, and release receipt substrate.
- [TS-Core](https://github.com/BoggersTheFish/TS-Core): graph/tension runtime kernel.
- [BoggersTheCIG](https://github.com/BoggersTheFish/BoggersTheCIG): local-first provenance-aware concept/evidence graph.
- [cig-ts-engine](https://github.com/BoggersTheFish/cig-ts-engine): CIG engine branch for claim/evidence/provenance experiments.

## Reproducibility Route

Start with TS-Reasoner-v0 because it is the cleanest receipt-backed runnable artifact.

Expected route:

```text
git clone https://github.com/BoggersTheFish/TS-Reasoner-v0
cd TS-Reasoner-v0
python3 -m unittest discover
python3 scripts/evaluate_real_exported_tensionlm_sample.py
```

The current v1.6.0 claim is:

> TS-Reasoner can evaluate multiple exported TensionLM-side candidate samples through a typed verification boundary where malformed, unsupported, contradictory, reverse, and deeper-chain current-limit cases are preserved as failure reasons instead of hidden.

This is a narrow cross-repo exported-set receipt, not live TensionLM integration into the verifier.

## Limits

- The v1.6.0 exported sample set is small, and the verifier remains parser-controlled.
- The deeper-chain support gap is recorded as a current-limit case and is the next repair target.
- The current reasoner is a toy system, not a production theorem prover.
- The current graph/provenance systems use heuristic confidence and contradiction logic.
- Current model experiments are not production language models.
- Older repos may have chaotic names and should be read as historical context unless routed from the flagship docs.

## Falsification / Weakening Conditions

The approach weakens if:

- tension telemetry does not improve repair, debugging, or verification over simpler baselines,
- verifier-backed traces are too noisy or expensive to inspect,
- low-tension states hide unsupported answers or incomplete proofs,
- provenance tracking does not improve contradiction handling or claim auditability,
- stronger external benchmarks show no benefit over conventional verifier/ranker baselines.

## Current Benchmark Direction

The current release direction is:

```text
v1.0.0 = typed tension channels + calibrator + structural repair
v1.1.0 = candidate bridge with adversarial containment
v1.2.0 = exported TensionLM-style adapter
v1.3.0 = messy language candidate stress
v1.4.0 = exported-output smoke boundary
v1.5.0 = real exported TensionLM-side sample crosses into TS-Reasoner as candidate data
v1.6.0 = TensionLM export set evaluation with preserved failure reasons
v1.7.0 = planned deeper-chain support repair
```

The bridge keeps TensionLM in the proposer role:

```text
real or exported TensionLM-side output
  -> adapter normalizes candidate claims
  -> TS-Reasoner typed channels verify, reject, or abstain
  -> trace records which candidates survived and why
```

The useful authority distinction is:

```text
TensionLM proposes.
TS-Reasoner verifies.
The trace explains.
```
