# README First

This is the current public route for the TS stack:

```text
TS-Start-Here
  -> TS-Reasoner-v0
  -> TensionLM-Wave02-H2H
  -> TensionLM-117M-TS-Reasoner-v10
  -> CIG / TS-Codex-OS
```

Lead with the bounded artifact:

> Here is a small bounded reasoning system. Here are the traces. Here are the
> failures. Here is what changed from v3 to v10.

## 1. TS-Start-Here

Use this repo as the map. It should tell a skeptical reader what exists, what
runs, what is still toy-scope, and which docs or receipts to inspect first.

## 2. TS-Reasoner-v0

TS-Reasoner is the stable public foundation. It is an inspectable reasoning
control loop:

```text
candidate chains -> local/global tension -> verifier loop -> settled trace
```

Start here for:

- one-command local runs,
- JSON trace schema,
- accepted and rejected candidates,
- benchmark receipts,
- known limits.

## 3. TensionLM-Wave02-H2H

This is the controlled comparison lane. Treat TensionLM as a model-mechanism
experiment and candidate proposer, not as a full chatbot claim.

What matters:

- same-size comparisons where possible,
- what changed between runs,
- whether tension-attention improves the reasoning loop,
- what the receipts do not prove.

## 4. TensionLM-117M-TS-Reasoner-v10

This is the integration lane. The clean claim is:

> We are testing whether a tension-attention language model can improve an
> inspectable reasoning loop.

The pipeline should stay:

```text
problem
  -> TS-Reasoner creates reasoning state
  -> TensionLM proposes candidate steps
  -> tension scorer evaluates them
  -> verifier checks them
  -> trace records acceptance, repair, rejection, or failure
```

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
