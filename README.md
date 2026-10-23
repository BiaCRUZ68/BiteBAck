# Biteback — History Has a Taste
## Authoritative Video Production Playbook

**Playbook version:** 1.0.0  
**Status:** Active default for all Biteback videos until the channel owner explicitly updates it.  
**Companion private plugin:** [History Behind the Bite](https://chatgpt.com/plugins/plugins_6ad911a995ac81918370d1d73551f0ff) (v1.1.0)

This repository is the source of truth for channel production rules. Read `docs/BITEBACK_WORKFLOW.md` before developing an episode. Character descriptions and templates live under `docs/`.

## Non-negotiable sequence
1. Research the topic and create an evidence ledger.
2. Draft the **complete narration script first**.
3. Review factual accuracy, fluency, coherence, repetition, hook strength, transitions, and payoff. Revise iteratively.
4. **Do not create image/video prompts until the user approves the complete script.**
5. Once approved, map every narration segment to a visual beat and deliver detailed image and video prompts separately.
6. Review the whole package against the quality checklist before calling it production-ready.

## Core constraints
- English-language, evidence-led historical food documentary; usual long-form target: 8–10 minutes, guided by story quality and actual narration timing.
- Exact narration text accompanies every visual beat.
- Every beat has a standalone copy-ready image prompt and a standalone copy-ready video prompt.
- Video prompts: ASMR and natural ambience only, synchronized to visible action. **No narrator, voice-over, dialogue, speech, lip-sync, or music.**
- Animation prompts require visible physical action with timing and cause/effect; camera movement is secondary.
- Compose in full 16:9; main subject and action must be large, legible, and visually important. Avoid tiny people or an empty distant city.
- Alex and Lia are silent visual investigators. When they appear, name them as Actor 1: Alex / Actor 2: Lia, include the full descriptions, and explicitly require the attached official character reference image. Never force them into a historical reconstruction where they do not belong.
- Clearly distinguish documented evidence from plausible reconstruction, disputed claims, and unknowns. Never invent historical recipes, citations, quotes, or details.

See [the complete workflow](docs/BITEBACK_WORKFLOW.md), [character bible](docs/CHARACTER_BIBLE.md), [storyboard template](docs/STORYBOARD_TEMPLATE.md), [evidence ledger](docs/EVIDENCE_LEDGER_TEMPLATE.md), and [QA checklist](docs/QA_CHECKLIST.md).

## Separate playbook in this repository
The automotive Reels workflow is a separate project and does not change Biteback's historical-food production rules:
- [Centro Automotivo São Luiz — Reels Storytelling Playbook](docs/CENTRO_AUTOMOTIVO_SAO_LUIZ_REELS_PLAYBOOK.md)

## Versioning
Changes to permanent rules require an explicit request from the channel owner. Update the playbook version and append a dated changelog entry. Episode-specific choices do not silently change the permanent workflow.

### Changelog
- 1.0.0 — 2026-10-23: Initial authoritative production workflow, full Alex/Lia consistency rules, narration-mapped dual prompts, and ASMR-only video generation standard.
