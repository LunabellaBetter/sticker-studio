# 07 · Sticker Definition Sheet

**Purpose:** Confirm what each sticker communicates before production, without making the user complete an unnecessarily long questionnaire.

## 1. Minimum definition required for every sticker

| Field | Requirement |
|---|---|
| Sticker ID | Stable internal ID |
| Exact caption | Exact visible text, or explicitly no caption |
| Intended meaning | What the sender wants to convey |
| Emotion / tone | Main emotion and social tone |
| Face / action | Key facial expression and body gesture |
| Misreading to avoid | Record only when a plausible ambiguity exists |
| Format | Static PNG or GIF, when known; infer when obvious |

The production system may derive intensity, gaze, pose details, timing, props, and other implementation details. Do not make the user fill these unless they materially affect the result.

## 2. Batch definition gate

Before producing a batch:

1. Parse the user's requested phrases or situations.
2. Create one compact row for each sticker using the minimum fields above.
3. Check whether the pack has distinct chat uses and whether any items are near-duplicates.
4. If a phrase has multiple materially different meanings, clarify that phrase only.
5. If the user is unsure what an expression should look like or how the pack should progress, use targeted web research and propose a concise interpretation.
6. Present the compact list for approval only when the meaning/action has been inferred or proposed in a way that could materially change the result.
7. After approval, lock the list for production. Do not silently add, remove, rename, or reinterpret items.

If the user already supplied a clear list and intended meaning, do not ask them to repeat or reconfirm it.

## 3. Expression progression

A pack should have useful coverage and visual variety. Consider:
- different communication functions (acknowledge, react, request, reassure, thank, celebrate, refuse, tease, etc.)
- different emotional tones and intensities
- different facial acting and gestures
- common situations in which the user would send the sticker

A narrative progression is optional. Do not force every pack into a story. Use web research only when the user is unsure or when suitable examples would materially improve the proposal.

## 4. Web research as inspiration

When needed, search public examples for the phrase, emotion, chat context, gesture, or expression sequence. Prefer sources with clear authorship and relevant visual examples. Record the source link and what general idea is being borrowed.

Use research to understand common visual conventions, gesture choices, emotional intensity, and pack coverage. Do not reproduce another creator's character, distinctive artwork, exact composition, or a complete sticker. The user's approved character and style references remain authoritative.

See `docs/11-expression-reference-research.md`.

## 5. Internal production brief

After the user-facing definition is confirmed, the production brief may expand each item with:
- communicative act and typical chat context
- intensity (1–5)
- intended recipient reading
- detailed eyes / brows / mouth / cheeks / gaze
- posture / shoulders / hands / head angle
- props
- motion arc and emotional peak
- caption reveal beat
- distinctness from the nearest approved sticker

These are production details. Keep the user-facing confirmation compact.

## 6. Compact worksheet

```text
Sticker ID:
Exact caption:
Intended meaning / chat use:
Emotion / tone:
Key facial expression:
Key body action:
Misreading to avoid (if any):
Static or GIF (if known):
```

## 7. Revision handling

Translate feedback into a specific field update:
- “太夸张了” → lower emotion intensity
- “不是这个意思” → revise intended meaning
- “这个动作不对” → replace facial/body acting or motion
- “更像生气，不像无语” → revise emotion cues
- “不需要动” → change GIF to static

Do not make unrelated visual changes.
