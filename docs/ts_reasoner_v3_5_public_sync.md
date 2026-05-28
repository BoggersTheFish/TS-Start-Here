# TS-Reasoner v3.5.0 Public Sync

TS-Reasoner v3.5.0 is the current flagship verifier-first reasoning release.

Release:

https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v3.5.0

Core line:

    LLMs propose.
    TS verifies.
    Confidence is not proof.
    Typed traces show why.

## What changed

v3.5.0 levels up TS-Reasoner from an internal release ladder into a clearer public research artifact.

It adds:

- v3.1 public surface artifact
- v3.2 cold-reader demo trace
- v3.3 external mini-benchmark adapter
- v3.4 verifier-first reasoning draft
- v3.5 TensionLM proposer boundary smoke

## Boundary

This release does not claim broad NLP understanding, general theorem proving, external benchmark victory, live TensionLM runtime integration, or model confidence as proof authority.

It claims a clearer public surface and bounded smoke artifacts for verifier-first reasoning.

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
