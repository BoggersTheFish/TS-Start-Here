# TS-Reasoner v10.0.0 Public Sync

TS-Reasoner v10.0.0 supersedes the earlier v3.5.0 public sync as the current flagship verifier-first reasoning release.

Release:

https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v10.0.0

Core line:

    Candidate events enter.
    TS verifies.
    Runtime integrity is not claim truth.
    Typed receipts show why.

## What changed

v10.0.0 levels up TS-Reasoner from a public verifier-first surface into a bounded runtime OS artifact.

It adds:

- runtime policy contracts
- ordered replay
- tamper-evident runtime ledger
- checkpoint and restore
- recovery drill
- v10 CLI, docs, tests, and receipts

## Boundary

This release does not claim broad NLP understanding, general theorem proving, external benchmark victory, live TensionLM runtime integration, or model confidence as proof authority.

It claims a clearer runtime surface and bounded receipts for verifier-first reasoning.

## Flagship evidence

The v3.3 external adapter reports:

    status_accuracy: 1.0
    wrong_accept_count: 0
    accepted_without_typed_support_count: 0
    trace_schema_validity: 1.0

The v3.5 proposer-boundary smoke reports:

    verifier_selection_accuracy: 1.0
    confidence_top_accuracy: 0.0
    verifier_overrode_confidence_count: 4
    accepted_without_typed_support_count: 0
    candidate_graph_contamination_count: 0
    live_tensionlm_runtime_loaded: false

## Interpretation

The point is not that the model is always right.

The point is that confidence is not proof.

A proposer can be confidently wrong, while the typed verifier still selects the supported claim and blocks unsupported candidates.
