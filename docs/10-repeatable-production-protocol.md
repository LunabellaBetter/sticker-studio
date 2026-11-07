# 10 · Repeatable Sticker Production Protocol

**Purpose:** Turn successful sticker-generation outcomes into a repeatable, inspectable production method without imposing a default character, art style, or output format on future projects.

**Scope:** Generic across people, children, pets, illustrated characters, and original mascots. Project-specific settings become binding only after the user approves them.

## 1. Production stability comes from controlled references

Before each new batch, identify the current approved reference anchors:

1. **Identity anchor:** the approved character model sheet / character lock. This is the source of who the character is.
2. **Style anchor:** one or more approved visual examples that define linework, texture, palette, and rendering.
3. **Motion anchor:** an approved GIF or frame sequence that demonstrates the desired facial acting, body acting, pace, and loop quality.
4. **Composition anchor:** an approved output showing canvas ratio, character scale, crop, safe margins, and caption placement.
5. **Text-treatment anchor:** an approved output showing whether words are absent, static, or revealed at a meaningful moment.

Use the same approved identity anchor throughout the series. Do not let a later generated image silently become the identity source. Style, motion, layout, and text references may guide their own dimensions only; they must not override character identity.

When the user has approved a successful output, record exactly what was approved and reuse it as a reference for the corresponding production dimension. Do not generalize a project-specific character, outfit, or visual style to unrelated projects.

## 2. Lock a project-specific production profile

Before batch production, extract the settings from the user's latest approved sample:

- canvas aspect ratio and export dimensions
- character / face scale and crop
- background and transparency behavior
- visual style and detail density
- caption placement and reveal behavior
- motion pace, peak hold, and loop style
- preferred delivery and preview format

Record the profile in the project brief or reference manifest. Treat it as locked for that character series until the user requests a change.

**Example of a user-approved profile from one child-character series (not a global default):**

- square 512 × 512 px export
- large face / upper-body close-up
- character visually dominant with minimal unused margins and safe edge clearance
- transparent background
- warm hand-drawn pencil / crayon rendering
- unhurried motion with a readable emotional peak
- caption appears only when it contributes to the expression
- mobile-first preview and direct access to each individual GIF

Other projects must derive their own profile from their approved references and target platform. Never impose this example on a new character automatically.

## 3. Run a cross-pack semantic and visual collision check

Before generating a batch, compare every proposed sticker with both the current batch and previously approved stickers in the same series.

Compare at least these dimensions:

| Dimension | Collision question |
|---|---|
| Caption | Is the wording identical or confusingly similar? |
| Communicative act | Do both stickers perform the same social function? |
| Emotion | Are the emotion and intensity effectively the same? |
| Facial acting | Do eyes, brows, mouth, cheeks, and gaze create a distinct reading? |
| Body acting | Are posture and hand gestures meaningfully different? |
| Motion arc | Does the action have a different beginning, peak, and settle? |
| Prop / visual motif | Is the same prop or symbol being reused without a new meaning? |
| Chat context | Would the user send both stickers in the same situation? |

### Collision decision

- **Pass:** the caption, intent, or performance is recognizably distinct.
- **Differentiate:** keep both only after changing the facial acting, gesture, motion, or context enough to make their use distinct.
- **Merge / replace:** if two stickers would communicate the same thing, recommend one stronger version or propose a different phrase.
- **Hold:** if the meaning is unclear, clarify only that item before production.

Do not treat a different caption as proof of a different sticker. Do not treat a different prop as sufficient differentiation when the face and gesture remain the same.

Examples of collision patterns to catch:
- acknowledgement variants such as “嗯嗯”, “收到”, and “我知道了” can collapse into the same nod; define different social intent and performance for each.
- a crying face and a request-for-comfort pose can look alike; distinguish emotional distress from actively asking for a hug through different gaze, tears, arm position, and movement.
- avoid repeating the same caption inside the artwork and again as a permanent heading above the character.

Maintain a simple pack-level index of approved captions, communicative acts, and signature gestures so later batches can be checked before generation.

## 4. Define each sticker before drawing

Complete a compact definition for every item using `docs/07-sticker-definition-sheet.md`.

At minimum, state:

- exact caption, or explicitly no caption
- communicative intent and typical chat context
- emotion and intensity
- intended recipient interpretation
- likely misreading to avoid
- facial acting: eyes, brows, mouth, cheeks, gaze
- body acting: posture, hands, shoulders, head angle
- motion arc and emotional peak
- text reveal beat, if any
- what makes this sticker distinct from the nearest existing sticker

For a batch, prepare and review the whole definition matrix before producing final files. Do not start by asking an image generator to create ten unrelated final stickers in one composite image.

## 5. Treat text as part of the performance

Text must support the expression, not behave like a decorative title.

### Preferred treatment

- Omit text when the face and gesture already communicate the message.
- If text adds a punchline or clarifies intent, reveal it at the meaningful emotional beat.
- Example: a character first smiles, the smile fades, and only then “不嘻嘻” appears.
- Keep the caption in a visually balanced position that does not cover the face or compete with the gesture.
- Once revealed, keep wording, shape, size, and position stable long enough to read.
- Ensure the same phrase is not redundantly repeated in a fixed header, speech bubble, and frame caption.

### Text QA

Check the exact wording, spelling, punctuation, appearance timing, reading duration, placement, and consistency across frames. Reject accidental duplicate text, text mutation, jitter, or an always-visible heading that weakens the composition.

## 6. Build animation as readable emotional acting

Design each GIF as one communicative act. Use only the beats needed:

1. anticipation / initial state
2. emotional or physical trigger
3. primary action and facial transition
4. emotional peak
5. readable hold
6. follow-through and settle
7. natural loop transition

