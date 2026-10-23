# Biteback Video Production Workflow
**Version:** 1.0.0  
**Effective date:** 2026-10-23  
**Status:** Authoritative. Applies to every Biteback video until explicitly updated by the channel owner.

## 1. Purpose and editorial promise
Biteback's slogan is **“History Has a Taste.”** Historical food is the entry point into a well-researched story about people, power, trade, technology, belief, daily life, migration, class, conflict, and cultural change. Food must remain causally relevant through the episode, not only appear in the opening hook.

Default language: English. Default format: long-form, narration-led historical food documentary, usually 8–10 minutes. Runtime is a planning target, not a license to add filler. Let the story and recorded narration determine actual timing.

## 2. Workflow stages: strict gates

### Stage A — Topic and research
1. Define the central question and the specific food, ingredient, preparation, ration, eating practice, supply chain, or culinary object at its center.
2. Explain why the question matters beyond food alone.
3. Check that sufficient credible evidence exists. Prefer primary sources, archaeology/material evidence, scholarly books and papers, museums, archives, heritage institutions, and reputable scholarly syntheses.
4. Record key claims in the evidence ledger before presenting them as fact.
5. For each claim, distinguish: directly attested; supported interpretation; plausible reconstruction; contested; or unknown.
6. Verify dates, geography, historical terminology, translations, and source context. Never invent citations, quotations, recipe steps, measurements, or certainty.
7. Record any disputes and the wording needed to convey uncertainty responsibly.
8. For food history, distinguish what was available, what was eaten, what was documented, and what is merely plausible. A single source does not establish a universal recipe or practice.

### Stage B — Complete script FIRST
Write the complete narration before generating visual prompts. Build a coherent episode, typically:
1. Cold open: a specific question, contradiction, mystery, or surprising consequence.
2. Establish the food and central question.
3. Place people and events in a specific time and location.
4. Explain ingredients, production, access, preparation, transportation, preservation, trade, or consumption as relevant.
5. Reveal the larger historical system connected to the food.
6. Present the strongest evidence-led discovery, complication, or qualification.
7. Answer the opening question and land a memorable final insight.

Script quality requirements:
- A strong hook without misleading clickbait.
- A clear central question and a satisfying answer.
- Logical progression: each block contributes new information, advances the explanation, or changes the viewer's understanding.
- Transitions create a reason to continue into the next block.
- Remove repeated facts, restated claims, filler, redundant rhetorical questions, and unnecessary scene-setting.
- Use precise, concrete, accessible language while retaining appropriate historical vocabulary.
- Keep food as a meaningful part of the causal explanation.
- Mark uncertain reconstructions rather than narrating them as established facts.
- Verify every substantive factual claim against the evidence ledger.
- Do not force every episode into identical chapter labels. Use a structure suited to the topic.

### Stage C — Script review and approval gate
Review the ENTIRE script before any prompt production:
- Factual accuracy and source support.
- Fluency, voice, grammar, clarity, and natural spoken rhythm.
- Narrative coherence and chronology.
- Hook strength and resolution.
- Block-to-block transitions.
- Semantic repetition and redundant examples.
- Whether each block introduces useful new information.
- Whether the conclusion answers the main question.
- Approximate runtime against recorded/estimated narration speed, without padding.

Revise as needed and return the complete updated script. The user must approve the complete script before storyboard/prompt production begins. If the user requests a script change later, update the script and identify any affected narration cues; do not silently alter already approved narration.

**Hard stop:** Before explicit script approval, do not generate the episode's image/video prompts. You may discuss visual strategy at a high level, but do not start shot-by-shot prompt production.

### Stage D — Lock script and make a narration master
After approval:
1. Mark the exact approved script version as LOCKED.
2. Create a stable version identifier/date.
3. Preserve the narration verbatim in storyboard cues. Never paraphrase cue text.
4. When audio exists, time visuals to the actual narration waveform/audio duration and natural pauses. Do not guess timing solely by counting words or sentences.
5. When audio is not available yet, estimate shot durations provisionally and label timing as provisional.

