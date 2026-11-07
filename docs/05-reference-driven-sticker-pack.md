# 05 · Reference-Driven Sticker-Pack Workflow

**Purpose:** Produce a coherent sticker pack while preserving an approved character identity, a confirmed expression list, and a reproducible production method.

## 1. Reference roles

Keep reference roles separate:

- **Character identity:** approved model sheet / character lock. Defines who the character is.
- **Style:** linework, texture, palette, and rendering.
- **Motion:** approved GIFs or key poses demonstrating facial/body acting and pace.
- **Composition:** canvas ratio, character scale, crop, margins, and layout.
- **Text treatment:** caption shape, placement, typography, and reveal behavior.
- **Approved output:** a complete user-approved sticker demonstrating several of the above dimensions. Record exactly which dimensions it is approved to guide.

An approved output from another character series may guide style, composition, text, expression, or motion only. It must never replace the current character's identity anchor.

## 2. Mandatory pre-production gates

### Gate A — Character lock
Use the current series' approved character model sheet as the identity anchor. Confirm that the actual image reference is available and loaded in the generation/editing step. A manifest entry or written description alone is not proof of loading.

### Gate B — Batch definition
Before final generation, prepare one compact row per sticker:

| Required item | Record |
|---|---|
| Exact caption | The exact words, punctuation, or “no caption” |
| Intended meaning | What the sender wants to communicate |
| Emotion / tone | The primary emotion and social tone |
| Face / action | The key facial expression and body gesture |
| Misreading to avoid | Only when a plausible wrong reading exists |

If the user already supplied a clear list and intent, complete the rows from context and proceed. Do not ask for redundant confirmation. Ask only about consequential ambiguity. Do not generate final assets until the list is clear and the user has approved any proposed interpretation that materially changes the meaning.

### Gate C — Expression progression and research
A pack should cover distinct, useful chat situations and avoid near-duplicates. A forced story arc is not required. If the user is unsure how a phrase should be expressed or how the pack should progress, use targeted web research to find suitable public examples and propose a concise set of options. Record sources and borrow general acting/gesture ideas only; do not copy distinctive artwork or another creator's character. See `docs/11-expression-reference-research.md`.

## 3. Choose and lock the production method

There is no single mandatory generation mode for every tool or series. Select from:

1. **Coordinated batch generation:** use when this method has already produced approved results for the same series and the generator can preserve identity and separation reliably.
2. **Independent sticker generation:** use when individual expressions require more control, when the generator drifts in a batch, or when complex captions/actions need separate handling.
3. **Hybrid production:** plan the whole pack together, generate a coordinated base or contact sheet where useful, then reconstruct/finish each item independently.

**Reproducibility rule:** For a series with a previously successful method, reuse that method and its model/tool, references, prompt structure, and post-processing recipe by default. Do not switch methods midway through a batch without recording the reason. If a drift appears, pause and compare the last successful run with the current run before continuing.

A contact sheet is always an intermediate review artifact. It is never the final independent sticker deliverable.

## 4. Production and export

- Use the same approved identity anchor for every item.
- Keep the batch-level style, composition, caption treatment, and export profile consistent.
- Each item must have one clear communicative intent.
- Each final sticker must be independently exported as its own PNG or GIF.
- For GIFs, preserve the same canvas size and character anchor across all frames.
- Keep exact caption wording; do not add, remove, duplicate, or rewrite text without permission.
- Do not silently carry props, captions, or visual motifs from a neighboring sticker into the current one.

## 5. Five-point user-priority QA

Every final sticker must pass all five checks:

1. **Character appearance:** aesthetically acceptable and consistent with the approved character identity/style.
2. **Caption layout:** exact, readable wording; no overlap, accidental duplication, or obstruction.
3. **Meaning match:** expression, gaze, pose, and action fit the caption and intended meaning.
4. **Square canvas:** 1:1 by default, using the approved project-specific pixel dimensions. Never stretch artwork to force a square.
5. **Transparent background:** verify actual transparency in the exported file; for GIF, inspect every frame after palette conversion.

These are the first approval gate. A failure in any one means `needs-revision`.

## 6. Additional GIF and file QA

For animated outputs, also verify:
- one GIF = one sticker = one communicative intent
- meaningful facial change; body motion supports the emotion
- natural timing, readable peak hold, and deliberate loop
- no jitter, flicker, shape mutation, or frame-to-frame identity drift
- the GIF opens and plays in a standard viewer
- all frames use identical canvas dimensions
- file size and format meet the named platform's current requirements

Inspect the actual exported file, not only the generation preview.

## 7. Delivery structure

Recommended per-pack structure:
- `character/` — approved model sheet and identity notes
- `source/` — source references and approved prompts
- `sheet/` — contact sheet preview, clearly marked as preview
- `stickers/png/` — individual static stickers
- `stickers/gif/` — individual animated stickers
- `storyboards/` — key poses and frame notes
- `qa/` — per-item checks and revision notes

Keep the contact sheet and individual exports linked by stable sticker IDs.


## 8. Batch prompt skeleton

Use the current series' approved identity reference and the confirmed batch definition. Keep the production mode consistent with the last successful batch for this series.

```text
Create the confirmed sticker pack for [SERIES / CHARACTER ID].

IDENTITY
Use [APPROVED CHARACTER REFERENCE] as the only source of character identity.
Do not redesign the face, hairstyle, proportions, outfit language, or signature features.

STYLE / OUTPUT REFERENCES
Use [APPROVED OUTPUT REFERENCES] only for their recorded roles:
[STYLE / EXPRESSION / MOTION / COMPOSITION / CAPTION TREATMENT].
Do not transfer another series' character identity.

LOCKED OUTPUT PROFILE
Canvas: square 1:1, [APPROVED PIXEL SIZE].
Background: transparent.
Keep the character visually dominant and preserve safe margins.
Caption: exact wording below; no duplicate text or overlap.

CONFIRMED STICKER DEFINITIONS
[PASTE THE APPROVED BATCH DEFINITION TABLE]

PRODUCTION
Use the already approved production method for this series: [BATCH / INDIVIDUAL / HYBRID].
Do not add, remove, rename, or reinterpret stickers.
Export each sticker as an independent file.
Inspect the actual export against the five-point acceptance contract.
```
