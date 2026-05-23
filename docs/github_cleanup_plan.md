# GitHub Cleanup Plan

This plan makes the public GitHub surface read as a serious independent AI research stack while preserving development history.

## Phase 1: Profile, Pins, Metadata

- Use `BoggersTheFish/BoggersTheFish` as the profile README.
- Pin repos in the flagship order:
  1. `TS-Start-Here`
  2. `TS-Reasoner-v0`
  3. `TS-Codex-OS`
  4. `TS-Core`
  5. `TensionLM`
  6. `BoggersTheCIG`
- Add sober repo descriptions and topics.
- Do not delete historical repos.

## Phase 2: Flagship README Standardization

Each flagship README should include:

- what it is,
- what it is not,
- runnable path,
- artifact/receipt path,
- known limitations,
- relationship to the rest of TS,
- next technical step.

## Phase 3: CIG Cleanup

Reframe `BoggersTheCIG` as:

```text
Local-first provenance-aware concept graph for confidence-weighted claims, evidence, contradictions, Obsidian-readable memory, and TS-style inspectable knowledge state.
```

Move autonomous/self-improvement language into an experimental section. Make clear that it requires human review and is not a finished autonomous reasoner.

## Phase 4: Historical Repo Routing Notes

Add the historical note to older repos:

```md
> Historical prototype.
> Current public research route: TS-Start-Here -> TS-Reasoner-v0 -> TensionLM -> TS-Codex-OS / TS-Core / CIG.
> Start here: https://github.com/BoggersTheFish/TS-Start-Here
```

Apply this before archiving or de-emphasizing anything.

## Phase 5: Website Alignment

- Homepage should route technical visitors to `TS-Start-Here`.
- Projects page should use the same flagship ordering as GitHub.
- CIG page should use the sober CIG framing.
- Proof Ranker / TS-Reasoner page should foreground receipts and limitations.
- Support/BGC material should stay separate from the research credibility path.
