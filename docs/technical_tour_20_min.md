# 20-Minute Technical Tour

Audience: skeptical technical visitor who wants to verify signal without reading the whole repo graph.

## 0:00-2:00 - Start Route

Open `TS-Start-Here`.

Say:

> TS is a small public research stack for inspectable reasoning traces, tension telemetry, provenance, and model-mechanism experiments. The claim is not general reasoning. The claim is that the artifacts are concrete enough to inspect, run, criticize, and falsify.

Show:

```text
TS-Start-Here -> TS-Reasoner-v0 v1.5.0 -> exported-sample receipt -> limitations -> next export set evaluation
```

## 2:00-8:00 - TS-Reasoner v1.5.0 Receipt

Run:

```bash
git clone https://github.com/BoggersTheFish/TS-Reasoner-v0
cd TS-Reasoner-v0
python3 -m unittest discover
python3 scripts/evaluate_real_exported_tensionlm_sample.py
```

Show:

- typed-channel verification in the candidate results,
- `artifacts/real_exported_tensionlm_sample_receipt.json`,
- preserved source provenance from the existing TensionLM-side eval artifact,
- verifier-over-confidence behavior,
- zero candidate graph contamination.

Say:

> TS-Reasoner can consume real exported TensionLM-side candidate data through a typed verification boundary where provenance is preserved, model confidence remains metadata, and typed channels remain the proof authority.

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

## 13:00-17:00 - Bridge Layer: TensionLM Candidate Data

Do not present this as live model integration. Present it as exported candidate
data under verifier authority:

```text
TS-Reasoner v1.5.0: real exported TensionLM-side sample
```

Show:

- exported TensionLM-side data proposes candidate claims,
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
Best receipt now: TS-Reasoner-v0 v1.5.0 real exported TensionLM-side sample receipt
Next issue: TS-Reasoner v1.6.0 TensionLM export set evaluation
```
