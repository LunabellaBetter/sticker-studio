# 06 · Character Lock Specification

**Purpose:** Turn a user-supplied person, pet, illustration, or existing character into one stable, reusable sticker identity.

## 1. When to use this

Use whenever the user provides a reference that defines who the character is: personal photos, photos of a friend or child, pet photos, an existing illustrated character, an avatar, or a prior sticker image.

Do not invent unrelated mascots or ask the user to choose between concepts when their reference already defines the subject.

## 2. Character lock workflow

### Step 1 — Identify the subject
- If the image contains one clear subject, use that subject.
- If multiple people appear, determine the intended subject from context or ask one focused clarification.
- Do not merge traits from different people unless explicitly requested.

### Step 2 — Extract stable identity cues
Review:
- face / head silhouette
- hairstyle silhouette, hairline, bangs, and parting
- hair color
- eye shape and spacing
- eyebrow shape and emotional range
- nose and mouth construction
- cheek fullness / jawline
- age impression
- head-to-body ratio
- visible accessories
- clothing language and key colors
- characteristic posture or gesture, where relevant

Do not turn temporary details into permanent traits unless the user wants them preserved. Background, lighting color, camera distortion, one-off props, and motion blur are usually not identity anchors.

### Step 3 — Translate into sticker form
Preserve recognizable face construction, hairstyle silhouette, age impression, and useful outfit cues. Simplify details for chat-size readability; unify linework and palette with the approved visual style; clarify silhouette and facial readability; remove decorative clutter that does not help recognition.

## 3. Mandatory character lock sheet

Before batch production, create one proposed character lock sheet.

### A. Identity views
- front view
- three-quarter view
- side view when hairstyle or profile matters
- neutral full-body or three-quarter-body pose

### B. Expression test row
At minimum: neutral, happy, surprised, embarrassed / shy, confused, tired, frustrated / pouty, touched / grateful.

For child-oriented or cute series, optionally add giggle / smug smile, crying, and sleepy.

### C. Gesture test row
At minimum: wave, nod, thumbs-up, hands together, shrug / open palm, and excited hands / clap.

### D. Identity notes
Record character ID, version, source reference(s), fixed attributes, allowed variable attributes, and style reference used.

## 4. Approval checkpoint

Ask:

> 这个人物原型是否符合你提供的参考形象？确认后我会锁定五官、发型、比例、服装语言和画风，再按你确认的表情清单制作。

If changes are requested, revise the same character. Do not branch into unrelated concepts unless explicitly asked.

After approval:
- assign a character ID and version
- save the model sheet as the identity reference
- record fixed identity attributes
- use the same reference in all later sticker batches and animation frames

## 5. Fixed vs. variable attributes

Fixed after approval:
- face construction
- hairstyle silhouette and hair color
- head-to-body ratio
- age impression
- distinctive visible features
- clothing language / signature outfit cues
- line quality and rendering language
- palette family

Variable by sticker:
- facial expression
- pose and hand gesture
- prop
- camera crop
- caption
- animation timing and emotional intensity

## 6. “Looks like the same person” check

Before approving the lock sheet, verify:
- with the caption hidden, does the character still resemble the supplied reference?
- do different expressions still look like the same person?
- at chat size, are hairstyle and face still recognizable?
- are any features drifting between views or expressions?

If not, revise before producing stickers.

## 7. Special guidance for child-based sticker packs

- Preserve softness and age-appropriate proportions.
- Avoid making the child look older or more mature than the reference.
- Keep expressions lively, direct, and readable.
- Simplify clothing while retaining recognizable cues.
- Avoid excessive stylization that erases resemblance.

## 8. Deliverable status

Character states: `proposed`, `approved`, `revised`, `deprecated`.

A sticker pack must not enter bulk production until the character lock sheet is `approved`.
