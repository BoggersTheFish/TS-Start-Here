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

- [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0): TS-Core-backed typed tension reasoner with learned channel calibration, stress tests, structural repair, JSON traces, and machine-readable receipts.
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
python3 scripts/evaluate_typed_tension.py
python3 scripts/generate_typed_channel_release_receipt.py
```

The current v1.0.0 claim is:

> TS-Reasoner v1.0.0 demonstrates TS-Core-backed typed tension reasoning with learned channel calibration. The release includes scoped evaluation, generalization stress testing, structural feature repair, and machine-readable receipts. It preserves trace validity while separating reasoning failures into typed operational channels such as transitivity, identity, directionality, quantifier scope, contradiction, confidence, and surface structure.

This is a narrow receipt, not a broad benchmark or natural-language robustness claim.

## Limits

- The v1.0.0 benchmark and stress receipts are synthetic, small, and parser-controlled.
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
v1.0.0 = typed reasoning substrate
v1.1.0 = TensionLM candidate bridge
v1.2.0 = messy natural-language stress
v1.3.0 = CIG memory write/read receipts
v1.4.0 = TS-Codex ecosystem truth-check
```

The v1.1.0 bridge should keep TensionLM in the proposer role:

```text
messy input text
  -> TensionLM/simple bridge proposes candidate claims
  -> TS-Reasoner typed channels verify, reject, or abstain
  -> trace records which candidates survived and why
```

The useful authority distinction is:

```text
TensionLM proposes.
TS-Reasoner verifies.
The trace explains.
```
