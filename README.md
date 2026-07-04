# Woven Within — by Melissa (v2: The Studio Wall update)

Where creativity becomes care. Creative life coaching, handmade goods, original watercolor art, and soulful resources for mothers.

## What's new in v2

- **The Studio Wall** — a real gallery of 16 of Melissa's original watercolors with handwritten-style titles and a full-screen lightbox (arrow keys work).
- **Real crochet in the shop** — Fire & Ice, Warm Colors, and Aqua Colors shawls plus the three one-of-a-kind statement neck pieces (Oceania, Earthy, Splash of Lime), photographed pieces replacing placeholders.
- **Free coloring pages** — four of Melissa's original line drawings turned into printable US-Letter PDFs (A Gathered Bouquet, Crown of Flowers, Heart of Flowers, Fern Leaf) with download buttons. A perfect gentle lead-in to the Grounding Guides.
- Hero now features three real paintings (Flow, Hokkaido Sunset, Blossom) as leaning framed canvases.
- Journal cards use the botanical watercolors (Fern, Snowflake, Pine); the Work Together offers use Movement, Pastels, and Crown of Flowers.
- New "Gallery" link in the navigation.

## How to update the live site

1. Unzip this package **over** the existing repo folder (do NOT delete the repo first).
2. These five images stay from the existing repo — the zip intentionally does not include them:
   - `public/images/melissa-portrait.jpg`
   - `public/images/shop-sweater-1.jpg`
   - `public/images/shop-sweater-2.jpg`
   - `public/images/art-bee.png`
   - `public/images/art-honeycomb.png`
3. Commit and push. Vercel rebuilds automatically.

## Setup

```bash
npm install
npm run dev      # Local development at localhost:4321
npm run build    # Build for production (output: dist/)
```

Vercel settings: Framework Preset **Astro**, build `npm run build`, output `dist`. No `index.html` in the repo root.

## Project structure

```
public/
  images/
    art/        ← 18 original watercolors (gallery, hero, journal, offers)
    shop/       ← 6 crochet photos (shawls + statement neck pieces)
    coloring/   ← 4 line-drawing previews
  downloads/    ← 4 printable coloring-page PDFs
src/
  layouts/Base.astro   ← nav, footer, favicons, scroll-reveal
  pages/index.astro    ← homepage (all sections + lightbox)
  styles/global.css    ← design tokens
```
