# 08 · GIF Approval Rules

**Purpose:** Prevent weak, confusing, or mechanically animated sticker GIFs.

## 1. Core rule

**One GIF = one expression / one communicative intent.**

A single sticker may contain a short setup and payoff, but it must still read as one clear reaction.

Not allowed as final delivery:
- one file cycling through multiple unrelated expressions
- a horizontal strip or contact sheet presented as a GIF deliverable
- several captions appearing in sequence unless the user explicitly requests a sequence sticker
- a weak motion loop that does not deepen the expression

## 2. Semantic requirement

A GIF passes only if it clearly communicates one intended meaning.

Check:
- if the caption is removed, can the viewer still roughly understand the emotion?
- do face and body support the same meaning?
- does motion strengthen the message instead of distracting from it?

If not, fail the GIF.

## 3. Facial-change requirement

A GIF must contain **real expression change**.

At least one of these must visibly change in a meaningful way:
- eyes
- eyebrows
- mouth
- cheeks / blush
- gaze direction

Preferably, two or more dimensions change together.

Fail cases:
- only the head wiggles but the face stays effectively the same
- only the body drifts while the expression is static
- the mouth opens and closes randomly without emotional logic

## 4. Body-action requirement

Body motion must support the intended emotion.

Examples:
- nodding for acknowledgement
- crossed arms and head turn for “哼”
- slight recoil for “what?!”
- shoulder bounce or tucked posture for “嘿嘿”
- drooping posture for sleepy / tired stickers

Fail decorative motion such as idle bobbing, unrelated arm movement, or random bouncing with no semantic role.

## 5. Natural motion requirement

Pass indicators:
- readable start, action, and settle
- sensible motion path
- deliberate acceleration / deceleration
- enough hold time to read the expression
- final frame returns naturally toward the first

Fail indicators:
- sudden snap between frames
- visible jitter
- inconsistent character size or shape
- no readable peak pose
- obvious loop seam

## 6. Single-expression integrity

Allowed:
- one reaction with a short loop
- one reaction with a small setup and payoff
- one stable caption

Not allowed:
- “无语 + 哼 + what?!” in one file
- one GIF behaving like a slideshow of separate stickers
- accidental frame-to-frame text changes

## 7. Text treatment and stability

If text is shown:
- wording must be correct
- text may be absent in opening frames when it is intentionally revealed at the emotional / semantic beat
- after appearing, wording, letterform, size, and placement must remain stable for a readable hold
- text must remain legible at small size
- do not repeat the same phrase as a permanent heading plus a speech bubble / in-scene caption
- placement must not flicker or jump

Fail if text appears before its emotional context, mutates, jitters, is misspelled, redraws inconsistently, repeats redundantly, or remains as a decorative heading that weakens the sticker.

## 8. Pack-level distinctness

Before approving a batch, compare each GIF with the other items in the batch and the previously approved stickers in the same series. Confirm distinct communicative intent, emotion, facial acting, body gesture, motion arc, and chat context. Different captions or props alone do not prove meaningful differentiation. Near-duplicates must be revised, replaced, merged, or explicitly accepted by the user as deliberate variants.

## 9. Technical approval

Recommended:
- transparent background
- one independent sticker per file
- consistent canvas dimensions
- intentional loop metadata
- frame timing matched to the expression

Fail if:
- the file is not actually animated
- expected transparency is missing
- neighboring artwork is accidentally included from a contact-sheet crop
- export is corrupted
- frame canvas changes create a visible jump

## 10. Pass/fail checklist

A GIF is approved only if all are true:
- [ ] one GIF, one expression
- [ ] intended meaning is clear
- [ ] face shows real emotional change
- [ ] body action supports the emotion
- [ ] motion feels natural, not mechanical
- [ ] no obvious loop seam
- [ ] caption is correct, intentionally timed, non-duplicated, and stable after reveal
- [ ] sticker is distinct from the rest of the pack
- [ ] character identity stays consistent across frames
- [ ] file is independently usable

## 11. Common failure reasons

- **Head wobble only:** head moves but eyes, brows, and mouth do not meaningfully change.
- **Multiple expressions in one GIF:** the file scrolls through unrelated reactions.
- **Expression mismatch:** caption says “无语” but face reads as angry or smug.
- **Identity drift:** hairstyle, face, or proportions visibly change between frames.
- **Text mutation:** caption shifts, redraws incorrectly, or changes accidentally.

## 12. Review order

Review in this order:
1. one expression or multiple?
2. intended meaning readable?
3. facial change strong enough?
4. body action supports meaning?
5. loop natural?
6. text stable?
7. export clean?

If a GIF fails at steps 1–4, do not approve it even if the file exports correctly.
