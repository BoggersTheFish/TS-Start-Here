# 20-Minute Technical Tour

Audience: skeptical technical visitor who wants to verify signal without reading the whole repo graph.

## 0:00-2:00 - Start Route

Open `TS-Start-Here`.

Say:

> TS is a small public research stack for inspectable reasoning traces, tension telemetry, provenance, and model-mechanism experiments. The claim is not general reasoning. The claim is that the artifacts are concrete enough to inspect, run, criticize, and falsify.

Show:

```text
TS-Start-Here -> TS-Reasoner-v0 -> TensionLM -> TS-Codex-OS / TS-Core / CIG
```

## 2:00-8:00 - TS-Reasoner v0.9 Receipt

Run:

```bash
git clone https://github.com/BoggersTheFish/TS-Reasoner-v0
cd TS-Reasoner-v0
python3 -m unittest discover
python3 scripts/evaluate_v09_proof_chains.py
```

Show:

- `27` tests pass.
- `artifacts/v09_proof_chain_report.json`.
- `small_proof_chain/full_control_loop = 2/2`.
- `full_control_loop = 10/10`.

Say:

> v0.8 exposed a useful failure: low tension could hide incomplete proof chains. v0.9 only fixes that narrow gap for positive universal all/all chains. It is still toy-scope and normalized.

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

## 13:00-17:00 - TensionLM Public Run

Run from the TensionLM repo:

```bash
python3 scripts/run_public_tensionlm.py \
  --repo-id BoggersTheFish/TensionLM-Curriculum-13M \
  --prompt "If all mammals are animals and all whales are mammals then"
```

Show:

- HF repo id,
- weight file,
- parameter count,
- raw generation,
- limitation note.

Say:

> TensionLM is model-mechanism research around sigmoid pairwise tension attention. Output quality is not the current public claim. The public claim is that the checkpoint route can be loaded and inspected.

## 17:00-20:00 - Limits And Falsification

Show `docs/first_contact.md`.

Say:

> This weakens if tension telemetry does not improve repair, if low-tension states hide unsupported conclusions, if provenance does not improve contradiction handling, or if broader benchmarks show no benefit over simpler ranker/verifier baselines.

Close with:

```text
Start here: https://github.com/BoggersTheFish/TS-Start-Here
Best receipt now: TS-Reasoner-v0 v0.9 proof-chain support
Model mechanism route: TensionLM public HF runner
```
