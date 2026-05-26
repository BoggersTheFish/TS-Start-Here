# TS Receipt Schema

A TS receipt is the credibility layer for a claim. It records what changed, what was verified, what failed, what remains unresolved, and what public claim level is justified.

## Shared Fields

```json
{
  "project": "TS-Reasoner",
  "version": "x.y.z",
  "commit": "...",
  "date": "...",
  "claim": "...",
  "scope": "...",
  "inputs": [],
  "commands_run": [],
  "tests": {},
  "benchmarks": {},
  "artifacts": [],
  "known_limitations": [],
  "tensions_detected": [],
  "tensions_resolved": [],
  "unresolved_tensions": [],
  "public_claim_level": "demo | benchmark | experimental | production"
}
```

## Required Questions

Every release receipt should answer:

- What changed?
- What was verified?
- What failed?
- What can we honestly claim?
- What can we not claim?
- Where is the artifact?

## Claim Levels

- `demo`: runnable artifact proves the interface or behavior on narrow examples.
- `benchmark`: result is tied to an externalized dataset, evaluator, command, commit, and artifact hash.
- `experimental`: result is promising but scoped, unstable, or not yet independently benchmarked.
- `production`: reserved for stable systems with operational monitoring and broad regression coverage.

## Typed Tension Additions

Typed-tension receipts should include:

- channels activated
- resolver actions taken
- reverse fallacy count
- identity collapse count
- unsupported leap count
- contradiction miss count
- abstention correctness
- trace schema validity
- mean channel tension
- mean global tension
