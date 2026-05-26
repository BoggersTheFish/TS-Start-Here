# 20-Minute Technical Tour

Audience: skeptical technical visitor who wants to verify signal without reading the whole repo graph.

## 0:00-2:00 - Start Route

Open `TS-Start-Here`.

Say:

> TS is a small public research stack for inspectable reasoning traces, tension telemetry, provenance, and model-mechanism experiments. The claim is not general reasoning. The claim is that the artifacts are concrete enough to inspect, run, criticize, and falsify.

Show:

```text
TS-Start-Here -> TS-Reasoner-v0 v1.0.0 -> release receipt -> limitations -> next TensionLM candidate bridge
```

## 2:00-8:00 - TS-Reasoner v1.0.0 Receipt

Run:

```bash
git clone https://github.com/BoggersTheFish/TS-Reasoner-v0
cd TS-Reasoner-v0
python3 -m unittest discover
python3 scripts/evaluate_typed_tension.py
python3 scripts/generate_typed_channel_release_receipt.py
```

Show:

- typed tension channels in the JSON trace,
- `artifacts/typed_channel_release_receipt.json`,
- scoped calibrator metrics,
- generalization stress Outcome B,
- structural repair deltas.

Say:

> TS-Reasoner v1.0.0 demonstrates TS-Core-backed typed tension reasoning with learned channel calibration. The release includes scoped evaluation, generalization stress testing, structural feature repair, and machine-readable receipts. It preserves trace validity while separating reasoning failures into typed operational channels such as transitivity, identity, directionality, quantifier scope, contradiction, confidence, and surface structure.

## 8:00-13:00 - Inspect Trace Shape

Run:

```bash
python3 inference.py \
  --question "If all seeds are plants and all plants are living and all living are need_water, are all seeds need_water?" \
  --premise "All seeds are plants." \
  --premise "All plants are living." \
  --premise "All living are need_water."
```

Show:

- selected chain,
- global tension,
- `artifacts/latest_trace.json`,
- candidate operation loops.

Say:

> The useful object is not just the answer. It is the trace: candidate chains, graph checks, issue kinds, operation loops, and receipt artifacts.

## 13:00-17:00 - Next Layer: TensionLM Candidate Bridge

Do not present this as solved yet. Present it as the next issue:

```text
TS-Reasoner v1.1.0: TensionLM candidate bridge
```

Show:

- TensionLM/simple bridge proposes candidate claims,
- TS-Reasoner typed channels verify, reject, or abstain,
- trace records proposed, accepted, and rejected candidates with channel reasons.

Say:

> TensionLM is the candidate proposal layer, not the reasoning authority. TS-Reasoner remains the verifier.

## 17:00-20:00 - Limits And Falsification

Show `docs/first_contact.md`.

Say:

> This weakens if tension telemetry does not improve repair, if low-tension states hide unsupported conclusions, if provenance does not improve contradiction handling, or if broader benchmarks show no benefit over simpler ranker/verifier baselines.

Close with:

```text
Start here: https://github.com/BoggersTheFish/TS-Start-Here
Best receipt now: TS-Reasoner-v0 v1.0.0 typed-channel release receipt
Next issue: TS-Reasoner v1.1.0 TensionLM candidate bridge
```
