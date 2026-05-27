# Repo Taxonomy

This taxonomy makes the public GitHub surface readable. The work has a long prototype history, but the current first-contact path should be stable and sober.

## First-Contact Repos

These repos should be read first by skeptical technical visitors.

| Repo | Role | Why first |
| --- | --- | --- |
| [TS-Start-Here](https://github.com/BoggersTheFish/TS-Start-Here) | Ecosystem map and taxonomy. | Gives the clean route and limitations before visitors hit older prototypes. |
| [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0) | TS-Core-backed typed tension traces, candidate containment, exported TensionLM-style ingestion, messy candidate stress, real exported TensionLM-side sample receipts, and export set failure preservation. | Best current runnable receipt path. |
| [TS-Codex-OS](https://github.com/BoggersTheFish/TS-Codex-OS) | Project graph, tension ledger, planner, release receipts. | Shows TS applied to project/release control. |
| [TS-Core](https://github.com/BoggersTheFish/TS-Core) | Graph/tension runtime kernel. | Core runtime substrate. |
| [TensionLM](https://github.com/BoggersTheFish/TensionLM) | Sigmoid pairwise tension attention experiments with a public HF runner. | Model-mechanism branch. |
| [BoggersTheCIG](https://github.com/BoggersTheFish/BoggersTheCIG) | Provenance-aware concept/evidence graph. | Knowledge/provenance branch. |

## Active Core Repos

These are active or useful infrastructure, but some still need README cleanup before they are ideal first-contact material.

- `cig-ts-engine`: possible cleaner CIG/TS engine branch.
- `boggersthefish-site`: public website and project archive.
- `BoggersTheAI`: experimental local TS runtime; needs sober framing.
- `TS-WaveLab`: visual lab for graph/tension dynamics.
- `TinyLLM`: small educational model experiment.

## Old Prototype Branches

Older branches are part of the history but should be labelled clearly:

- `GOAT-TS`
- `BoggersTheMind`
- `BoggersTheLLM`
- `woke-baby-llm`
- `BoggersTheSystem`
- `BoggersThePulse`
- `BoggersBrain`
- `ts-llm`
- `BAGI`
- `BLM`
- `schizo_bet`
- `hehe`

These should not be deleted or rewritten out of history. They should get routing notes pointing to the current flagship route.

## Duplicate / Superseded Branches

These should be archived, marked historical, or clearly pointed at the canonical repo:

- `GOAT-TS-DEVELOPMENT`
- `GOAT-TS-LITE`
- `GOAT-TS-SUPERLITE`
- `GOAT-PUBLIC_TEST`
- `GOAT-OS`
- `BoggersTheAI-Dev`
- `BoggersTheCIG_v2`
- `CIG-APP-V1`
- `ts-wave-lab`
- `ts-wave-colony`
- `ts-visualizer`

## Naming Caveat

Some older repo names are chaotic because they were exploratory prototypes. That is real development history, but it should not be the first-contact research story.

The clean route is:

```text
TS-Start-Here -> TS-Reasoner-v0 v1.6.0 -> TensionLM export set receipt -> limitations -> next deeper-chain repair
```

## Where A Serious Reviewer Should Start

1. Read the profile README.
2. Read this repo's README.
3. Read [First Contact](first_contact.md).
4. Run TS-Reasoner-v0 and inspect its v1.6.0 TensionLM export set receipt.
5. Review the v1.0.0 through v1.6.0 ladder before treating TensionLM outputs as anything more than candidate data.