### Stage E — Storyboard coverage
Split the approved narration into manageable visual beats. One beat should convey one main visual idea or one connected action. Every word of narration must be covered by at least one assigned beat unless the producer explicitly documents a deliberate pause, title card, or other reason.

Every beat must specify:
- Shot ID and section.
- Exact narration phrase (verbatim).
- Purpose of the image in the story.
- Claim/evidence IDs, where applicable.
- Visual mode: historical human action, food/object close-up, environment, map/diagram, archival-style collage, or a purposeful modern silent investigator beat.
- Main subject and scale.
- Physical action and start/end state.
- Time/place-specific environment, props, clothing, materials, and light.
- Continuity and anachronism risks.
- Intended shot duration and transition.

Avoid using Alex or Lia in every scene. Use them only where they help investigate, compare evidence, or guide the audience. They are modern channel characters and must not be inserted into historical scenes as though they were actual witnesses.

### Stage F — Produce two prompts per beat
For EVERY storyboard beat, deliver all of the following in the response:
1. Shot number/title.
2. **Exact narration segment**, quoted verbatim.
3. **IMAGE PROMPT** in its own copy-ready code block.
4. **VIDEO PROMPT** in a separate copy-ready code block.

The image prompt must stand alone and be detailed enough to generate the still without needing the reader to reconstruct context from earlier prompts. Include aspect ratio, style, subject, composition, action/pose, background, lighting/palette, historically correct details, restrictions and exclusions.

The video prompt must stand alone and use the still/reference image as a visual guide when relevant. It must specify:
- Total shot duration.
- A timed action plan (e.g., 0–2s, 2–4s, 4–6s).
- Visible physical actions with cause-and-effect and changes to objects/subjects.
- Body/hand movement, object interaction, environmental movement, and meaningful motion.
- Camera framing and movement, with action as the priority.
- ASMR/natural ambience matched to visible events.
- Explicit audio restrictions.
- Historical, character, and style continuity requirements.

Do not describe a video by camera movement alone. There must be visible action. Avoid generic loops, repeated gestures, and identical compositions across consecutive shots. Change the subject scale, angle, movement, visual mode, or story function between adjacent beats when useful.

Do not collapse image and video prompts into one code block. Do not omit narration text. Do not write “same as the previous prompt”; each prompt is self-contained and copy-ready.

### Stage G — Character-reference protocol
If Alex or Lia appears in a shot:
- Explicitly label **Actor 1: Alex** and/or **Actor 2: Lia**.
- Tell the model to use the attached official character sheet as the mandatory primary visual reference.
- Include that character's complete relevant master description from `CHARACTER_BIBLE.md` in both the image and video prompts. Avoid a short name-only reference.
- Repeat identity and proportion consistency rules in every applicable prompt.
- Preserve the character's design and outfit unless the historical period/scene explicitly requires a costume adjustment; any adjustment must retain the core identity.
- Treat them as silent visual investigators: curious, observant, expressive, and purposeful.
- Never request lip-sync, spoken acting, dialogue, or narration from Alex or Lia. Their mouths may show silent expressions only, without implying speech.
- Never fabricate attached image access. If the reference images are not attached or available in the working context, explicitly state that the official reference image is needed and avoid pretending it was used.

Full specifications are in `CHARACTER_BIBLE.md`.

### Stage H — Image and video visual standards
- Aspect ratio: 16:9 landscape unless the user explicitly requests another format.
- The principal subject/action must be large, clear, and readable at typical viewing size.
- Wide city, canal, battlefield, market or landscape shots must still fill the frame with meaningful, legible activity. Avoid scenes with tiny people and empty space dominating the composition.
- Use close-ups when a key ingredient, tool, inscription, hand action, or expression matters.
- Include only objects appropriate to the exact date, region, and culture. Watch for modern produce varieties, materials, cookware, architecture, farming equipment, lighting, transport, textiles, and tools.
- Use credible historical visual references where details matter.
- Distinguish documented objects from plausible reconstruction.
- Do not treat a speculative recipe or scene as a photographed historical fact.
- Default Biteback style: collage-textured 2D stickman character language, expressive faces, irregular dark ink outlines, watercolor/colored-pencil texture, aged paper, earth palette of ochre, terracotta/rust, olive, warm ivory and charcoal. Historical food/architecture can be detailed but should live in the same illustrated world.
- Avoid unintended photorealism, glossy 3D, anime, generic vector explainer style, contemporary cartoon redesigns, and random style changes.
- Do not rely on AI-generated text for historically important labels. Use editor-added text when legibility matters.

