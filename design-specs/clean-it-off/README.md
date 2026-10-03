# Clean It Off PDP — Figma design spec (local reference)

Source: Figma file `575q58qifMXTxdfNw09mjq`, frame **"CLEAN IT OFF" (node 191:36)**, desktop 1920 × 10294 px.
Link: https://www.figma.com/design/575q58qifMXTxdfNw09mjq/Untitled?node-id=191-36
Extracted 2026-10-03. Everything needed to build the sections is stored here, so building them should not need more Figma API calls.

**Ignored on purpose** (per the brief): `Rectangle 1139962724` (191:37), `Group 1321324248` (191:624), `Group 2087329716` (191:947).

## Folder map

| Path | What it is |
|---|---|
| `tokens.md` | Every text style (font, weight, size, line-height, letter-spacing), the full color palette, radii and effects, with usage counts |
| `sections/NN-slug.md` | One file per section: typography table, colors, radii, effects, plus the **full node tree** with x/y/w/h, fills, strokes, auto-layout padding/gap, and every text string with its exact style (including mixed-style runs) |
| `sections/NN-slug.json` | Same data as structured JSON |
| `screenshots/NN-slug.png` | 1:1 render of each section, 1920 px wide; `00-full-page.png` is the whole frame |
| `assets/NN-slug/` | Raster images used in the section (named by Figma imageRef) |
| `assets/NN-slug/icons/` | SVG exports of icons and vectors (stars, arrows, checkmarks, handles…) |
| `icons.md` | Index of every exported SVG |
| `image-refs.json` | Section → image refs |
| `figma-raw-node-191-36.json` | Untouched Figma REST response (geometry included), the fallback for anything not covered above |

Coordinates in `sections/*.md`: **x** is from the 1920 frame's left edge, **y** is from the top of that section. The content column runs from x=100 to x=1820 (1720 px), which matches `.main-container { padding: 0 100px }` in `assets/tlpc-pdp-style.css`.

## Section index

| # | Section | Figma node(s) | Top y in page | Screenshot |
|---|---|---|---|---|
| 01 | Announcement bar, "Save 20% on your first order" | 191:62, 191:63 | 0 | `screenshots/01-announcement-bar.png` |
| 02 | Header / nav (HOW IT WORKS, OUR STORY, SHOP ALL, SCIENCE, ABOUT US) | 191:64, 191:92 | 46 | `screenshots/02-header.png` |
| 03 | Product hero: gallery, title, reviews, benefits, pack size, ATC, trust row, accordions (Ingredients / Usage / Benefits), "Loved by thousands" quotes, "Complete your ritual" upsell | 191:60 … 191:392 (15 nodes) | 112 | `screenshots/03-product-hero.png` |
| 04 | "WHY US?" marquee strip | 191:135 | 1752 | `screenshots/04-why-us-marquee.png` |
| 05 | **Honest skin, honest results**: testimonial card + before/after compare | 191:393 | 1926 | `screenshots/05-honest-results.png` |
| 06 | "Why your skin will love Clean It Off", 01/04 numbered slider | 191:446 | 2726 | `screenshots/06-why-love.png` |
| 07 | "What's inside, and exactly why", ingredient carousel | 191:464, 465, 472, 473, 474, 479 | 3786 | `screenshots/07-whats-inside.png` |
| 08 | "What makes it different from others", comparison table | 191:484 | 4604 | `screenshots/08-comparison.png` |
| 09 | "The science behind the results", % stats | 191:540 | 5244 | `screenshots/09-science.png` |
| 10 | "Five products. one complete ritual", bundle builder | 191:589 | 6191 | `screenshots/10-bundle-ritual.png` |
| 11 | "Everything you want to know first", FAQ | 191:886 | 8150 | `screenshots/11-faq.png` |

## Page-level tokens

- Page background: `#FFFCF9`
- Primary text: `#28201F`. Opacity variants in use: 80% (`#28201FCC`), 50% (`#28201F80`), 10% (`#28201F1A`) for dividers, 8% (`#28201F14`)
- Accent brown (active buttons, CTAs): `#78563D`
- Light surfaces: `#F6F3EE` (inactive round buttons), `#F5EEE6` (compare handle, cards), `#EAE7E2`
- Announcement bar: `#BB9A82`
- Stars: `#F69104`
- Success green: `#008000`, with a 10% tint

