# Header / navigation

- Figma node ids: 191:64, 191:92
- Section top in page frame: y=46.0px (screenshot crop y 26–112)
- Screenshot: `../screenshots/02-header.png`
- Raw JSON: `02-header.json`

## Typography used in this section

| Font | Weight | Italic | Size | Line-height px | Letter-spacing px | Count |
|---|---|---|---|---|---|---|
| Blauer Nue | 300 |  | 14.0 | 16.8 | -0.28 | 5 |

## Colors used

- `#28201F` ×11
- `#000000` ×2
- `#28201F @ 9%` ×1

## Full node tree (positions in px, x from frame left, y from section top)

- GROUP `Group 1321321656` (191:64) [x80.0 y0.0 1772.0×46.0] 
  - RECTANGLE `image 2` (191:65) [x917.0 y0.0 86.0×46.0] fills=["IMAGE(ref=b407fcaa358def7d6f6a8fe9e3c6a351c4b9c0f4, scaleMode=STRETCH)"]
  - GROUP `Group 1321321654` (191:66) [x1495.0 y14.0 235.0×17.0] 
    - **TEXT** `HOW IT WORKS` [x1495.0 y14.0 111.0×17.0]  
      “HOW IT WORKS”  
      → Blauer Nue 300 14.0px / lh 16.8px (INTRINSIC_%) / ls -0.28px / LEFT / color ['#28201F']
    - **TEXT** `OUR STORY` [x1646.0 y14.0 84.0×17.0]  
      “OUR STORY”  
      → Blauer Nue 300 14.0px / lh 16.8px (INTRINSIC_%) / ls -0.28px / LEFT / color ['#28201F']
  - GROUP `Group 1321321655` (191:69) [x80.0 y14.0 287.0×17.0] 
    - **TEXT** `SHOP ALL` [x80.0 y14.0 72.0×17.0]  
      “SHOP ALL”  
      → Blauer Nue 300 14.0px / lh 16.8px (INTRINSIC_%) / ls -0.28px / LEFT / color ['#28201F']
    - **TEXT** `SCIENCE` [x192.0 y14.0 60.0×17.0]  
      “SCIENCE”  
      → Blauer Nue 300 14.0px / lh 16.8px (INTRINSIC_%) / ls -0.28px / LEFT / color ['#28201F']
    - **TEXT** `ABOUT US` [x292.0 y14.0 75.0×17.0]  
      “ABOUT US”  
      → Blauer Nue 300 14.0px / lh 16.8px (INTRINSIC_%) / ls -0.28px / LEFT / color ['#28201F']
  - GROUP `Group 1321321653` (191:73) [x1772.0 y14.0 80.0×16.0] 
    - FRAME `Frame` (191:74) [x1804.0 y14.0 16.0×16.0] clips=true
      - GROUP `Group` (191:75) [x1804.0 y14.0 16.0×16.0] 
        - GROUP `Clip path group` (191:76) [x1804.0 y14.0 16.0×16.0] 
          - GROUP `a` (191:77) [x1804.0 y14.0 16.0×16.0] mask=true
            - VECTOR `Vector` (191:78) [x1804.0 y14.0 16.0×16.0] fills=["#000000"] stroke={"paint": ["#000000"], "weight": 1.0, "align": "INSIDE"}
          - GROUP `Group` (191:79) [x1805.61 y14.63 12.78×14.75] 
            - VECTOR `Vector` (191:80) [x1805.61 y22.0 12.78×7.37] stroke={"paint": ["#28201F"], "weight": 1.0, "align": "CENTER"}
            - VECTOR `Vector` (191:81) [x1808.31 y14.63 7.37×7.37] stroke={"paint": ["#28201F"], "weight": 1.0, "align": "CENTER"}
    - FRAME `Frame` (191:82) [x1772.0 y14.0 16.0×16.0] clips=true
      - GROUP `Group 1321321652` (191:83) [x1773.0 y15.0 14.0×14.0] 
        - VECTOR `Vector` (191:84) [x1783.62 y25.62 3.38×3.38] stroke={"paint": ["#28201F"], "weight": 1.0, "align": "CENTER"}
        - VECTOR `Vector` (191:85) [x1773.0 y15.0 12.44×12.44] stroke={"paint": ["#28201F"], "weight": 1.0, "align": "INSIDE"}
    - FRAME `Frame` (191:86) [x1836.0 y14.0 16.0×16.0] clips=true
      - GROUP `Group` (191:87) [x1837.75 y14.62 12.5×14.75] 
        - VECTOR `Vector` (191:88) [x1837.75 y19.62 12.5×9.75] stroke={"paint": ["#28201F"], "weight": 1.0, "align": "CENTER"}
        - VECTOR `Vector` (191:89) [x1840.25 y14.62 7.5×7.5] stroke={"paint": ["#28201F"], "weight": 1.0, "align": "CENTER"}
