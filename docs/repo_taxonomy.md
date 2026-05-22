# Repo Taxonomy

This taxonomy exists to make the public GitHub surface readable. The work has a long prototype history, but the current first-contact path should be clear.

## Flagship Repos

These repos should be read first.

| Repo | Role | Status |
| --- | --- | --- |
| [TS-Start-Here](https://github.com/BoggersTheFish/TS-Start-Here) | Public orientation map for the TS ecosystem. | flagship |
| [TS-Reasoner-v0](https://github.com/BoggersTheFish/TS-Reasoner-v0) | Inspectable toy reasoning telemetry, trace contract, verifier-backed loop, and release receipts. | flagship |
| [TS-Codex-OS](https://github.com/BoggersTheFish/TS-Codex-OS) | Local-first project graph, tension ledger, planner, and release receipt substrate for Codex-driven development. | flagship |
| [TS-Core](https://github.com/BoggersTheFish/TS-Core) | Lightweight graph dynamics kernel for propagation, relaxation, stability, and tension experiments. | flagship |
| [bozo / TensionLM](https://github.com/BoggersTheFish/bozo) | Sigmoid pairwise tension-attention experiments as an inspectable alternative to softmax attention. | flagship |
| [BoggersTheCIG](https://github.com/BoggersTheFish/BoggersTheCIG) / [cig-ts-engine](https://github.com/BoggersTheFish/cig-ts-engine) | Provenance-aware claim/evidence graph work for contradiction tracking and confidence updates. | active core |

## Active Experiments

These repos may contain useful ideas but should not be the first thing a cold visitor reads.

| Repo | Role | Status |
| --- | --- | --- |
| [BoggersTheAI](https://github.com/BoggersTheFish/BoggersTheAI) | Experimental local TS runtime combining graph memory, tools, dashboard, and optional LLM synthesis. | active experiment |
| [TS-WaveLab](https://github.com/BoggersTheFish/TS-WaveLab) | Interactive TS tension graph and wave propagation lab. | active experiment |
| [TinyLLM](https://github.com/BoggersTheFish/TinyLLM) | Minimal word-level attractor language-model experiment. | active experiment |
| [TS-MultiAgent](https://github.com/BoggersTheFish/TS-MultiAgent) | Early multi-agent tension coordination prototype. | active experiment |
| [ts-visualizer](https://github.com/BoggersTheFish/ts-visualizer) | Visualization layer for TS graph and tension-field experiments. | active experiment |

## Historical Prototypes

These repos are part of the research history but should be labelled as historical, experimental, duplicated, or superseded.

Examples include:

- `GOAT-TS`
- `GOAT-TS-DEVELOPMENT`
- `GOAT-TS-LITE`
- `GOAT-TS-SUPERLITE`
- `GOAT-PUBLIC_TEST`
- `GOAT-OS`
- `BoggersTheMind`
- `BoggersTheSystem`
- `BoggersThePulse`
- `BoggersBrain`
- `BoggersTheLLM`
- `ts-llm`
- `woke-baby-llm`
- `BoggersTheAI-Dev`
- `BoggersTheCIG_v2`
- `CIG-APP-V1`
- `BAGI`
- `BLM`
- `schizo_bet`
- `hehe`

They should not be deleted or rewritten out of history. They should be routed around with clear README notes.

## Naming Caveat

Some older repos have chaotic names because they were exploratory prototypes. That is real history, but it should not define the first-contact research story.

The clean research path is now:

```text
TS-Start-Here -> TS-Reasoner-v0 -> TS-Codex-OS -> TS-Core / TensionLM / CIG
```

Use that path when describing the work publicly.

## Recommended Historical Note

Add this to older prototype READMEs over time:

```md
> Historical prototype.
> Current public research route: TS-Start-Here -> TS-Reasoner-v0 -> TS-Codex-OS -> TS-Core / TensionLM / CIG.
> Start here: https://github.com/BoggersTheFish/TS-Start-Here
```
