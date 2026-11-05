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
- `references/README.md`
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
- Include requested caption text accurately and keep it stable across frames.
- Apply the pass/fail rules in `docs/08-gif-approval-rules.md`.

## Resolution and framing

- Use `docs/09-resolution-and-framing.md` for master canvas, character scale, safe margins, and export.
- Generate / compose at high resolution. Do not solve a small-looking asset through simple upscaling alone.
- Keep the character visually dominant and preserve fine linework at export size.

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