- LINE `Line 1` (191:92) [x0.0 y66.0 1920.0×0.0] stroke={"paint": ["#28201F @ 9%"], "weight": 1.0, "align": "CENTER"}

## Build notes

All numbers below come from the node tree above, `02-header.json`, or the raw Figma file (`figma-raw-node-191-36.json`). In this file, y=0 is page y=46, the top of the header content. The announcement bar occupies page y 0–26 above it.

### Layout

- **Header band**: page y 26 → 112 = **86 px** tall. It is 20 px top padding, 46 px content row and 20 px bottom padding, then a full-width 1 px bottom rule.
  - Announcement bar bottom (page y=26) → header content top (page y=46) = **20 px**.
  - Content row height = **46 px** (the logo height; `Group 1321321656` 191:64 is 1772 × 46).
  - Content bottom (y=46) → `Line 1` (191:92, y=66) = **20 px**.
  - Line 1 (page y=112) → product hero content (page y=132, `03-product-hero` frameOffsetY) = **20 px**.
- **Horizontal**: the header group runs from **x=80 to x=1852**. The left inset is **80 px** but the right inset is **68 px** (1920 − 1852). It isn't on the 100 px `.main-container` grid. See Gotchas.
- **Three zones** (CSS grid `1fr auto 1fr`):
  1. Left nav `Group 1321321655` (191:69) x 80 → 367 (287 wide): `SHOP ALL` x80 (w72), `SCIENCE` x192 (w60), `ABOUT US` x292 (w75). The gap between items is **40 px** (152→192, 252→292).
  2. Centre logo `image 2` (191:65) **86 × 46** at x=917, centred on x=960.
  3. Right side: nav `Group 1321321654` (191:66) x 1495 → 1730: `HOW IT WORKS` x1495 (w111), `OUR STORY` x1646 (w84), with a **40 px** gap (1606→1646). Then **42 px** (1730→1772) to the icon group `Group 1321321653` (191:73) x 1772 → 1852 (80 × 16).
     - Icons, each 16 × 16: search (191:82) x1772, account (191:74) x1804, bag (191:86) x1836. The gap between icons is **16 px**.
- Vertical alignment inside the 46 px row: nav text boxes are y=14, h=17 (centre 22.5); icons are y=14, h=16 (centre 22); logo centre 23. Use `align-items:center`.
- Bottom rule: `Line 1` is 1920 wide (full-bleed, not container width), 1 px, `#28201F` at **9%** opacity.
- The page background behind the header is the frame fill `#FFFCF9`. The header has no fill of its own.

### Text roles

| Role | Sample | CSS font-family | Weight | Size | Line-height | Letter-spacing | Transform | Color |
|---|---|---|---|---|---|---|---|---|
| Nav link (×5) | `SHOP ALL`, `SCIENCE`, `ABOUT US`, `HOW IT WORKS`, `OUR STORY` | `'Blauer Nue LT'` | 300 | 14px | 16.8px (120%) | -0.28px (-0.02em) | uppercase in the source string (no Figma textCase). Use `text-transform: uppercase` so editors can type any case | `#28201F` = `#28201FFF` = `rgba(40,32,31,1)` |

Bottom rule color: `#28201F` @ 9% = `#28201F17` = `rgba(40,32,31,0.09)`.

### Components & states

- **Logo**: raster image, displayed at **86 × 46**. Figma crops the source PNG (see Gotchas). No link styling is drawn.
- **Nav links**: plain text with no underline, pill or indicator. No hover or active state is drawn in Figma.
- **Icons** (all 16 × 16, stroke `#28201F`, stroke width **1 px**, no fill):
  - Search: a circle (12.44 × 12.44) plus a handle (3.38 × 3.38).
  - Account: a head (7.37 × 7.37) and shoulders (12.78 × 7.37). It uses a luminance mask inside the SVG.
  - Bag: a body (12.5 × 9.75) and handle (7.5 × 7.5).
