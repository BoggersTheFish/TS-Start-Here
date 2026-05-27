# README First

This is the current public route for the TS stack:

```text
TS-Start-Here
  -> TS-Reasoner-v0
  -> typed verification and exported-sample receipts
  -> current limitations
  -> deeper-chain support repair
  -> CIG / TS-Codex-OS
```

Lead with the bounded artifact:

> Here is TS-Reasoner v1.6.0. Here is the exported TensionLM-side sample set.
> Here is the typed verification receipt. Here are the preserved failure
> reasons. Here is the next deeper-chain repair step.

## 1. TS-Start-Here

Use this repo as the map. It should tell a skeptical reader what exists, what
runs, what is still toy-scope, and which docs or receipts to inspect first.

## 2. TS-Reasoner-v0

TS-Reasoner is the stable public foundation. The current release claim is:

> TS-Reasoner can consume real exported TensionLM-side candidate data through a typed verification boundary where provenance is preserved, model confidence remains metadata, and typed channels remain the proof authority.

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

## 4. TS-Reasoner v1.6.0: TensionLM Export Set Boundary

This integration lane is now active through v1.6.0. The clean claim is:

> TensionLM-side outputs enter as candidate data. TS-Reasoner verifies them. Candidate confidence is not proof.

The pipeline should stay:

```text
real or exported TensionLM-side output
  -> adapter normalizes candidate claims
  -> TS-Reasoner typed channels verify, reject, or abstain
  -> trace records which candidates survived and why
```

The next technical step is v1.7.0: repair the deeper-chain support failure that
v1.6.0 preserved as a current-limit case.

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