The face must perform the emotion. Change eyes, brows, mouth, cheeks, or gaze in a purposeful way; preferably coordinate multiple features. Body movement must reinforce the meaning.

Keep the pace unhurried enough for mobile chat viewing. The peak expression and any caption need enough hold time to be read. Do not use fast head shaking, idle bobbing, random blinking, or repetitive movement as a substitute for acting.

A nod, for example, should show a clear down-and-up head arc, subtle eye / brow / mouth response, a short readable hold, and a controlled return. A wave should show an intelligible hand lift and wrist / hand action. A comfort-seeking pose should clearly communicate the request through the arms and gaze.

## 7. Generate and assemble one deliverable at a time

Batch planning may happen together, but each final sticker must be produced and checked independently.

- Use the approved identity anchor in every generation or editing step.
- State the exact current sticker name, caption, intent, and required action in each production prompt.
- Explicitly exclude props, captions, and motifs from neighboring stickers when context carry-over is likely.
- If the output repeats a previous theme or caption, stop and correct the input; do not export it under a new filename.
- Approve the key visual / key poses before spending effort on all in-between frames when the action is complex.
- Assemble one independent GIF per expression.
- Contact sheets and spritesheets are intermediate review assets only; split and verify every independent output.

## 8. Composition and transparency checks

Use the project-specific approved production profile and `docs/09-resolution-and-framing.md`.

For every frame:
- canvas width and height are identical
- character scale and anchor point remain stable
- the face and gesture are large enough at actual chat size
- hair, hands, props, and caption stay within safe margins
- transparent pixels remain transparent after GIF palette conversion
- no black / white matte, colored rectangle, or opaque background is introduced unintentionally

Do not fix a small composition by simply enlarging a low-resolution export. Recompose or regenerate from a sufficiently detailed master, then export to the approved target dimensions.

## 9. Actual-file QA and mobile-first delivery

Inspect the exported files, not only the generation preview.

### Per-GIF checks

- file opens in a standard viewer and plays
- frame count is greater than one when labelled GIF
- actual duration and per-frame timing are intentional
- all frames use the approved canvas dimensions
- transparency is verified across the animation, not only the first frame
- caption is correct, non-duplicated, stable, and readable
- character identity and scale remain consistent
- expression is understandable at 240 px and silhouette at 96 px
- at least three consecutive loops are inspected for visible seams
- the GIF contains one expression and one communicative intent

### Delivery format

For mobile-friendly delivery, prioritize:
1. show the actual animated GIF inline when the client supports animation
2. provide a direct link to each individual GIF
3. provide one ZIP for the complete batch
4. provide a contact sheet only as a secondary review aid

Never substitute a static preview, contact sheet, or spritesheet for the individual animated file. If inline animation cannot be rendered in the current client, say so and provide the direct file link.

## 10. Failure handling and approval status

- If identity, theme, caption, or action is wrong, mark `needs-revision` and regenerate / revise only the affected item.
- If the GIF file is corrupt, incorrectly encoded, opaque, or the wrong size, fix the export before visual approval.
- If two stickers collide semantically or visually, revise the definition before redrawing.
- Do not silently accept old captions or motifs carried over from a previous generation.
- Technical export success does not equal visual approval.

Use the statuses in `docs/04-quality-assurance.md`:
- `draft` — not yet reviewed
- `needs-revision` — one or more checks failed
- `approved` — visual and technical checks passed and user approval is recorded
- `published` — packaged for the named target platform

## 11. Stop condition

Stop when every requested item has:
- a distinct approved definition
- an independent export
- verified dimensions and transparency
- readable, natural animation where GIF was requested
- an honest per-item QA status
- mobile-friendly preview and download access

Do not add extra variations merely to increase pack size.


## 12. Batch definition lock

Before generation, lock the exact list of stickers and their intended meanings. Each item needs only:
- exact caption (or no caption)
- intended meaning / chat use
- emotion / tone
- key facial expression and body action
- likely misreading to avoid, if any

If the user already gave clear meanings, infer the remaining production details and do not ask for redundant confirmation. Clarify only materially ambiguous items. If the user is unsure how to express a phrase or how the pack should progress, use targeted web research for suitable public examples, record source links, and propose interpretations for approval. Do not copy distinctive third-party artwork or characters. See `docs/11-expression-reference-research.md`.

Once approved, treat the list as locked. Do not silently add, remove, rename, or reinterpret items during production.

## 13. Preserve the successful recipe

For every series with a user-approved batch, record the actual production recipe:
- generation tool/model and version, when available
- actual identity, style, motion, composition, and text references loaded
- prompt/template version
- production mode (coordinated batch, independent, or hybrid)
- working and export canvas
- transparency handling
- crop, split, compositing, and post-processing steps
- per-item result and user approval

Reuse the last successful recipe for that same character series by default. Do not change model, generation mode, reference set, prompt structure, or post-processing midway through a batch without recording the reason. If a later batch degrades, pause and compare the successful and current recipe before producing more. Change one material variable at a time where practical.

A reference manifest documents intended assets; it does not prove they were actually loaded. Verify the reference files used in the current run.

## 14. Five-point first-pass acceptance

Before detailed GIF review, every final sticker must pass:
1. Character appearance is aesthetically acceptable and consistent with the approved character.
2. Caption is exact, legible, non-overlapping, and not duplicated.
3. Expression and action fit the caption and intended meaning.
4. Canvas is square (1:1) by default, at the approved series dimensions.
5. Background is genuinely transparent in the exported file; for GIF, verify every frame.

Only after these five pass should the item proceed to additional animation, loop, integrity, and platform QA.