- **No cart count badge** is drawn.
- **Bottom divider**: 1 px, `rgba(40,32,31,0.09)`, full width.
- No shadows, blur or effects (`effects: []` on every node).

### Assets

| Element | File |
|---|---|
| Logo "SONNET WELLNESS" | `assets/02-header/b407fcaa358def7d6f6a8fe9e3c6a351c4b9c0f4.png` (1667 × 1190 source, cropped in Figma). The same file is reused in `08-comparison`. |
| Search + account + bag icons (one combined 80 × 16 SVG, search at x0, account at x32, bag at x64) | `assets/02-header/icons/191-73-group-1321321653.svg`. Split it into three inline SVG snippets so each can be its own link. |

### Interactions (inferred)

- *Inferred:* nav links come from a `link_list` menu, split into a left group and a right group.
- *Inferred:* search opens the theme's predictive search (`sections/predictive-search.liquid`), account goes to `/account`, and bag opens the cart drawer (`sections/cart-drawer.liquid`) with a count badge.
- *Inferred:* the header could be sticky. Figma doesn't show it.
- *Inferred:* hover state for the links: a `#78563D` text color or an underline, consistent with the theme accent. Not designed.
- Mobile hamburger/drawer: not designed (see the responsive suggestions).

### Suggested customizer schema

This is most likely a restyle of the existing `sections/header.liquid` (a header group). If you build a new one:

| id | type | default | notes |
|---|---|---|---|
| `logo` | `image_picker` | (upload the cropped logo) | |
| `logo_width` | `range` 40–200, step 2, unit px | `86` | height auto (46) |
| `mobile_logo_width` | `range` 40–160, step 2, unit px | `64` | suggestion |
| `menu_left` | `link_list` | `main-menu-left` → SHOP ALL, SCIENCE, ABOUT US | |
| `menu_right` | `link_list` | `main-menu-right` → HOW IT WORKS, OUR STORY | |
| `show_search` / `show_account` / `show_cart` | `checkbox` | `true` | |
| `nav_gap` | `range` 16–80, step 2, unit px | `40` | |
| `padding_top` / `padding_bottom` | `range` 0–60, unit px | `20` / `20` | |
| `mobile_padding_top` / `mobile_padding_bottom` | `range` 0–40, unit px | `12` / `12` | suggestion |
| `color_background` | `color` | `#FFFCF9` | |
| `color_text` | `color` | `#28201F` | |
| `border_color` | `color` | `#28201F` | rendered at 9% opacity, or use `color_background`-aware rgba |
| `show_border` | `checkbox` | `true` | |
| `sticky` | `checkbox` | `false` | |
| `custom_class` | `text` | blank | |

### Responsive suggestions (Figma is desktop-only, so these are suggestions)

- ≤1660 / ≤1400: follow `.main-container` (80 → 50 px side padding). Reduce `nav_gap` to 32 px at ≤1400.
- ≤990: hide the text navs. Show a hamburger on the left (16 × 16 icon, same 1 px stroke) and the icons on the right. Keep the logo centred.
- ≤768: side padding 16 px, row height ~40 px (logo ~64 × 34), top and bottom padding 12 px. Keep search and bag, and move account into the drawer.

### Gotchas

- **Asymmetric side insets**: left 80 px, right 68 px. Figma draws the icon group 32 px past the 1820 content edge. Recommend symmetric padding (80 px each side, or the `.main-container` 100 px) and right-align the icons to that.
- **Logo is cropped in Figma**: the fill is `STRETCH` with an `imageTransform` that shows only x 9.06%–91.34% and y 17.74%–79.50% of the 1667 × 1190 PNG (about px 151–1523 × 211–946, aspect 209:112 ≈ 1.866). The raw PNG has extra empty margins, so crop it before uploading, or use `object-fit: cover` with a matching `object-position` on an 86 × 46 box.
- Nav letter-spacing is **-0.28px (-2%)**, while the announcement bar uses -0.56px at the same 14px size.
- The account icon SVG contains a luminance `mask` and a clip-path. If you inline it more than once, make the `id`s unique (`mask0_191_73`, `clip0_191_73`).
- The divider is 9% opacity (`#28201F17`), not the 10% (`#28201F1A`) used for dividers elsewhere on the page.
- Nav text is uppercase in the source string, with no textCase applied.