## Figma font → theme CSS `font-family` mapping

The fonts are already loaded in `assets/home-tlpc.css`. **Each weight has its own family name**, so use the name, not `font-weight`:

| Figma | CSS `font-family` | weight |
|---|---|---|
| Blauer Nue 200 | `'Blauer Nue TH'` | 200 |
| Blauer Nue 300 | `'Blauer Nue LT'` | 300 |
| Blauer Nue 400 | `'Blauer Nue RG'` | 400 |
| Blauer Nue 500 | `'Blauer Nue MD'` | 500 |
| Test Tiempos Fine 500 (roman) | `'Test Tiempos Fine'` | 500 |
| Test Tiempos Fine 400 *italic* | `'Test Tiempos Fine Italic RG'` | 400, italic |
| Test Tiempos Fine 500 *italic* | `'Test Tiempos Fine Italic'` | 500, italic |
| Test Tiempos Fine 600 *italic* (FAQ numbers, bundle) | **not loaded**. Closest is `'Test Tiempos Fine Italic'` (500); upload a SemiBold Italic woff2 if an exact match is needed | |
| Montserrat 500 / 700 | **not loaded by the theme** (the live accent font is `futura_n4`). Load it per section with a `font_picker` setting (default `montserrat_n5`) + `font_face`, as `sections/honest-results.liquid` does with `tag_font` | |

Letter-spacing in Figma is almost always **-2% of the font size** (e.g. 58px → -1.16px = `-0.02em`). Line-heights are mostly 120% (headings), 130% (small text) and 150% (body copy).

## Existing theme conventions to reuse

- `.main-container`: 100px side padding (80 at ≤1660, 50 at ≤1400, 16 at ≤768)
- `h2.class_h2` with a richtext `<em>` gives the Tiempos italic word ("Honest skin, *honest results*" pattern)
- `.arrow-slider` + `snippets/arrow-left.liquid` / `arrow-right.liquid`: 48px round nav buttons, `#F6F3EE` → hover `#78563D`
- Swiper 11 is loaded globally (deferred) in `layout/theme.liquid`
- Section settings pattern: `padding_top/bottom`, `mobile_padding_top/bottom`, `color_background`, `color_text`, `custom_class`
- Mobile breakpoint: `max-width: 768px`

## Icons are already in theme `assets/` (prefix `cio-`)

All Figma icons are in the theme's `assets/` folder, deduplicated and named by what they show. `theme-icon-map.json` maps each Figma export to its theme file. Use them inline so `currentColor` and CSS colors work:

```liquid
{{ 'cio-star-filled.svg' | inline_asset_content }}
```

Single-color icons built for recoloring (`currentColor`): `cio-star-filled`, `cio-star-outline`, `cio-compare-chevrons`, `cio-arrow-left`, `cio-arrow-right`. The other icons keep their Figma colors.

| Group | Files |
|---|---|
| Honest results | cio-star-filled, cio-star-outline, cio-compare-handle (with pill bg), cio-compare-chevrons, cio-arrow-left, cio-arrow-right |
| Product hero | cio-check-circle-outline, cio-shield, cio-leaf, cio-heart, cio-badge-check, cio-plus-circle-small, cio-play-button(-2/-3), cio-star-small, cio-plus, cio-truck, cio-lock, cio-return, cio-rating-stars-4 |
| Header | cio-header-search-account-cart |
| Why-us marquee | cio-marquee-shield-check, -face, -badge, -leaf, -heart, -india, -no-chemicals |
| What's inside | cio-circle-arrow-next, cio-circle-arrow-prev |
| Comparison | cio-check-circle-filled, cio-cross-circle |
| Science | cio-science-sun-skin, -skin-layers, -drops, -shield-cross, -face-glow |
| FAQ | cio-faq-plus-circle, cio-faq-minus-circle |

## Images for the customizer (WebP)

`~/Downloads/clean-it-off-customizer-images/<section>/` holds every image as WebP, cropped exactly as Figma frames it (the inverse of the Figma imageTransform). Its `README.md` maps each file to a Figma node and, for Honest Results, to the customizer setting.
