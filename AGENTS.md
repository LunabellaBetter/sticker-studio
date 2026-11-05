# Sticker Studio · Working Rules

## Scope
Create general-purpose chat stickers for everyday communication, social interaction, humor, reactions, and emotional expression.

## Scope exclusions
- Do not make the character specific to any employer, industry, job title, or profession.
- Do not add company logos, proprietary slogans, employee data, or internal screenshots.
- Do not assume a default character or default mascot.

## User-reference-first character workflow
- The user may supply personal photos, photos of another person, pets, illustrations, or existing character images.
- Treat the supplied reference as the source of character identity. Extract visible, stable traits and stylize them into one coherent character.
- Do not ask the user to choose among unrelated character concepts when they have supplied a character reference.
- Produce one proposed character model sheet based on the reference and applicable Notion visual rules. Ask the user to approve or correct that proposed identity before batch production.
- If multiple references conflict or it is unclear which subject should be represented, ask one focused clarification.
- Once approved, preserve face silhouette, hairstyle, distinguishing features, proportions, palette, outfit language, and linework. Pose, expression, gesture, props, and caption may change.
- Use the approved model sheet as the identity reference for every sticker and every animation frame.

## Notion multi-sticker prompt reference
- Use Notion Visual Style Library S37 (Chinese 16-cell chat stickers) and S38 (multilingual sticker pack) as workflow references: character reference, optional layout reference, varied expressions, phrase-count handling, and a coordinated sticker sheet.
- Do not inherit their deliberately rough MS Paint style unless the user requests it.
- Strengthen their identity rule: preserve the user's approved character, not merely a consistent drawing style.
- A contact sheet is a review layout. Final deliverables must be individual, independently usable sticker files.

## Expression semantics
Before drawing, establish the intended communicative act, emotion, intensity, social tone, context, desired recipient interpretation, and likely misreading. A phrase can carry multiple meanings; do not infer one meaning from the phrase alone.
For a batch, prepare a compact phrase + intended meaning + proposed visual action list for user confirmation when the request does not already define these clearly. See docs/07-sticker-definition-sheet.md.

## Animation
- Decide whether each sticker needs motion. Do not animate every item by default.
- Design key poses and timing before producing in-between frames.
- Use anticipation, action, follow-through, settle, and a deliberate loop transition where appropriate.
- Preserve character identity across all frames.
- One GIF represents one sticker / one communicative intent. Never combine unrelated stickers in one GIF.
- A GIF must show meaningful facial acting; head or body movement alone is insufficient when the expression itself does not change.
- Body motion must support the intended emotion. Avoid decorative idle wobbling.
- Apply the pass/fail rules in docs/08-gif-approval-rules.md.

## Approval and change control
- Character status: proposed → approved → revised (new version).
- Sticker status: draft → needs-revision → approved → published.
- Do not bulk-produce a series before the character prototype is approved.
- Do not overwrite approved assets silently.
- Keep source artwork, approved model sheet, expression brief, key poses, frame sequence, exports, and review notes traceable.
