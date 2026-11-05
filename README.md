# Sticker Studio

A general-purpose, reference-driven system for creating consistent chat sticker packs from user-supplied photos, illustrations, or existing character images.

## Production workflow

1. Receive user references.
2. Extract visible identity cues and create one proposed character model sheet.
3. Ask the user to approve or correct that single proposed character. Do not ask them to choose among unrelated concepts.
4. Confirm the requested sticker phrases and intended meanings.
5. Generate a coordinated sticker sheet using the approved character reference.
6. Split the contact sheet into individual assets; animate only stickers whose meaning benefits from motion.
7. Review identity, semantics, legibility, motion, transparency, and platform constraints.

## Current status

**Foundation draft · 2026-11-05**

- General-purpose; no profession, company, or industry identity is assumed.
- The user's reference determines the character; no default mascot is imposed.
- Notion S37 / S38 provide the multi-sticker batch workflow reference. Their deliberately rough mouse-doodle aesthetic is optional, not mandatory.
- The character model sheet must be approved before batch production.
- No character or sticker pack is currently marked as approved.

## Project documents

- Character identity and approval — docs/01-character-identity.md
- Expression intent specification — docs/02-expression-intent.md
- Animation and frame-by-frame storyboard — docs/03-animation-storyboard.md
- Quality assurance checklist — docs/04-quality-assurance.md
- Reference-driven sticker-pack workflow — docs/05-reference-driven-sticker-pack.md

## Working principle

**The user's reference defines the character. The user's intent defines the expression. The approved model sheet keeps the whole pack consistent.**
