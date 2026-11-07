# Sticker Studio

A general-purpose, reference-driven production system for creating consistent chat sticker characters and sticker packs from user-supplied photos, pets, illustrations, or existing characters.

**Package status:** Skill and production documentation foundation; reference library structure established.

## Start here

1. Read [SKILL.md](SKILL.md) — the end-to-end production workflow.
2. Read [AGENTS.md](AGENTS.md) — mandatory project rules and privacy requirements.
3. Read the [Reference Pack](references/README.md) — reference roles, provenance, and private asset handling.
4. Follow the numbered production documents under `docs/`.

## Production workflow

1. Receive the user's character references.
2. Extract stable identity cues and create one proposed character model sheet.
3. Ask the user to approve or correct that one prototype.
4. Translate the requested phrases into expression intent, facial acting, body acting, and motion.
5. Confirm the expression list where needed.
6. Produce each sticker as an individual asset.
7. Animate selectively with real facial and body acting.
8. Inspect actual exports and deliver independent PNG / GIF files, preview, manifest, and ZIP.

## Project structure

```text
sticker-studio/
├── AGENTS.md
├── SKILL.md
├── README.md
├── docs/
│   ├── 01-character-identity.md
│   ├── 02-expression-intent.md
│   ├── 03-animation-storyboard.md
│   ├── 04-quality-assurance.md
│   ├── 05-reference-driven-sticker-pack.md
│   ├── 06-character-lock-spec.md
│   ├── 07-sticker-definition-sheet.md
│   ├── 08-gif-approval-rules.md
│   ├── 09-resolution-and-framing.md
│   └── 10-repeatable-production-protocol.md
└── references/
    ├── README.md
    ├── reference-manifest.example.yml
    ├── prompts/
    │   ├── character-model-sheet.md
    │   └── individual-sticker-and-gif.md
    └── private/  # local-only; Git-ignored
```

## Key production rules

- The user's reference determines the character. No default mascot is imposed.
- The character model sheet must be approved before batch production.
- Confirm the exact sticker list and intended meaning before final generation; clarify only consequential ambiguity.
- Reuse the previously successful production recipe for the same character series.
- Every final sticker must pass the five-point contract: approved character appearance, clear/non-overlapping caption, caption-to-expression match, square 1:1 canvas by default, and verified transparent background.
- A phrase must be translated into communicative intent, emotion, facial acting, and body acting.
- One GIF represents one sticker and one communicative intent.
- Head wobbling without meaningful facial change fails GIF QA.
- A contact sheet is a review artifact, never a substitute for individual sticker files.
- Use a high-resolution master and make the character visually dominant; see [Resolution and Framing](docs/09-resolution-and-framing.md).
- Before batch generation, check semantic and visual collisions across the current and previously approved pack; see [Repeatable Production Protocol](docs/10-repeatable-production-protocol.md).
- Treat captions as part of the performance: reveal them at a meaningful beat when useful, and avoid redundant fixed headings.
- Public references require documented provenance and permission. Keep private photos and derivative child likeness assets out of the public repository without guardian permission.

## Production documents

| Document | Responsibility |
|---|---|
| [01 Character Identity](docs/01-character-identity.md) | Reference intake and identity approval |
| [02 Expression Intent](docs/02-expression-intent.md) | Meaning, emotion, intensity, and visual acting |
| [03 Animation Storyboard](docs/03-animation-storyboard.md) | Key poses, timing, motion, and loop |
| [04 Quality Assurance](docs/04-quality-assurance.md) | Semantic, character, temporal, and technical QA |
| [05 Reference-driven Workflow](docs/05-reference-driven-sticker-pack.md) | Batch workflow and generation template |
| [06 Character Lock](docs/06-character-lock-spec.md) | Fixed identity anchors and approval |
| [07 Sticker Definition Sheet](docs/07-sticker-definition-sheet.md) | Per-sticker production brief |
| [08 GIF Approval Rules](docs/08-gif-approval-rules.md) | Explicit GIF pass / fail rules |
| [09 Resolution and Framing](docs/09-resolution-and-framing.md) | Master size, scale, detail, and export |
| [10 Repeatable Production Protocol](docs/10-repeatable-production-protocol.md) | Reference anchors, collision checks, text timing, reproducible production, and mobile delivery |
| [11 Expression Reference Research](docs/11-expression-reference-research.md) | Optional web research for expression ideas and pack progression |

## Reference library

The public repository contains reference organization, prompts, and manifest templates. Private character assets remain in the local ignored `references/private/` folder until public-use permission is confirmed.

See [references/README.md](references/README.md), [visual direction](references/visual-direction-and-accepted-reference-criteria.md), and the [ten-sticker expression example](examples/ten-sticker-pack-expression-brief.md).

## Status and release discipline

- Character: proposed → approved → revised → deprecated
- Sticker: draft → needs-revision → approved → published
- A successful export does not equal QA approval.
- Do not merge unreviewed changes into `main`.


## Batch stability and approval

- Confirm the exact sticker list and intended meaning before final generation; clarify only consequential ambiguity.
- If expression ideas or pack progression are uncertain, use targeted web research for inspiration and record sources; never copy another creator's distinctive artwork.
- Reuse the previously successful production recipe for the same character series. Do not change model, generation mode, references, or post-processing midway through a batch without recording the change.
- Every final sticker must pass the five-point contract: approved character appearance, clear/non-overlapping caption, caption-to-expression match, square 1:1 canvas by default, and verified transparent background.
- Read [Expression Reference Research](docs/11-expression-reference-research.md) when external visual inspiration is useful.
- Approved output references are separate from character identity references. They may guide style, expression, caption treatment, composition, or motion only for the dimensions they demonstrate.
