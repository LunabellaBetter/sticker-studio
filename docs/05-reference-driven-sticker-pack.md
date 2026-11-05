# 05 · Reference-Driven Sticker-Pack Workflow

**Purpose:** Turn user-supplied character references and a confirmed expression list into a consistent, usable sticker pack.

## 1. Reference roles

- Reference A — character identity: user's photo, pet photo, illustration, avatar, or existing character. This determines who the character is.
- Reference B — visual style (optional): a Notion style card or image guiding linework, texture, palette, and rendering. It must not replace identity from Reference A.
- Reference C — layout (optional): a 4×4 / 3×4 / other sticker-sheet layout. It controls the review arrangement only; it must not change the character.

If the user provides only one image, do not invent extra reference requirements.

## 2. Workflow

### Stage 1 — Read the reference
Identify the intended subject and visible identity anchors. If several people appear, establish which one is the sticker subject only when unclear.

### Stage 2 — Create one character lock sheet
Create one coherent illustrated character based on the supplied reference. Include a neutral view and a small range of expressions to test identity stability.

### Stage 3 — User approval
Ask whether this single proposed character matches the reference. Revise it until approved. Do not ask the user to compare three unrelated concepts.

### Stage 4 — Confirm sticker content
Translate the user's phrases / situations into exact caption, intended meaning, emotion and intensity, face and body language, and static or animated treatment. For a large batch, prepare a compact list for approval. Clarify only genuinely ambiguous meanings.

### Stage 5 — Generate the sticker sheet
Use the approved model sheet as the character identity reference. Generate one coordinated sheet with distinct expressions and varied poses. Keep every cell clearly separated and avoid repeated compositions.

### Stage 6 — Split into individual files
The sheet is a contact sheet for review, not the final deliverable. Crop or reconstruct each sticker as an independent transparent-background asset. Check that no neighboring cell, border, or caption is accidentally included.

### Stage 7 — Animate selectively
Choose GIF for expressions where motion adds meaning (nodding, waving, trembling, laughing, sighing). Keep other stickers static when a single pose communicates better. Follow the animation storyboard and QA checklist.

## 3. Adapted multi-sticker prompt template

This template borrows the batch-production structure from Notion S37 / S38 while strengthening identity preservation. It does not impose their rough MS Paint aesthetic.

~~~text
Create a coordinated chat sticker pack using Reference A as the sole source of character identity.

CHARACTER IDENTITY
- Preserve the recognizable face / head silhouette, hairstyle, hair color, distinctive visible features, proportions, and approved outfit language from Reference A.
- Translate the reference into the approved illustration style without changing who the character is.
- Keep the same character design, line quality, palette, rendering, and proportions across every sticker.
- Expressions, poses, gestures, props, and captions may vary; identity anchors must not drift.
- Do not invent a different character, alter the hairstyle between cells, or randomly change clothing.

STICKER CONTENT
- Use the user-confirmed captions and expression briefs below.
- Each cell must express a distinct communicative intent, not merely a different mouth shape.
- Vary facial expression, gaze, posture, gesture, and composition to match each intent.
- Match the language and exact wording supplied by the user.
- Do not add, omit, rewrite, or misspell captions without permission.
- If a caption is intentionally absent, do not add one.

LAYOUT
- Create [N] clearly separated stickers in a [GRID] contact sheet.
- Each cell is an independent composition with enough padding for later cropping.
- Avoid shared body parts, overlapping characters across cell boundaries, panel borders, cell numbers, and decorative clutter.
- Do not force every cell into an identical pose or composition.
- Keep the character's scale and visual identity consistent across the set.

OUTPUT
- The contact sheet is for review.
- Each sticker must also be exportable as a separate transparent-background asset.
- Do not add a background that prevents clean separation.
- Prioritize small-size legibility and recognizable expression.
- Mark uncertain text or visual detail for review instead of silently inventing it.

Reference B may guide visual style only.
Reference C may guide grid layout only.
Neither may override character identity from Reference A.

APPROVED CHARACTER MODEL:
[Attach approved model sheet / character reference]

CONFIRMED STICKER LIST:
[Paste confirmed captions and expression briefs]
~~~

## 4. Style consistency vs. identity consistency

A batch can look stylistically consistent while depicting a slightly different person in every cell. That is insufficient.

Verify:
- same person / character
- same face construction and hairstyle
- same proportions and outfit language
- same illustration language
- distinct, semantically correct expressions

## 5. Delivery structure

Recommended per-pack structure:
- character/ — approved model sheet and identity notes
- source/ — source references and approved prompts
- sheet/ — contact sheet preview
- stickers/png/ — individual static stickers
- stickers/gif/ — individual animated stickers
- storyboards/ — key poses and frame notes
- qa/ — review results and revisions

Keep the contact sheet and individual exports linked by stable sticker IDs.
