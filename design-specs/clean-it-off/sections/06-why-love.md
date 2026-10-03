# Why your skin will love Clean It Off (numbered slider)

- Figma node ids: 191:446
- Section top in page frame: y=2726.0px (screenshot crop y 2726–3686)
- Screenshot: `../screenshots/06-why-love.png`
- Raw JSON: `06-why-love.json`

## Typography used in this section

| Font | Weight | Italic | Size | Line-height px | Letter-spacing px | Count |
|---|---|---|---|---|---|---|
| Test Tiempos Fine | 500 | yes | 80.0 | 96.96 | -1.6 | 1 |
| Test Tiempos Fine | 400 | yes | 58.0 | 70.3 | -1.16 | 1 |
| Blauer Nue | 500 |  | 58.0 | 69.6 | -1.16 | 1 |
| Test Tiempos Fine | 500 | yes | 40.0 | 48.48 | -0.8 | 1 |
| Blauer Nue | 300 |  | 24.0 | 36.0 | -0.48 | 2 |
| Blauer Nue | 400 |  | 18.0 | 21.59 | -0.36 | 1 |
| Blauer Nue | 500 | yes | 16.0 | 22.4 | -0.16 | 1 |

## Colors used

- `#78563D` ×3
- `#FFFFFF` ×2
- `#28201F @ 80%` ×2
- `#28201F` ×1
- `#28201F @ 10%` ×1
- `#F5EEE6` ×1
- `#D9D9D9` ×1
- `#28201F @ 60%` ×1

## Corner radii

- 50.0px ×4
- 10.0px ×2

## Full node tree (positions in px, x from frame left, y from section top)

- GROUP `Group 2087330665` (191:446) [x0.0 y0.0 1920.0×960.0] 
  - RECTANGLE `Rectangle 1430107054` (191:447) [x0.0 y0.0 960.0×960.0] fills=["#D9D9D9", "IMAGE(ref=9dca23095541b7e634040f28a588b4df4e95906d, scaleMode=STRETCH)"]
  - RECTANGLE `Rectangle 1430107055` (191:448) [x960.0 y0.0 960.0×960.0] fills=["#F5EEE6"]
  - GROUP `Group 2087330662` (191:449) [x900.0 y420.0 130.0×130.0] radius=10.0
    - RECTANGLE `Rectangle 1430107056` (191:450) [x900.0 y420.0 130.0×130.0] fills=["#FFFFFF"] radius=10.0
    - **TEXT** `01` [x914.0 y434.0 42.0×48.0]  
      “01”  
      → Test Tiempos Fine 500 italic 40.0px / lh 48.48px (INTRINSIC_%) / ls -0.8px / LEFT / color ['#78563D']
    - **TEXT** `/04` [x982.0 y516.0 32.0×22.0]  
      “/04”  
      → Blauer Nue 400 18.0px / lh 21.59px (INTRINSIC_%) / ls -0.36px / LEFT / color ['#28201F @ 60%'] / case UPPER
  - GROUP `Group 2087330666` (191:453) [x1090.0 y100.0 700.0×704.0] radius=50.0
    - **TEXT** `Why your skin will love Clean It Off` [x1158.0 y100.0 564.0×140.0]  
      “Why your skin will love Clean It Off”  
      → Blauer Nue 500 58.0px / lh 69.6px (INTRINSIC_%) / ls -1.16px / CENTER / color ['#28201F']
      ↳ run “Why your skin will ”: {"fontSize": 58.0}
      ↳ run “love Clean It Off”: {"fontFamily": "Test Tiempos Fine", "fontWeight": 400, "italic": true, "fontSize": 58.0, "lineHeightPx": 70.2959976196289, "letterSpacing": -1.16, "color": ["#28201F"]}
    - GROUP `Group 2087330664` (191:455) [x1090.0 y290.0 700.0×514.0] radius=50.0
      - GROUP `Group 2087329688` (191:456) [x1253.0 y345.0 375.0×40.0] radius=50.0
        - RECTANGLE `Rectangle 34` (191:457) [x1253.0 y345.0 375.0×40.0] fills=["#78563D"] radius=50.0
        - **TEXT** `CLEANSES WITHOUT STRIPPING THE SKIN` [x1273.0 y354.0 336.0×22.0]  
          “CLEANSES WITHOUT STRIPPING THE SKIN”  
          → Blauer Nue 500 italic 16.0px / lh 22.4px (140.0%) / ls -0.16px / LEFT / color ['#FFFFFF'] / case UPPER
      - LINE `Line 10` (191:459) [x1090.0 y290.0 700.0×0.0] stroke={"paint": ["#28201F @ 10%"], "weight": 1.0, "align": "OUTSIDE"}
      - GROUP `Group 2087330663` (191:460) [x1122.0 y427.0 637.0×377.0] 
        - **TEXT** `17%` [x1374.0 y427.0 133.0×97.0]  
          “17% ”  
          → Test Tiempos Fine 500 italic 80.0px / lh 96.96px (INTRINSIC_%) / ls -1.6px / LEFT / color ['#78563D']
        - **TEXT** `Cocamidopropyl Betaine — coconut-derived` [x1182.0 y540.0 495.0×36.0]  
          “Cocamidopropyl Betaine — coconut-derived ”  
          → Blauer Nue 300 24.0px / lh 36.0px (150.0%) / ls -0.48px / CENTER / color ['#28201F @ 80%']
        - **TEXT** `Pairs two surfactants, not one. Cocamido` [x1122.0 y696.0 637.0×108.0]  
          “Pairs two surfactants, not one. Cocamidopropyl Betaine buffers the system so skin is thoroughly cleansed without the tight, stripped feeling after.”  
          → Blauer Nue 300 24.0px / lh 36.0px (150.0%) / ls -0.48px / CENTER / color ['#28201F @ 80%']

