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

## 7. Chat-size preview

Review every sticker at:
- master size (detail and defects)
- export size (line quality and crop)
- 240 px preview (expression legibility)
- 96 px preview (silhouette and recognition)

If the expression disappears at 96–240 px, simplify and strengthen the expression before delivery.
