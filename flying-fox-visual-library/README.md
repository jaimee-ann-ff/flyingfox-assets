# Flying Fox Visual Schedule Library

202 images used by the Flying Fox Visual Schedule.

## Structure

**Flat** — all images at the top level, named by slug. This is what the WeasyPrint
PDF renderer expects.

```
{slug}.png
```

For example: `breakfast.png`, `laser-tag.png`, `karaoke.png`.

Category information is preserved in `manifest.json` (see below), not in the folder
structure.

## Uploading to GitHub

Drop the contents of this folder (all `.png` files + `manifest.json`) into:

```
github.com/jaimee-ann-ff/flyingfox-assets/main/visual-schedule/
```

Once uploaded, the WeasyPrint PDF renderer will find each image at:

```
https://raw.githubusercontent.com/jaimee-ann-ff/flyingfox-assets/main/visual-schedule/{slug}.png
```

## manifest.json

Machine-readable index. One entry per image with slug, display name, category, file
name, and byte size. Useful if you want to audit the library, generate documentation,
or reconcile against the artifact's shared library.

## Categories

- **Activities** — 98 images
- **Program** — 18 images
- **Routine** — 17 images
- **Meals** — 15 images
- **Excursions** — 14 images
- **Feelings** — 14 images
- **Transitions** — 9 images
- **Objects** — 5 images
- **People** — 4 images
- **Weather** — 4 images
- **Venues** — 3 images
- **Anchors** — 1 images

## Sizing note

These are the artifact-optimised versions: images resized to ~240px wide and
palette-quantised for a small footprint (typically 3-10 KB each). Good enough for
on-screen review and the visual schedule PDF at typical tile size (~50mm square in print).

For very large print (posters, high-res exports for Canva), you'll want the originals —
user-uploaded illustrations from your own source files, and library images (ARASAAC /
Mulberry) from the source repositories.

## Attribution

Library images sourced from:
- **ARASAAC** (arasaac.org) — CC BY-NC-SA 4.0. Attribution required for public use.
- **Mulberry Symbols** (straight-street.com) — CC BY-SA 2.0.
- **Custom Flying Fox illustrations** — created or commissioned for the org.
- **Staff uploads** via the artifact editor.

When publishing visual schedules externally (families, funders, partner orgs), include:
> Symbols by ARASAAC (arasaac.org) and Mulberry Symbols (straight-street.com), used
> under Creative Commons licenses.