## Build notes

All numbers below come from the node tree above, `06-why-love.json`, or `figma-raw-node-191-36.json`. Coordinates use the same frame as the tree: x from the 1920 frame's left edge, y from the section top (page y 2726).

### Layout

- **Full-bleed split, no `.main-container`.** The section is 1920 × 960 and has two equal halves:
  - Left: image `Rectangle 1430107054` (191:447), x 0–960, 960 × 960, square (aspect 1:1). It has a `#D9D9D9` base fill under the image, which you can use as the placeholder colour.
  - Right: solid panel `Rectangle 1430107055` (191:448), x 960–1920, 960 × 960, fill `#F5EEE6`.
- **Section padding:** none inside the section; both halves start at y 0 and end at y 960. The page has a 100 px gap on each side of the section:
  - Section 05's group (191:393, h 700, starting at page y 1926) ends at page y 2626. That leaves 2626 → 2726 = **100 px above**.
  - This section ends at page y 3686, and section 07's heading starts at page y 3786. That leaves **100 px below**.
  - Suggested defaults: `padding_top: 0`, `padding_bottom: 0`. The 100 px gaps come from the neighbouring sections (05's bottom padding and 07's top padding).
- **Right content column** `Group 2087330666` (191:453): x 1090–1790, **700 px wide**. It is centred in the right panel with **130 px** on each side (1090 − 960 = 130; 1920 − 1790 = 130). Every text in it is centred on x ≈ 1440.
  - Panel top → heading top = **100 px**.
  - Body bottom (y 804) → panel bottom (y 960) = **156 px**.
  - So the content is *not* vertically centred: it sits 28 px above centre, because the content midpoint is y 452 and the panel midpoint is y 480. Use `padding: 100px 130px 156px`, or `justify-content: flex-start` with a 100 px top padding.
- **Vertical rhythm (right column):**

| From → to | Measured gap |
|---|---|
| panel top (0) → heading top (100) | 100 px |
| heading (100–240, 2 lines) → divider (y 290) | 50 px |
| divider (290) → pill top (345) | 55 px |
| pill (345–385) → stat "17%" top (427) | 42 px |
| stat (427–524) → stat caption top (540) | 16 px |
| stat caption (540–576) → body top (696) | **120 px** (a large gap, and it is deliberate in the file) |
| body (696–804) → panel bottom (960) | 156 px |

