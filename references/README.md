# Sticker Studio Reference Pack

This directory defines how reference material is organized and used.

## Reference categories

| Category | Purpose | Can override character identity? |
|---|---|---|
| `character/` | Approved model sheets and identity notes | Yes — this is the identity source |
| `style/` | Linework, texture, palette, and rendering examples | No |
| `motion/` | Approved GIFs / keyframe examples showing motion quality | No |
| `layout/` | Contact-sheet and crop-layout examples | No |
| `prompts/` | Reusable generation and animation prompt templates | No |

## Current reference baseline

The current child-character series has a user-approved hand-drawn crayon / pencil style and an approved character prototype. The accepted motion examples demonstrate:
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

## Reference manifest

Use [reference-manifest.example.yml](reference-manifest.example.yml) to record provenance, approval, intended usage, and privacy scope.
