---
name: sticker-studio
description: Create consistent, reference-driven chat sticker characters and sticker packs from user-supplied photos, pets, illustrations, or existing characters. Covers character prototype approval, expression semantics, individual sticker illustration, frame-by-frame GIF production, QA, and delivery.
---

# Sticker Studio Skill

Use this skill for any request involving sticker character creation, sticker packs, expression design, animation, GIF export, or sticker asset QA.

## Mandatory startup

Before production, read the current project version of:
- `README.md`
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

Use the task's designated branch. If no branch is named, inspect the current branch and report the exact revision used. Never assume a remembered version is current. If a required document is unavailable, pause the affected production step and identify the missing item.

## Core operating principle

The user's reference defines **who the character is**. The user's intent defines **what the sticker communicates**. The approved character model keeps the complete series consistent.

Do not invent a default mascot. Do not ask the user to choose between unrelated characters when their supplied reference already identifies the subject.

## Production workflow

### 1. Intake and reference separation
Classify supplied materials:
- Character identity reference — determines the person / pet / character.
- Style reference — determines linework, texture, palette, and rendering only.
- Layout reference — determines contact-sheet arrangement only.
- Approved output reference — demonstrates an already accepted expression or motion treatment.

Never let a style or layout reference overwrite the approved character identity.

### 2. Build one character prototype
Extract face shape, hairstyle, hairline, eye and brow shape, mouth construction, age impression, proportions, outfit cues, accessories, and distinguishing features.

Create one proposed model sheet. Include front and three-quarter views, a neutral pose, and an expression range that tests whether the same character remains recognizable. Ask the user to approve or correct this one prototype.

Do not begin bulk production until the user approves it. Once approved, lock identity anchors and reuse the same master reference for every sticker and animation frame.

### 3. Understand the requested expressions
For each phrase or situation, define:
- exact caption
- intended communicative act
- emotion and intensity
- social tone and likely chat context
- desired recipient interpretation
- misreading to avoid
- facial acting
- body acting
- prop, if useful
- static or GIF decision

Clarify only genuinely ambiguous meanings. If the user has already explained the intent, do not ask them to reconfirm it.

### 4. Design each sticker as an individual asset
One sticker is one independent composition and one deliverable file.

A contact sheet may be used for batch review only. It is never a substitute for individual PNG / GIF exports.

For each item:
1. define one expression and one communicative intent
2. create a strong key visual
3. confirm composition, character scale, caption, and gesture
4. animate only if movement adds meaning
5. export and inspect the individual file

### 5. Animate with real acting
Plan anticipation, action, peak expression, follow-through, settle, and loop transition. Use only the beats required by the action.

A GIF must show meaningful facial acting. Eyes, brows, mouth, cheeks, or gaze must change in a way that communicates the emotion. Body motion must reinforce that meaning. Head wobbling or idle bobbing alone fails QA.

One GIF = one expression / one communicative intent. Do not combine unrelated stickers into a single GIF.

### 6. Apply high-resolution composition
Use `docs/09-resolution-and-framing.md` for working canvas, character scale, face scale, safe margins, text, and export rules.

Do not solve a small-looking sticker by merely enlarging a low-resolution export. Generate / compose at a sufficiently large master size, make the character occupy the intended visual area, preserve line detail, then export to the target platform's supported dimensions.

### 7. Stabilize batch production

Before producing a batch, lock the approved identity, style, motion, composition, and text-treatment references as separate anchors. Derive a project-specific production profile from the latest user-approved output; do not impose one character or output specification on other projects. Compare captions, communicative intent, emotion, facial acting, body gesture, motion arc, props, and chat context across the current and prior approved pack. Different wording alone does not make two stickers distinct. Revise, replace, or remove collisions before generation. Treat captions as part of the acting: reveal text at a meaningful beat when useful, then hold it stable; avoid permanent duplicate headings. Produce and inspect each final sticker independently. Follow `docs/10-repeatable-production-protocol.md` for the full repeatable method.

### 8. Inspect and approve
Inspect actual exported files, not only previews. Verify:
- one expression per file
- semantic accuracy
- character identity across frames
- face and body movement
- timing and loop continuity
- text accuracy and stability
- transparent background
- canvas dimensions and file integrity
- readability at actual chat size

Mark each item as draft, needs-revision, approved, or published. Never claim a file passed checks that were not performed.

## Reference library

Read `references/README.md` and `references/reference-manifest.example.yml` before using any reference pack.

The public repository must not contain identifiable source photographs or derivative likeness assets of a private person / child without explicit permission from the person or their guardian. Keep such files in the ignored local `references/private/` directory. Public reference examples should be generic, licensed, and provenance-documented.

## Delivery

For a batch, provide:
- inline animated previews when the client supports them
- direct links to each individual GIF
- individual transparent PNGs where applicable
- one independent GIF per animated expression
- a contact-sheet preview clearly marked as preview
- a ZIP archive
- a manifest with filenames, dimensions, frame counts, duration, and QA status
- a per-item QA result

Do not label a static image as a GIF. Do not mark a pack approved until each file has been inspected.

## Change control

Preserve the approved character and visual direction. Apply feedback only to the affected expression or production parameter unless the user requests a wider redesign. Keep source, key poses, exports, and QA notes traceable.


## Batch definition and approval gate

Before final generation, prepare a compact definition for every requested sticker: exact caption, intended meaning/use, emotion/tone, key face/body action, and any misreading to avoid. If the user's list and meaning are already clear, fill the details from context and proceed without unnecessary reconfirmation. Ask one focused question only for a materially ambiguous phrase. Do not start final production while the list or a consequential ambiguity is unresolved.

When the user is unsure how an expression should look or how the pack should progress, use targeted web research to find suitable public examples and propose interpretations. This is optional and only used when it adds value. Borrow general expression ideas, gesture logic, emotional progression, or chat-use patterns; do not copy another creator's character, distinctive artwork, or complete composition. Record useful source links in the batch brief and let the user approve the interpretation. Read `docs/11-expression-reference-research.md`.

## Reuse successful production recipes

For a character series with previously approved batch results, reuse the same verified production method, model/tool, identity anchor, style/output references, prompt structure, and post-processing path. A previous successful batch is evidence to preserve, not a reason to redesign the process. Do not switch generation modes midway through a batch without recording why. If quality drifts, pause and compare the successful and current run before continuing.

The Skill and manifest do not prove that an image reference was actually loaded. Verify the actual reference files used in the current generation step. Record the method and reference IDs for each batch.

## Five-point final delivery contract

Every final sticker must pass these user-priority checks:
1. Character appearance is aesthetically acceptable and matches the approved character identity/style.
2. Caption wording is exact, legible, and does not overlap, duplicate, or obstruct the character.
3. Facial expression and body action match the caption and intended meaning.
4. Canvas is square (1:1) by default, using the approved project-specific pixel size; never distort artwork to force the ratio.
5. Background is genuinely transparent in the exported file; for GIF, verify transparency across all frames.

These five checks are the first approval gate. GIF timing, natural movement, loop continuity, file integrity, and platform limits remain additional checks for animated deliverables.