- **Heading box:** 564 px wide (x 1158–1722), centred. It wraps to 2 lines: "Why your skin will" / "love Clean It Off". Give it `max-width: 564px; margin: 0 auto;`.
- **Divider:** spans the full 700 px column (x 1090–1790).
- **Pill:** auto width, 375 × 40, centred (x 1253–1628).
- **Body:** 637 px wide (x 1122–1759), centred, 3 lines.
- **Counter badge** `Group 2087330662` (191:449): 130 × 130 at x 900–1030, y 420–550. It **straddles the image/panel seam**: 60 px sits over the image and 70 px over the panel. Its centre is (965, 485); the section centre is (960, 480), so the badge is 5 px right of and 5 px below true centre. Centre it on the seam: `left: 50%; top: 50%; transform: translate(-50%, -50%)`. If you need pixel parity, add a +5 px offset.
  - "01" is pinned top-left with a **14 px** inset (x 914 − 900, y 434 − 420).
  - "/04" is pinned bottom-right with a **16 px** right inset (1030 − 1014) and a **12 px** bottom inset (550 − 538).
- **Alignment:** everything in the right column is centred. The badge contents are left (number) and right (total).

### Text roles

| Role | Sample | CSS font-family | Weight | Size | Line-height | Letter-spacing | Transform | Colour |
|---|---|---|---|---|---|---|---|---|
| Section heading (roman part) | "Why your skin will " | `'Blauer Nue MD'` | 500 | 58px | 69.6px (120%) | -1.16px (-0.02em) | none | `#28201F` / `#28201FFF` / rgba(40,32,31,1) |
| Section heading (italic run) | "love Clean It Off" | `'Test Tiempos Fine Italic RG'` (italic) | 400 | 58px | 70.296px (121.2%) | -1.16px (-0.02em) | none | `#28201F` / `#28201FFF` / rgba(40,32,31,1) |
| Pill label | "CLEANSES WITHOUT STRIPPING THE SKIN" | `'Blauer Nue MD'` + `font-style: italic` (see Gotchas) | 500 italic | 16px | 22.4px (140%) | -0.16px (**-0.01em**) | uppercase (textCase UPPER) | `#FFFFFF` / `#FFFFFFFF` / rgba(255,255,255,1) |
| Stat number | "17%" | `'Test Tiempos Fine Italic'` (italic) | 500 | 80px | 96.96px (121.2%) | -1.6px (-0.02em) | none | `#78563D` / `#78563DFF` / rgba(120,86,61,1) |
| Stat caption | "Cocamidopropyl Betaine — coconut-derived" | `'Blauer Nue LT'` | 300 | 24px | 36px (150%) | -0.48px (-0.02em) | none | `#28201F` @ 80% / `#28201FCC` / rgba(40,32,31,0.8) |
| Body | "Pairs two surfactants, not one. Cocamidopropyl Betaine buffers the system so skin is thoroughly cleansed without the tight, stripped feeling after." | `'Blauer Nue LT'` | 300 | 24px | 36px (150%) | -0.48px (-0.02em) | none | `#28201F` @ 80% / `#28201FCC` / rgba(40,32,31,0.8) |
| Counter, current | "01" | `'Test Tiempos Fine Italic'` (italic) | 500 | 40px | 48.48px (121.2%) | -0.8px (-0.02em) | none | `#78563D` / `#78563DFF` / rgba(120,86,61,1) |
| Counter, total | "/04" | `'Blauer Nue RG'` | 400 | 18px | 21.59px (≈120%) | -0.36px (-0.02em) | uppercase (no visible effect) | `#28201F` @ 60% / `#28201F99` / rgba(40,32,31,0.6) |

Notes on the text:
- Text alignment in Figma is CENTER for the heading, caption and body. The stat, pill label and counter texts are LEFT inside auto-width boxes that are themselves centred, so in CSS use `text-align: center` for the whole column.
- The heading follows the theme's `h2.class_h2` + richtext `<em>` pattern. Override the class values (40px / line-height 100% / letter-spacing 0) with 58px / 1.2 / -0.02em.

