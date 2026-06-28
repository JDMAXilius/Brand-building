# Elyoun — Logo Assets

Generated 2026-06-27, per `BRAND_IDENTITY.md`. Premium dark/gold system.

## Files

| File | Format | Use |
|------|--------|-----|
| `elyoun-wordmark-dark.{svg,png}` | Vector + raster | **Primary.** Wordmark on obsidian. |
| `elyoun-wordmark-light.{svg,png}` | Vector + raster | Wordmark on light/bone backgrounds. |
| `elyoun-wordmark-transparent.{svg,png}` | Vector + raster (alpha) | Wordmark (bone) over photos/dark surfaces. |
| `elyoun-monogram-dark.{svg,png}` | Vector + raster | **E** monogram — favicon, app icon, avatar (dark). |
| `elyoun-monogram-light.{svg,png}` | Vector + raster | **E** monogram on light backgrounds. |
| `elyoun-lockup-horizontal-dark.{svg,png}` | Vector + raster | Wordmark + monogram + descriptor. |
| `_contact-sheet.png` | raster | Overview of all variants (not for production). |

The mark: a high-contrast serif wordmark **Elyoun** with a **gold full-stop** —
the signature device ("the standard, full stop"). The lettermark is an **E** in a
gold-ruled square (a hallmark/maker's-mark feel).

## Colors

- Obsidian `#0A0A0C` · Bone `#ECE8DF` / `#F7F5F0`
- Elyoun Gold `#C8A96A` · Light Gold `#E3C98C` · Deep Gold (light bg) `#A8884B`

## Rules

- **Clear space:** keep a margin of at least the height of the "E" (cap height) on all sides.
- **Minimum size:** wordmark ≥ 120px wide (digital); monogram ≥ 24px.
- **The gold dot is never removed or recolored.** It is the mark's signature.
- Use on obsidian or bone only — never gold-on-gold, never on busy backgrounds without a container.
- Don't stretch, rotate, recolor the wordmark, add effects, or substitute the typeface.

## Fonts (important)

- SVGs reference **Playfair Display** (free, Google Fonts), falling back to **Didot/Georgia**.
- PNG previews here are rendered in **Didot** (system serif) as a faithful stand-in.
- **For final production**, either install Playfair Display, or **convert the wordmark/E to outlines**
  (vector paths) so the logo is font-independent. The current SVGs use live text for editability.

## Regenerating PNGs

PNGs were produced from a Pillow script (in session scratchpad) using Didot.
The SVGs are the source of truth; re-export PNGs from the SVGs once Playfair Display
is installed, or hand to a designer to finalize as outlined vectors.
