# 09 · Resolution, Character Scale, and Framing

**Purpose:** Prevent sticker artwork from looking too small, under-detailed, or weak at actual chat size.

## 1. Master canvas vs. delivery canvas

Work at a larger master size. Export to the target platform's supported dimensions only after composition and QA.

| Asset | Working master | Typical export target | Notes |
|---|---:|---:|---|
| Square bust / face reaction | 1024 × 1024 px | 640 × 640 px | Use for facial reactions and hand gestures |
| Full-body portrait sticker | 1024 × 1280 px | 640 × 800 px | Keep shoes, hair, and caption inside safe area |
| Wide action sticker | 1280 × 1024 px | 720 × 576 px | Use only when gesture genuinely needs horizontal space |
| GIF frames | Match the approved master canvas | 512–640 px on the long edge, platform permitting | Keep every frame on the same canvas |

These are production targets, not claims about universal platform limits. Check the target platform's current file-size and dimension rules before final export.

## 2. Character scale

The character must be visually dominant.

Starting targets:
- Full-body character: character silhouette occupies approximately 78–86% of canvas height.
- Bust / upper-body character: head and torso occupy approximately 78–88% of canvas height.
- Face-focused reaction: face occupies approximately 42–58% of canvas height, adjusted for hand gestures and props.
- Leave approximately 5–8% safe margin around hair, hands, shoes, props, and text.

Do not shrink the character to make room for oversized decorative backgrounds. Backgrounds should remain transparent unless the user requests a solid or illustrated background.

## 3. Detail density

Prioritize detail where it improves recognition:
- hair strands and ponytail silhouette
- eyes, brows, mouth, and cheek expression
- collar, buttons, wristband, and signature clothing cues
- hand shape and gesture
- line weight and paper / crayon texture

Avoid micro-detail that disappears at chat size. Keep the outer silhouette strong and internal details clear.

## 4. High-resolution generation and finishing

- Generate or draw the master at 1024 px or larger on the long edge whenever the tool supports it.
- Do not rely on simple interpolation to turn a small image into a detailed large asset.
- If the first generation makes the character too small, revise the composition: tighter crop, larger character, less empty space, and a clear safe margin.
- Preserve the approved character proportions. Do not enlarge only the head or hands in a way that changes the approved identity style.
- Downsample only after linework, text, and transparency have been checked at master size.

## 5. Composition rules

- Use a transparent background for normal chat stickers.
- Keep one clear visual focal point.
- Place captions near the character without competing with the face.
- Do not crop important gestures or facial features.
- Avoid adding colored rectangular backplates unless explicitly requested.
- If a visual effect (question mark, tears, heart, impact marks) is used, it must support the intended meaning and remain separate from the character silhouette where possible.

## 6. GIF canvas consistency

- Every frame in one GIF must use identical width and height.
- Keep character scale and anchor point stable unless intentional movement requires a small shift.
- Do not let the character jump in size between frames.
- Check transparency on all frames, not only the first.
- Keep caption position and size stable.
- For ping-pong loops, inspect the transition at both ends; for cyclic motion, match the first and last pose and motion direction.

## 7. Project-specific approved output profile

Do not assume one canvas or character scale for every project. Extract the production profile from the user's latest approved output and record it before the next batch.

For one user-approved child-character series, the accepted delivery profile is a **512 × 512 px square canvas**, transparent background, large face / upper-body close-up, character filling most of the usable area, minimal unused margins, and sufficient safe clearance for hair, hands, and text. This is a series-specific approved profile, not a universal Sticker Studio default. Apply it to that series until the user changes it; other characters and target platforms must use their own approved profile.

When the user says the sticker looks too small in chat, recompose or regenerate with a tighter crop and larger character / face. Do not merely enlarge a low-resolution export or crop away meaningful gestures.

## 8. Chat-size preview

Review every sticker at:
- master size (detail and defects)
- export size (line quality and crop)
- 240 px preview (expression legibility)
- 96 px preview (silhouette and recognition)

If the expression disappears at 96–240 px, simplify and strengthen the expression before delivery.


## 9. Default chat-sticker output contract

Unless the user explicitly requests another shape or a target platform requires a different profile:
- use a **square 1:1 canvas**
- use a **transparent background**
- keep the character, gesture, props, and caption within the safe area
- do not stretch the artwork to force a square; recompose the layout instead
- use the current character series' approved pixel dimensions rather than assuming one universal export size

For a GIF, every frame must have exactly the same square canvas dimensions. Verify transparency in every frame of the actual exported GIF, not only in the first frame or a preview. A background color shown by an image viewer may be its transparency display; inspect the file's alpha/transparency data before deciding it has an opaque background.

A user-approved reference may have a non-square canvas. It can still guide character appearance, linework, expression, caption treatment, or motion. Do not copy its canvas ratio when the current production profile requires square output.