### Components & states

- **Image half:** 960 × 960, no radius, no border. Use `object-fit: cover`. The Figma fill is STRETCH with `imageTransform [[1,0,0],[0,0.652,0.222]]`:
  - It shows the full width of the 1200 × 1840 source and a vertical slice from 22.2% to 87.4%, i.e. a 1200 × 1200 square starting at source y ≈ 409 px.
  - The CSS equivalent is `object-fit: cover; object-position: 50% 64%`.
- **Right panel:** `#F5EEE6` / rgba(245,238,230,1). No radius.
- **Divider** `Line 10` (191:459): 700 px × 1 px, `#28201F` @ 10% (`#28201F1A`, rgba(40,32,31,0.1)).
  - Stroke align is OUTSIDE, so it renders at y 289–290, just above the line's y 290.
  - Use `border-top: 1px solid rgba(40,32,31,.1)`.
- **Pill / tag** (`Rectangle 34`, 191:457):
  - 375 × 40, `border-radius: 50px` (fully rounded), fill `#78563D`, no border, no shadow.
  - Text inset: 20 px left (1273 − 1253), 19 px right (1628 − 1609), 9 px top (354 − 345), 9 px bottom (385 − 376). In CSS: `padding: 9px 20px; display: inline-block`.
- **Counter badge** (191:450): 130 × 130, fill `#FFFFFF`, `border-radius: 10px`, no shadow and no border (none in the file).
  - "01" and "/04" sit inside with the insets listed under Layout.
  - The "/04" total should be computed from the number of slides; the current index is zero-padded to 2 digits.
- **No arrows, dots or progress bar are drawn.** The only slider affordance is the 01/04 counter.
- **States:** only state 01 is designed, so no active/inactive styles exist.

### Assets

| File | Element |
|---|---|
| `assets/06-why-love/9dca23095541b7e634040f28a588b4df4e95906d.png` (1200 × 1840, RGB, close-up of a face/cheek) | Left half image, `Rectangle 1430107054` (191:447). Crop to a square (see the object-position above). |
| — | No SVG icons in this section (`icons.md` lists none for 06). |

### Interactions (inferred)

- *(inferred)* The "01 /04" counter means a **4-slide** slider. Each slide is probably: pill label + stat + stat caption + body text, and possibly a different left image.
- *(inferred)* Advance on autoplay (fade or vertical slide of the right-column content), and/or by swipe/drag on mobile. A click on the counter badge could go to the next slide.
- *(inferred)* Keep the heading and divider static. Only the pill, stat, caption, body (and the image, if it differs per slide) change.
- Swiper 11 is already loaded globally: `effect: 'fade'`, `loop: true`, `autoplay` optional, and update the counter on `slideChange`.
- Re-initialise on `shopify:section:load`, and on `shopify:block:select` go to the selected slide.

### Suggested customizer schema

Section settings:

| id | type | default / notes |
|---|---|---|
| `image` | image_picker | Default image for the left half (asset 9dca…). |
| `image_position` | select (`left`/`right`) | `left` |
| `heading` | richtext | `<p>Why your skin will <em>love Clean It Off</em></p>` |
| `show_divider` | checkbox | `true` |
| `color_background` | color | `#FFFCF9` (page) |
| `color_panel` | color | `#F5EEE6` |
| `color_text` | color | `#28201F` |
| `color_accent` | color | `#78563D` (pill fill, stat, counter number) |
| `color_pill_text` | color | `#FFFFFF` |
| `color_counter_bg` | color | `#FFFFFF` |
| `show_counter` | checkbox | `true` |
| `autoplay` | checkbox | `false` |
| `autoplay_speed` | range 3–10 s, step 1 | `5` |
| `padding_top` / `padding_bottom` | range 0–200 px | `0` / `0` |
| `mobile_padding_top` / `mobile_padding_bottom` | range 0–100 px | `0` / `0` |
| `custom_class` | text | "" |

Block type `slide` (limit 8):

