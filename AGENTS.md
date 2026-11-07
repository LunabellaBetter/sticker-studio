# Sticker Studio · Working Rules

## Mandatory Skill Loading

Before any sticker-related task—including character design, sticker illustration, expression design, animation, GIF production, editing, export, or QA—read the current project rules from this repository.

Required reading:
- `README.md`
- `SKILL.md`
- `AGENTS.md`
- `docs/01-character-identity.md`
- `docs/02-expression-intent.md`
- `docs/03-animation-storyboard.md`
- `docs/04-quality-assurance.md`
- `docs/05-reference-driven-sticker-pack.md`
- `docs/06-character-lock-spec.md`
- `docs/07-sticker-definition-sheet.md`
- `docs/08-gif-approval-rules.md`
- `docs/09-resolution-and-framing.md`
- `docs/10-repeatable-production-protocol.md`
- `docs/11-expression-reference-research.md` when web research is used or expression meaning/progression is uncertain
- `references/reference-manifest.example.yml`
- `references/visual-direction-and-accepted-reference-criteria.md`
- `examples/ten-sticker-pack-expression-brief.md`
- relevant prompt templates under `references/prompts/`

Use the latest version available on the task's designated project branch. If the project branch is not specified, inspect the repository's current working branch and report which revision is being used. Do not silently rely on remembered, copied, or outdated rules.

If any required file cannot be accessed, identify the missing file and pause the affected production step. Do not claim compliance with a document that was not read.

The Skill defines a generic production method. It does not impose a default character, person, outfit, visual style, phrase list, or fixed sticker theme. Determine those from the current user's references, instructions, and approvals for each task.

## Scope

Create general-purpose chat stickers for everyday communication, social interaction, humor, reactions, and emotional expression.

## Scope exclusions

- Do not make the character specific to any employer, industry, job title, or profession unless explicitly requested for a particular task.
- Do not add company logos, proprietary slogans, employee data, or internal screenshots unless explicitly supplied and authorized for that task.
- Do not assume a default character or default mascot.

## User-reference-first character workflow

- The user may supply personal photos, photos of another person, pets, illustrations, or existing character images.
- Treat the supplied reference as the source of character identity. Extract visible, stable traits and stylize them into one coherent character.
- Do not ask the user to choose among unrelated character concepts when they have supplied a character reference.
- Produce one proposed character model sheet based on the supplied reference and applicable visual rules. Ask the user to approve or correct that proposed identity before batch production.
- If multiple references conflict or it is unclear which subject should be represented, ask one focused clarification.
- Once approved, preserve the character's face silhouette, hairstyle, distinguishing features, proportions, palette, outfit language, and linework.
- Use the approved model sheet as the identity reference for every sticker and every animation frame in that character series.
- A newly supplied character reference or a new project may establish a different character. Never carry one task's character identity into another task without the user's instruction.

## Reference handling and privacy

- Separate character identity references, style references, layout references, and approved output references.
- Read `references/README.md` and the reference manifest before using assets.
- Do not publish private source photographs or derivative likeness assets of a private person / child to a public repository without explicit permission from the person or guardian.
- Keep private references under `references/private/`; the directory is Git-ignored.
- Document provenance, permission scope, intended use, and approval status for every public reference.

## Expression semantics

Before drawing, establish the intended communicative act, emotion, intensity, social tone, context, desired recipient interpretation, and likely misreading.
For a batch, prepare a compact phrase + intended meaning + proposed visual action list for confirmation when the request does not already define these clearly. See `docs/07-sticker-definition-sheet.md`.

## Animation

- Decide whether each sticker needs motion. Do not animate every item by default.
- Design key poses and timing before producing in-between frames.
- Use anticipation, action, follow-through, settle, and a deliberate loop transition where appropriate.
- Preserve approved character identity across all frames.
- One GIF represents one sticker / one communicative intent. Never combine unrelated stickers in one GIF.
- A GIF must show meaningful facial acting; head or body movement alone is insufficient when the expression itself does not change.
- Body motion must support the intended emotion. Avoid decorative idle wobbling.
- Treat text as part of the performance: it may appear at a planned emotional beat, then must remain legible and stable; avoid redundant permanent headings or duplicate captions.
- Before a batch, compare captions, communicative acts, emotions, facial acting, gestures, motion arcs, props, and chat contexts against other items in the pack and previously approved stickers. Different wording alone does not prove a distinct sticker.
- Use approved identity, style, motion, composition, and text-treatment references as separate anchors. Do not let later generated outputs silently replace the approved identity source.
- Lock project-specific canvas, character scale, transparency, caption behavior, and pacing from the user's latest approved sample; do not impose one project's settings on another.
- Apply the pass/fail rules in `docs/08-gif-approval-rules.md`.

