# Public Signal Reduction Checklist

Canonical route:

```text
BoggersTheFish profile
-> TS-Start-Here
-> TS-Reasoner-v0
-> TensionLM
-> TS-Codex-OS / TS-Core / CIG
```

## Completed Locally

- `TS-Start-Here` routes technical visitors through the same canonical path.
- `TS-Reasoner-v0` has v1.5.0 typed verification receipts from typed channels through a real exported TensionLM-side sample boundary.
- `TensionLM` has a public Hugging Face load/run script.
- Local Hugging Face model-card checkouts route back to `TS-Start-Here` and `TensionLM`.
- Profile README and public repo index use `TensionLM`, not `bozo`, for the first-contact route.
- A 20-minute technical tour exists at `docs/technical_tour_20_min.md`.

## Public Metadata To Confirm

- GitHub repo `bozo` renamed to `TensionLM`.
- GitHub repo descriptions/topics match `docs/repo_metadata_recommendations.md`.
- Hugging Face model cards published from the local card updates.
- TS-Reasoner v1.5.0 release created with `artifacts/real_exported_tensionlm_sample_receipt.json`.

Remaining UI-only check:

- Pinned repos should be ordered as `TS-Start-Here`, `TS-Reasoner-v0`, `TensionLM`, `TS-Codex-OS`, `TS-Core`, `BoggersTheCIG`. The correct six repos are pinned; GitHub's available CLI/GraphQL schema in this run did not expose a profile-pin reorder mutation.

## Non-Claims

- No broad benchmark claim.
- No production theorem-prover claim.
- No instruction-tuned assistant claim for TensionLM.
- No new repo graph expansion.