| id | type | default (slide 1, from Figma) |
|---|---|---|
| `image` | image_picker | empty, which falls back to the section image |
| `label` | text | `Cleanses without stripping the skin` (rendered uppercase by CSS) |
| `stat` | text | `17%` |
| `stat_caption` | text | `Cocamidopropyl Betaine — coconut-derived` |
| `body` | textarea (or inline_richtext) | `Pairs two surfactants, not one. Cocamidopropyl Betaine buffers the system so skin is thoroughly cleansed without the tight, stripped feeling after.` |

Preset: 4 `slide` blocks so the counter reads /04.
- Figma only has copy for slide 1.
- For slides 2–4, either duplicate slide 1 or use the stat copy from section 09 (`6%` Glycerin, `5%` Aloe Barbadensis, `1%` Lactobacillus Ferment Lysate). That copy is taken from section 09, not from this design.

### Responsive suggestions (Figma is desktop-only; these are suggestions)

- **≤1400:**
  - Keep the split.
  - Right column padding 130 px → 60 px each side, top 80 / bottom 100.
  - Heading 58 → 48 px; stat 80 → 64 px; caption/body 24 → 20 px.
  - Caption → body gap 120 → 64 px.
- **≤990:**
  - Stack the halves: image on top (`aspect-ratio: 1/1` or 4/5), panel below.
  - Badge stays centred on the seam, now horizontal: `top: <image height>; left: 50%; transform: translate(-50%,-50%)`.
  - Panel padding 80 px 50 px 60 px.
  - Heading 40 px; stat 56 px; body 18 px; pill text 14 px.
- **≤768:**
  - Panel padding 60 px 16 px 48 px (matches the theme's 16 px mobile gutter).
  - Heading 28 px (theme mobile h2), line-height 120%.
  - Divider gap 50 → 24 px; pill height 34 px, text 12–13 px, padding 8 px 16 px, allowing wrap with `white-space: normal`.
  - Stat 48 px; caption and body 16 px / 150%; caption → body gap 32 px.
  - Counter badge 90 × 90, radius 8; "01" 28 px; "/04" 14 px; insets 10 px.
  - Enable swipe.

### Gotchas

- **Blauer Nue Medium *Italic* (PostScript `BlauerNue-Medium_Italic`) is used for the pill but is not loaded** in `assets/home-tlpc.css`, which only has the roman TH/LT/RG/MD files. `font-style: italic` on `'Blauer Nue MD'` will be a browser-synthesised oblique. Upload the italic woff2 if you need an exact match.
- The heading is a **mixed-style run**: the roman part is Blauer Nue 500 with line-height 69.6; the italic run is Tiempos 400 italic with line-height 70.296. Use the richtext `<em>` pattern. Don't hard-code a `<br>`; it wraps naturally at 564 px.
- The **stat is Tiempos Medium Italic 500** (`'Test Tiempos Fine Italic'`), not the Regular Italic used in headings.
- **Source text quirks:**
  - `textCase: UPPER` on "/04" (no visible effect).
  - The pill text is already uppercase in the source *and* has textCase UPPER. Store sentence case in the setting and use `text-transform: uppercase`.
  - Trailing spaces in "17% " and "Cocamidopropyl Betaine — coconut-derived ", so trim them (`| strip`).
  - The caption uses an em dash "—".
- **Inert radii:** Groups 191:453, 191:455 and 191:456 carry `cornerRadius 50`, but radii on groups do not render. Only `Rectangle 34` (pill) radius 50 and the badge rectangle radius 10 are real.
- The counter badge rectangle has `targetAspectRatio 198×198`, so it was scaled down from a 198 px original. 130 px is the final size.
- The badge is **off-centre by +5 px / +5 px** relative to the seam and the section middle. This is probably not intentional.
- The left image is **cropped by an imageTransform**, not shown whole. A merchant upload will need `object-fit: cover`. Expose a focal point, or `object-position`, if the crop matters.
- The 120 px gap between caption and body (larger than the gap between any other two elements) and the 100/156 top/bottom asymmetry are **in the design**. Do not "fix" them to equal values without checking.
- The pill letter-spacing is -0.01em. Every other text in this section uses -0.02em.
