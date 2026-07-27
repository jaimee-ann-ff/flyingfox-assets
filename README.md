# Flying Fox Visual Schedule Library

202 images used by the Flying Fox Visual Schedule editor artifact.

## What's here

- `manifest.json` — machine-readable index: slug, display name, category, filename, size
- One folder per category, each containing images named by slug

## Categories

- **Activities** (98) → `activities/`
- **Program** (18) → `program/`
- **Routine** (17) → `routine/`
- **Meals** (15) → `meals/`
- **Excursions** (14) → `excursions/`
- **Feelings** (14) → `feelings/`
- **Transitions** (9) → `transitions/`
- **Objects** (5) → `objects/`
- **People** (4) → `people/`
- **Weather** (4) → `weather/`
- **Venues** (3) → `venues/`
- **Anchors** (1) → `anchors/`

## Slug naming

Every image is named by its Flying Fox slug (e.g. `breakfast.png`, `trivia.png`).
Slugs are the primary reference used in the visual schedule JSON exports and by the
WeasyPrint renderer.

## Sizing note

These are the artifact-optimised versions: images resized to ~240px wide and
palette-quantised for a small footprint (typically 3-10 KB each). Good for on-screen
review and for the artifact's picker thumbnails.

**For high-resolution print or Canva work**, use the originals — user-uploaded
illustrations come from your own source files, and library images (ARASAAC / Mulberry)
are available at higher resolution in `flying-fox-library-v2.zip`.

## Using with the WeasyPrint PDF renderer

The `flying-fox-visual-schedule` skill's `render_visual_schedule.py` expects images at:

```
https://raw.githubusercontent.com/jaimee-ann-ff/flyingfox-assets/main/visual-schedule/{slug}.png
```

To wire this library up to the renderer, upload the images (or a chosen subset) to
that path in the `flyingfox-assets` repo. The renderer will pick them up automatically
for any tile whose slug matches.

## Attribution

Library images sourced from:
- ARASAAC (CC BY-NC-SA 4.0)
- Mulberry Symbols (CC BY-SA 2.0)
- Custom illustrations commissioned by Flying Fox
- Custom uploads via the artifact editor
