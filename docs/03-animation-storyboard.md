# 03 · Animation and Frame-by-Frame Storyboard

**Core rule:** A four- or five-stage storyboard describes the motion beats. It does not mean the finished GIF should contain only four or five frames.

## 1. Design motion before drawing frames

For each sticker, define:
- starting pose
- primary action
- strongest expression / pose
- follow-through
- settling pose
- loop transition
- total duration
- where the viewer's eye should focus

## 2. Motion beats

Use only the beats needed by the action.

1. **Anticipation** — a small preparation before the main action.
2. **Action** — the main readable movement.
3. **Peak** — the strongest pose or emotional moment.
4. **Follow-through** — hair, sleeves, hands, or body continue slightly after the main action.
5. **Settle** — the pose becomes readable and holds.
6. **Loop transition** — the final pose returns naturally to the opening state.

Some stickers need only a small action and hold. Do not force every sticker into a large movement.

## 3. Natural motion principles

- Use arcs for hands, head turns, and body movement; avoid straight robotic translation where a jointed action is expected.
- Use ease-in and ease-out so movement does not start and stop at constant speed.
- Add slight overshoot only when the emotion supports it.
- Separate primary motion from secondary motion. Hair and sleeves should lag behind the body slightly.
- Let the strongest expression settle long enough to be read.
- Keep the pace unhurried enough for actual mobile chat viewing; do not rush the emotional peak or caption reveal.
- Keep the eyes, mouth, and gesture synchronized.
- Avoid moving every feature in every frame.
- Keep camera framing stable unless a camera move is part of the intended joke or emphasis.

## 4. Example storyboard: wave hello

| Beat | Pose / action | Timing guidance |
|---|---|---|
| 1 · Ready | Arm begins to lift; eyes turn toward viewer | brief anticipation |
| 2 · Lift | Hand reaches beside face | smooth acceleration |
| 3 · Wave A | Wrist turns outward | short action |
| 4 · Wave B | Hand moves back; fingers follow | slight follow-through |
| 5 · Peak | Friendly smile; hand reaches clearest wave pose | short readable hold |
| 6 · Settle | Arm lowers slightly; hair settles | slower deceleration |
| 7 · Loop | Return to opening pose without a visible snap | match position and velocity |

The exported GIF may use 8–12 FPS as an initial test range, with frame count and holds adjusted to the action. This is a starting point, not a universal fixed setting.

## 5. Example timing map

A simple 0.9–1.4 second loop may allocate:
- anticipation: 80–140 ms
- main action: 250–450 ms
- peak hold: 180–300 ms
- settle and return: 250–450 ms

Adjust by expression. A blink, quick shock, gentle nod, and long sigh need different timing.

## 6. Caption as part of the performance

Text is optional. Use it only when it clarifies the communicative intent or adds a punchline. Do not automatically place a permanent title above every character.

When timing matters, reveal the caption at the semantic beat: for example, let a smile disappear first, then reveal “不嘻嘻”. Once visible, keep the exact wording, position, and letterform stable for a readable hold. Do not repeat the same phrase as a top heading, speech bubble, and secondary caption. Avoid text appearing before the expression that gives it meaning.

The caption may be absent in the opening frames. This is intentional, not text instability. After its planned reveal, it must not mutate, jitter, or jump.

## 7. Frame production strategy

Preferred order:
1. approve the static key visual
2. create the opening pose
3. define 3–6 key poses for the action
4. verify character identity in every key pose
5. add in-between frames or use controlled interpolation
6. assemble the loop
7. inspect the animation at actual chat size

Do not rely on a single unconstrained prompt to generate a complete GIF. Independent frame generation can cause facial, hairstyle, clothing, and outline drift. Use the approved master image and consistent pose references as anchors.

For simple actions, a controlled 2D rig or image-layer animation may provide more consistency than regenerating each frame. For complex actions, use more key poses and review transitions individually.

## 8. Loop design

- Match the final frame to the opening frame in position, scale, and silhouette.
- Where possible, match motion direction and velocity at the loop boundary.
- Avoid a long still pause followed by a sudden reset.
- Use a held neutral pose only when it is part of the intended rhythm.
- Preview at least three consecutive loops.

## 9. Technical starting targets

| Parameter | Initial target |
|---|---|
| Canvas | 512 × 512 px working master |
| Background | Transparent |
| Frame rate | Test 8–12 FPS |
| Loop | Seamless |
| Motion | One primary action per sticker |
| Caption | Optional; reveal at a planned beat when useful, then hold exact text and placement steadily |
| Safe area | Keep character and caption away from canvas edge |

Platform-specific dimensions and file-size limits must be checked separately before final export.
