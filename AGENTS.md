# Sonnet Shopify theme

## Design reference (Figma → local)
- The Clean It Off PDP design (Figma `575q58qifMXTxdfNw09mjq`, node 191:36) is fully extracted to `design-specs/clean-it-off/`. Start from `design-specs/clean-it-off/README.md`, which has the section index, the Figma-font → theme `font-family` map, and the tokens.
- Before building a section, read `design-specs/clean-it-off/sections/NN-*.md` (exact fonts, sizes, line-heights, letter-spacing, colors, padding, gaps, positions) and compare against `screenshots/NN-*.png`. Images and SVG icons are in `assets/NN-*/`.
- Icons are in theme `assets/cio-*.svg` (use `inline_asset_content`); customizer images are WebP in `~/Downloads/clean-it-off-customizer-images/`.
- Don't call the Figma API again unless the design has changed. Everything is in `figma-raw-node-191-36.json`.
- `design-specs/` and this file are excluded from theme uploads via `.shopifyignore`.

## Section conventions
- Fonts: one family per weight (`'Blauer Nue TH|LT|RG|MD'`, `'Test Tiempos Fine Italic RG'`). See the README table.
- Reuse `.main-container`, the `class_h2` richtext `<em>` italic pattern, `.arrow-slider` + `snippets/arrow-left|right.liquid`, and the padding/color settings pattern from the existing custom sections.
- Every section must be customizer-editable (schema settings + blocks + presets) and re-initialise its JS on `shopify:section:load`.
