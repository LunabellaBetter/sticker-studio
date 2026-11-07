# Sticker Studio Reference Pack

This directory defines how reference material is organized and used.

## Reference categories

| Category | Purpose | Can override character identity? |
|---|---|---|
| `character/` | Approved model sheets and identity notes | Yes — this is the identity source |
| `style/` | Linework, texture, palette, and rendering examples | No |
| `motion/` | Approved GIFs / keyframe examples showing motion quality | No |
| `approved-output/` | Complete user-approved sticker outputs; guide only the dimensions they demonstrate | No, unless explicitly approved as identity |
| `layout/` | Contact-sheet and crop-layout examples | No |
| `prompts/` | Reusable generation and animation prompt templates | No |

## Current production learnings

Stable results come from keeping the approved identity, style, motion, composition, and text-treatment references separate and reusing the same approved identity anchor throughout a series. A successful output should be recorded as a reference for the dimension it demonstrates; a generated output must not silently replace the character identity source.

For each project, derive and lock a project-specific profile from the user's latest approved output: canvas, character scale, crop, transparency, caption behavior, pace, and delivery format. One child-character series has an approved 512 × 512 square, large-face, transparent profile. This is not a global default for other characters or projects.

Before batch production, check for repeated captions, communicative intent, facial acting, gestures, motion arcs, and props across both the new batch and previously approved stickers. Treat text as part of the performance; reveal it at the meaningful beat when useful, then keep it stable and avoid redundant fixed headings.

See [Visual Direction and Accepted Reference Criteria](visual-direction-and-accepted-reference-criteria.md), [Resolution and Framing](../docs/09-resolution-and-framing.md), and [Repeatable Production Protocol](../docs/10-repeatable-production-protocol.md).

## Current reference baseline

The current child-character series has a user-approved hand-drawn style and an approved character prototype. Accepted motion examples demonstrate:
- readable facial acting, not head wobbling
- a clear action and emotional peak
- body gestures that reinforce the expression
- one sticker per GIF
- a calm, readable hold and a deliberate loop

The child-derived model sheet and GIF examples are treated as **private project references**. They are intentionally excluded from this public repository until explicit guardian permission for public distribution is confirmed.

## Private reference storage

Place private assets locally under:

```text
references/private/
├── character/
│   ├── approved-model-sheet.png
│   └── character-lock.md
├── motion/
│   ├── approved-speechless.gif
│   └── approved-thumbs-up.gif
└── manifest.yml
```

This directory is ignored by Git. Do not force-add its contents.

## Public contribution requirements

A reference may be added to the public repository only when:
1. the asset is generic or the owner / subject / guardian has explicitly authorized public use
2. its source and creator are documented
3. its license / permission scope is recorded
4. it does not contain private photographs, personal information, or an identifiable child likeness without permission
5. it has a clear role: identity, style, motion, or layout

## Prompt templates

- [Character model sheet](prompts/character-model-sheet.md)
- [Individual sticker and GIF](prompts/individual-sticker-and-gif.md)

## Example expression brief

See [Ten-sticker expression brief](../examples/ten-sticker-pack-expression-brief.md) for a reusable example of phrase-to-expression mapping.

## Reference manifest

Use [reference-manifest.example.yml](reference-manifest.example.yml) to record provenance, approval, intended usage, and privacy scope.


## Approved output references

Use `approved-output/` for complete sticker images or GIFs that the user has explicitly approved and authorized for the intended repository visibility.

Each approved output pack must include a small manifest recording:
- series / character scope
- source and permission basis
- original filename and repository path
- dimensions, frame count, and transparency status when verified
- which dimensions the output may guide: character identity, style, expression, motion, composition, or text treatment
- restrictions on reuse

Do not assume every approved output is an identity reference. A reference from another character series may guide only the visual dimensions it demonstrates. It must never overwrite or merge with the current series' approved character identity.

The user-provided ten-sticker office-girl pack is a separate approved-output reference series. It may guide aesthetic quality, hand-drawn rendering, expression-to-caption matching, speech-bubble treatment, and motion examples. It is not the identity source for the separate child-character series.

See `approved-output/office-girl-pack-v1/README.md` and its manifest.
