# 02 · Expression Intent Specification

**Purpose:** Translate what the user means into a visual performance that viewers interpret correctly.

A phrase alone is insufficient. The same words can carry different emotions, social intent, and intensity.

## 1. Expression brief

For every sticker, record:
- exact visible phrase, if any
- literal meaning
- communicative act (acknowledge, reassure, thank, refuse, tease, celebrate, comfort, etc.)
- underlying emotion and intensity (1–5)
- social tone (warm, neutral, playful, sarcastic, formal, intimate, awkward)
- context and intended recipient interpretation
- likely misreading to avoid
- facial cues, body language, and motion
- caption treatment

## 2. Example: one phrase, multiple meanings

The phrase “收到” can express:
- warm acknowledgement: soft smile, bright eyes, small nod
- neutral confirmation: calm expression, upright posture, short nod
- reluctant acceptance: uneven smile, shoulder drop, slow nod
- overwhelmed acknowledgement: wide eyes, tense smile, raised shoulders, quick nod

The system should infer from context only when the context is clear. Otherwise clarify the intended nuance, not the whole sticker design.

## 3. Emotion-to-body translation

- Joy: lifted cheeks, open eyes, raised posture, outward gesture.
- Embarrassment: averted gaze, softened shoulders, small hand movement, blush.
- Frustration: compressed brows, tight mouth, restrained or abrupt gesture.
- Surprise: raised brows, widened eyes, brief recoil, then hold.
- Gratitude: softened gaze, slight bow or hands together, gentle follow-through.
- Exhaustion: lowered eyelids, dropped shoulders, delayed movement, longer hold.
- Uncertainty: asymmetrical brows, side glance, slight head tilt, small pause.

These are starting hypotheses. Adjust them to the user's intended tone and approved character.

## 4. Semantic review

Before illustration, check:
1. If the caption is hidden, does the face and gesture communicate the intended emotion?
2. Is the likely interpretation close to the user's intent?
3. Does intensity match the phrase and relationship?
4. Could the pose be misread as sarcastic, dismissive, angry, or flirtatious?
5. Is the expression distinct from other stickers in the set?

## 5. Batch confirmation workflow

When the user requests a sticker pack:
1. Parse the phrases or situations supplied.
2. For each item, write a short intended meaning and proposed visual action.
3. Detect phrases with multiple plausible meanings. Clarify only those ambiguous items.
4. If there are too few phrases for the requested pack size, propose natural additions that match the pack's tone and label them as suggestions.
5. Present a compact phrase + intended meaning + visual action list for confirmation when the batch content is not already explicit.
6. After confirmation, use the approved character model sheet as the identity anchor for every sticker.

Example:
| Phrase | Intended meaning | Proposed visual action |
|---|---|---|
| 收到 | Warm acknowledgement | Smile and one small nod |
| 我真的服了 | Amused disbelief | Half-smile, raised brow, open palm |
| 辛苦了 | Sincere appreciation | Gentle smile and slight bow |

The same phrase may need a different visual action if the user's context or desired tone differs.
