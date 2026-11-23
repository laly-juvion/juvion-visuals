# Juvion Visuals

Interactive showcases and visuals from Juvion's neuromuscular research, published with GitHub Pages.

**Live site:** https://laly-juvion.github.io/juvion-visuals/

## Contents

| Path | What it is |
|---|---|
| `index.html` | Gallery page listing every visual |
| `neuromuscular-showcase/` | Interactive stand showcase, dark edition |
| `neuromuscular-showcase/light/` | Same showcase, light edition |
| `neuromuscular-showcase/img/` | Images used by the showcase |
| `assets/` | Gallery preview images |
| `assets/fonts/` | Inter typeface files shared by every page |
| `assets/brand/` | Juvion logo and favicon (from the juvion-website repo) |

Images and fonts are ordinary files that the pages load by path (nothing is base64-embedded).

**Branding** follows juvionhs.com: brand orange `#fe6603`, Playfair Display for headings (loaded from Google Fonts, like the website) and Inter for text.

**Offline use (e.g. at a stand):** download the repository (Code → Download ZIP), unzip it, and open `neuromuscular-showcase/index.html` in Chrome or Edge. Keep the folder structure intact. Without internet, headings fall back from Playfair Display to Georgia; everything else is identical.

## Adding a new visual

1. Create a folder for it, e.g. `my-new-visual/`, with an `index.html` and its images inside. Load fonts from `../assets/fonts/fonts.css` and the logo from `../assets/brand/`.
2. Add a 1280×720 preview image to `assets/`.
3. In the root `index.html`, add an entry at the top of the `VISUALS` list (newest first; the first entry is shown large).
4. Commit. The site updates within a minute or two.

## Using the stand showcase

- Loops automatically. Tap or click to pause and explore; glowing points open descriptions.
- Resumes the tour on its own after 45 seconds without interaction.
- Keys: arrow keys change slides, F toggles full screen, Esc closes a panel or resumes the tour.
