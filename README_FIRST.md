# README First

This is the current public route for the TS stack:

```text
TS-Start-Here
  -> TS-Reasoner-v0
  -> verifier-first runtime OS receipts
  -> current limitations
  -> policy contracts / recovery drill / checkpoint restore
  -> CIG / TS-Codex-OS
```

Lead with the bounded artifact:

> Here is TS-Reasoner v10.0.0. Here is the verifier-first runtime OS receipt.
> Here are the policy contracts, replay ledger, checkpoint/restore, recovery
> drill, and proof-boundary limits.

## 1. TS-Start-Here

Use this repo as the map. It should tell a skeptical reader what exists, what
runs, what is still toy-scope, and which docs or receipts to inspect first.

## 2. TS-Reasoner-v0

TS-Reasoner is the stable public foundation. The current release claim is:

> TS-Reasoner v10.0.0 processes candidate runtime events through policy contracts, replay, tamper-evident ledger, checkpoint/restore, and recovery while generated text, model confidence, and runtime integrity remain non-proof without typed verifier support.

Start here for:

- one-command local runs,
- JSON trace schema,
- typed channel traces,
- accepted and rejected resolver operations,
- release receipts,
- known limits.

## 3. TensionLM-Wave02-H2H

This is the controlled comparison lane. Treat TensionLM as a model-mechanism
experiment and candidate proposer, not as a full chatbot claim.

What matters:

- same-size comparisons where possible,
- what changed between runs,
- whether tension-attention improves the reasoning loop,
- what the receipts do not prove.

## 4. TS-Reasoner v10.0.0: Verifier-First Runtime OS

This integration lane is now active through v10.0.0. The clean claim is:

> Candidate events enter as candidate data. TS-Reasoner routes them through policy contracts and typed verifier boundaries. Candidate confidence is not proof.

The pipeline should stay:

```text
candidate event
  -> runtime policy contract
  -> TS-Reasoner typed verifier boundary
  -> quarantine / repair / branch / check
  -> replay ledger, checkpoint/restore, receipt
```

The next technical step is keeping GitHub releases, website surfaces, README,
model card, and release authority synchronized around v10.

## 5. CIG / TS-Codex-OS

CIG and TS-Codex-OS are support infrastructure:

- CIG: provenance, claim/evidence graphs, contradiction pressure.
- TS-Codex-OS: repo graph, release-control receipts, project-state tension.

They should reinforce the trace contract rather than pull the first-contact
story back into broad theory.

## Current Rule

Do not lead with “this could be huge.”

Lead with:

- what runs,
- where the trace is,
- what passed,
- what failed,
- what changed between versions.
