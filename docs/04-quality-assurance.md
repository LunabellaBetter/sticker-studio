# 04 · Quality Assurance

A GIF is approved only when it passes semantic, visual, temporal, and technical review.

## A. Semantic QA
- [ ] The intended meaning is written down before production.
- [ ] The image communicates the intended emotion without relying entirely on the caption.
- [ ] Intensity matches the user's intent.
- [ ] No likely unintended reading (sarcasm, anger, dismissal, flirtation, etc.).
- [ ] Caption and body language reinforce each other.

## B. Character QA
- [ ] Same face construction as the approved master.
- [ ] Same hairstyle silhouette and color.
- [ ] Same head/body ratio.
- [ ] Same outfit language and palette.
- [ ] Same line weight and rendering style.
- [ ] Hands, eyes, mouth, and props remain anatomically coherent.

## C. Temporal QA
- [ ] Anticipation is present when the action needs it.
- [ ] Motion follows a readable path.
- [ ] Acceleration and deceleration feel intentional.
- [ ] Secondary motion is subtle and delayed appropriately.
- [ ] Peak expression has enough reading time.
- [ ] No jitter, flicker, shape mutation, or accidental frame jump.
- [ ] At least three consecutive loops have no visible seam.

## D. Small-size QA
- [ ] Meaning remains legible at 240 px.
- [ ] Silhouette remains recognizable at 96 px.
- [ ] Caption remains readable at actual chat size.
- [ ] Important details are not lost against transparent backgrounds.

## E. Technical QA
- [ ] GIF opens in standard viewers.
- [ ] Transparent background behaves correctly.
- [ ] Frame timing and loop metadata are intentional.
- [ ] Canvas dimensions are consistent across the set.
- [ ] File size is within the target platform's current limit.
- [ ] Filename, source, key poses, and export are catalogued.

## Approval states

- draft — concept or visual under review
- needs-revision — failed one or more QA dimensions
- approved — user-approved character / expression / animation
- published — exported and packaged for a target platform

Never mark a draft as approved merely because the file exports successfully.