## Resolution and framing

- Use `docs/09-resolution-and-framing.md` for master canvas, character scale, safe margins, and export.
- Generate / compose at high resolution. Do not solve a small-looking asset through simple upscaling alone.
- Keep the character visually dominant and preserve fine linework at export size.
- Derive exact canvas ratio and dimensions from the approved project profile. A 512 × 512 square, large-face, transparent export is an approved profile for one current series, not a universal default.

## Approval and change control

- Character status: proposed → approved → revised (new version).
- Sticker status: draft → needs-revision → approved → published.
- Do not bulk-produce a series before the character prototype is approved.
- Do not overwrite approved assets silently.
- Keep source artwork, approved model sheet, expression brief, key poses, frame sequence, exports, and review notes traceable.

## Delivery requirements

- One sticker is one independent deliverable.
- Contact sheets and storyboards are review artifacts, not final individual stickers.
- For GIF batches, export one separate GIF per expression unless the user explicitly requests a combined animation.
- Inspect actual exported files: animation, frame timing, dimensions, transparency, text, loop continuity, and identity consistency.
- Report failed checks honestly. Do not describe a file as a GIF if it is static.
- Provide a clear file list, manifest, preview, and ZIP for multi-asset delivery.
- For mobile-first delivery, show the actual animated GIF inline when supported and provide direct links to each individual GIF plus a ZIP. A contact sheet is secondary review material only.


## Batch definition gate

Before producing a new sticker batch, create one compact definition row per requested sticker. At minimum record:
- exact visible caption (or explicitly no caption)
- intended meaning / chat use
- emotion and tone
- key facial expression and body action
- one likely misreading to avoid, when relevant

The user-facing confirmation should stay compact. If the user has already supplied a clear phrase list and intent, infer the straightforward details and proceed; do not ask them to reconfirm the entire list. Ask only about materially ambiguous items. Do not begin final generation while the requested sticker list or a consequential ambiguous meaning remains unresolved.

If the user is unsure how a phrase should be performed or how a pack should progress, use web search to collect suitable public examples and propose a small set of interpretations. Research is optional and targeted, not a mandatory step for every batch. Use examples as inspiration for expression, gesture, tone, and sequence only; do not copy another creator's character, distinctive artwork, composition, or complete sticker. Keep source links and a short note in the batch brief, then obtain user approval for the proposed meanings before production. See `docs/11-expression-reference-research.md`.

## Reproducible batch method

- Preserve the production method, model/tool, approved references, prompt structure, and post-processing recipe that previously produced user-approved results for the same character series.
- Do not switch between contact-sheet, per-sticker, or hybrid generation methods midway through a batch without recording the reason and obtaining approval when the change affects the expected result.
- A contact sheet may be used when it is part of a proven successful workflow, but it remains a review/intermediate asset. Every final sticker must be independently exported and checked.
- When a previously successful batch begins to drift, stop expanding the batch. Compare the last successful recipe with the current run: actual loaded identity/style references, model/tool/version, prompt, generation mode, canvas, transparency handling, and post-processing. Change one material variable at a time where practical.
- Record the successful recipe and its evidence so later batches can reproduce it. Do not assume a Skill file or manifest proves that a reference was actually loaded during generation.

## Five-point delivery contract

Unless the user explicitly requests a different treatment, every final chat sticker must pass all five user-priority checks:
1. **Character appearance:** aesthetically acceptable and consistent with the approved character identity and style.
2. **Caption layout:** exact wording, legible, with no overlap, accidental duplication, or obstruction.
3. **Meaning match:** facial expression, pose, and action clearly fit the caption and intended chat meaning.
4. **Square canvas:** 1:1 output by default; use the approved project-specific pixel dimensions. Do not stretch artwork to force a square.
5. **Transparent background:** verify actual alpha/transparency in the exported file, including every GIF frame.

These five checks are the first approval gate. GIF timing, natural movement, loop continuity, file integrity, and target-platform limits remain additional technical checks when applicable. A generated preview alone does not prove export compliance.
