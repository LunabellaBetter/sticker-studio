# 07 · Sticker Definition Sheet

**Purpose:** Convert the user's requested phrase or reaction into a precise, producible sticker brief. A sticker is defined by what the user means, not only by its visible text.

## 1. Required fields

| Field | What to record |
|---|---|
| Sticker ID | Stable internal ID |
| Visible caption | Exact text shown, if any |
| Literal meaning | What the words literally say |
| Intended meaning | What the sender wants to convey |
| Communicative act | acknowledge / tease / comfort / celebrate / refuse / complain / etc. |
| Emotion | Primary emotion |
| Intensity | 1–5 |
| Social tone | warm / neutral / playful / awkward / sarcastic / etc. |
| Typical use context | Chat situation where it is used |
| Desired recipient reading | How the recipient should interpret it |
| Misreading to avoid | Unintended interpretation |
| Facial acting | Eyes / brows / mouth / cheeks / gaze |
| Body acting | Posture / shoulders / hands / head angle |
| Motion idea | Movement that communicates the emotion |
| Props | Optional supporting object |
| Static or GIF | Whether motion adds meaning |
| Notes | Special requirements |

## 2. Choose static PNG or animated GIF

Choose **static** when one pose communicates clearly and motion adds little meaning.

Choose **GIF** when motion adds meaning: nodding, waving, trembling / crying, clapping, sighing, changing facial state, peeking, recoiling, or sleepy drifting.

Do not animate by default.

## 3. Batch confirmation process

1. Parse the user's phrases or situations.
2. Fill one definition row per sticker.
3. Clarify only genuinely ambiguous meanings.
4. If the requested pack needs more items, propose additions and mark them as suggestions.
5. Present a compact phrase + intended meaning + visual action list for confirmation when the request is not already clear.
6. After confirmation, use the approved character model sheet as the identity anchor for every sticker.

## 4. Example definition table

| Sticker ID | Caption | Intended meaning | Emotion | Intensity | Face | Body | Motion idea | Format |
|---|---|---|---|---:|---|---|---|---|
| ST-01 | 无语 | 无奈、懒得多说 | drained annoyance | 2 | half-lidded eyes, flat mouth | chin in hands / small exhale | slow blink + tiny sigh | GIF |
| ST-02 | 哼！ | 傲娇、不服气 | stubborn pout | 3 | eyes closed, pouting mouth | arms crossed, head turned away | small head turn + puff | GIF |
| ST-03 | what?! | 惊讶、没想到 | surprise | 4 | wide eyes, raised brows, open mouth | slight recoil | recoil + hold | GIF |
| ST-04 | 嘿嘿 | 偷笑、得意 | smug delight | 2 | squinting smile | shoulders tucked in | tiny shoulder bounce | GIF |
| ST-05 | 不嘻嘻 | 收起假笑、认真起来 | mood drop | 3 | smile disappears, flat stare | hands on hips / still pose | expression shift | GIF |
| ST-06 | 爱你！ | 亲昵表达 | affection | 3 | smiling eyes, warm smile | heart gesture | form heart + hold | GIF |
| ST-07 | 碎觉觉 | 要去睡了 / 困了 | sleepiness | 1 | droopy eyelids | hug pillow / sway | yawn + drift | GIF |

These are examples, not fixed interpretations. Follow the user's intended nuance and context.

## 5. Semantic quality checks

Before production, verify:
- intended meaning is clear
- ambiguous phrases have been clarified only where necessary
- intensity matches the user's actual use case
- proposed action supports the emotion
- the sticker is distinct from others in the same pack

## 6. Revision handling

Translate feedback into an explicit field update:
- “太夸张了” → lower intensity
- “不是这个意思” → revise intended meaning
- “这个动作不对” → replace body acting / motion idea
- “更像生气，不像无语” → revise facial acting and emotion cues
- “不需要动” → change GIF to static

Do not make unrelated visual changes.

## 7. Compact worksheet

```text
Sticker ID:
Visible caption:
Intended meaning:
Emotion:
Intensity (1–5):
Typical use context:
Misreading to avoid:
Facial acting:
Body acting:
Motion idea:
Prop:
Static or GIF:
Notes:
```
