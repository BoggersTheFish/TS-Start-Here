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

- [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0): deterministic Python toy reasoner with candidate chains, CIG checks, tension issues, repair suggestions, operation loops, and JSON traces.
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
python3 scripts/evaluate_v09_proof_chains.py
```

The current v0.9 receipt reports:

- `27` unit tests passing,
- `10` curated externalized benchmark tasks,
- `direct`: `4/10` correct,
- `random_selector`: `6/10` correct,
- `ranker_only`: `10/10` correct,
- `full_control_loop`: `10/10` correct, `10/10` settled, mean final tension `0.0`,
- `small_proof_chain/full_control_loop`: `2/2` correct.

This is a narrow receipt, not a broad benchmark claim.

## Limits

- The v0.9 benchmark receipt is small, curated, and normalized into TS-Reasoner relation templates.
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

The current benchmark direction is TS-Reasoner v0.9:

```text
Transitive proof-chain support for positive universal all/all chains
```

v0.8 exposed the failure: settlement is not proof completion. The control loop could settle into low-tension abstention on small proof-chain tasks.

v0.9 tests:

```text
small_proof_chain failure
  -> detect unresolved transitive edge
  -> construct bridge candidate
  -> verify bridge against premises
  -> rerun control loop
  -> confirm abstention converts into valid proof
```

The useful telemetry distinction is:

```text
settled_abstention
settled_answer
settled_proof_complete
settled_invalid
```