### Stage I — Video and sound prompts: mandatory audio policy
Generated shot prompts must specify **ASMR and natural ambience only**, synchronized to visible actions.

Every video prompt must explicitly include all of the following:
- “ASMR and natural ambience only, synchronized to the visible action.”
- “No narrator, no voice-over, no dialogue, no speech, no lip-sync, no music.”

Do not request a narrator, spoken narration, character dialogue, lyrics, musical score, or lip movement implying speech. The narration is placed separately in the edit. Do not include lines of speech or voice-over in video prompts even if the historical scene includes people.

Sounds must be motivated by the image/action: grinding, chopping, footsteps, fabric movement, water, fire crackle, pottery contact, tools, wind, crowd texture without intelligible speech, animal/environment sounds where historically appropriate. Avoid unsupported or anachronistic sounds. Sound design should not introduce a modern object absent from the image.

### Stage J — Production batches and review
1. Generate prompts in chapter-sized batches when the script is long, without losing shot coverage.
2. Maintain sequential shot IDs across batches.
3. Check the first few generated images/videos before scaling production.
4. Correct issues systematically: subject too small, weak action, poor historical details, character drift, repeated framing, missing ASMR, prohibited audio, or prompt omissions.
5. Never start the next block if the user specifically asks to fix an earlier batch first.
6. Keep track of approved, generated, rejected, and regenerated shots.

### Stage K — Final quality control
Before declaring prompts/episode ready, run `QA_CHECKLIST.md`. Confirm:
- Full script approved and matches narration cues.
- Every cue has both image and video prompt.
- Every prompt is complete and copy-ready.
- Physical motion is specified with timing/cause-and-effect.
- Every video prompt carries required audio exclusions.
- Every character appearance includes full reference protocol.
- All historically risky details are sourced or qualified.
- Composition and framing are legible.
- Adjacent shots do not feel like repetitive variants of the same image.
- Final runtime and shot durations are aligned with the narration.
- Visuals do not assert anything the script/evidence does not support.

## 3. Required response format for shot production

### Shot NN — Short purpose title
**Narration**
> [exact approved phrase, verbatim]

**IMAGE PROMPT**
```text
[Standalone image prompt; detailed, self-contained, 16:9; mandatory character boilerplate if applicable.]
```

**VIDEO PROMPT**
```text
[Standalone video prompt; timed physical actions; action-led; ASMR only; explicit audio exclusions; mandatory character boilerplate if applicable.]
```

Use this format for every shot. Do not replace the complete prompts with summaries, abbreviated placeholders, or a table.

## 4. Topic-specific adaptation
The permanent workflow stays stable, but episode details vary. Do not apply one historical episode's ingredients, character wardrobe, location, or terminology to another. Build each episode's evidence ledger and visual restrictions anew. If the user requests an intentional departure, follow the request for that episode while keeping permanent rules intact unless the user explicitly asks to change the playbook.

## 5. Playbook updates and precedence
This repository is the channel workflow source of truth. The companion private plugin reinforces it in ChatGPT. Neither workflow should be claimed to automatically monitor, self-update, or guarantee behavior across systems.

Only the channel owner can authorize permanent workflow changes. For each authorized update:
1. Preserve previous decisions unless they conflict with the explicit change.
2. Update relevant documents and templates.
3. Bump version using semantic intent (major = foundational change; minor = significant workflow additions; patch = clarifications).
4. Update the changelog with date, version, change, and rationale.
5. Ensure repository instructions and companion plugin remain aligned.

If any older note conflicts with this version, follow the latest explicitly approved playbook revision. If an episode-specific request conflicts with a permanent rule, treat it as a one-episode exception unless the user clearly says the rule itself should change.
