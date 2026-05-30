# TS-Reasoner v4.5.0 — Milestone Receipt Pack

TS-Reasoner v4.5.0 is the current verifier-first milestone pack.

Release: https://github.com/BoggersTheFish/TS-Reasoner-v0/releases/tag/v4.5.0

## What v4.5.0 means

v4.5.0 packages the verifier-first ladder from v3.6 through v4.4 into one cold-reader receipt.

It is not a new capability claim. It is a packaging and milestone release that makes the evidence stack easier to inspect.

## Headline receipt

- input reports: 8
- known cases: 114
- known candidates: 151
- wrong accepts: 0
- accepted without typed support: 0
- candidate graph contamination: 0
- all gates passed: true

## Boundary

TS-Reasoner keeps the same public rule:

- generated text is not proof
- confidence is not proof
- external benchmark text is not proof
- GPT-2-style output is not proof
- typed verifier channels remain proof authority

## Role in the TS ecosystem

TS-Reasoner is the verifier-first reasoning harness.

Candidate systems can propose claims, but typed verifier channels decide whether a claim is accepted, rejected, or abstained.
