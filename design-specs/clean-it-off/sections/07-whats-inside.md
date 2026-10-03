# What's inside, and exactly why (ingredient carousel)

- Figma node ids: 191:464, 191:465, 191:473, 191:472, 191:474, 191:479
- Section top in page frame: y=3786.0px (screenshot crop y 3686–4604)
- Screenshot: `../screenshots/07-whats-inside.png`
- Raw JSON: `07-whats-inside.json`

## Typography used in this section

| Font | Weight | Italic | Size | Line-height px | Letter-spacing px | Count |
|---|---|---|---|---|---|---|
| Blauer Nue | 500 |  | 58.0 | 69.58 | -1.16 | 1 |
| Test Tiempos Fine | 400 | yes | 58.0 | 70.3 | -1.16 | 1 |
| Blauer Nue | 500 |  | 24.0 | 33.6 | -0.48 | 1 |
| Blauer Nue | 200 |  | 18.0 | 25.2 | -0.36 | 1 |

## Colors used

- `#28201F` ×4
- `#FFFFFF` ×2
- `#78563D` ×2
- `#F6F3EE` ×1
- `#28201F @ 85%` ×1

## Corner radii

- 500.0px ×5

## Full node tree (positions in px, x from frame left, y from section top)

- **TEXT** `What's inside, and exactly why.` [x573.0 y0.0 775.0×70.0]  
  “What's inside, and exactly why.”  
  → Blauer Nue 500 58.0px / lh 69.58px (INTRINSIC_%) / ls -1.16px / LEFT / color ['#28201F']
  ↳ run “What's inside, ”: {"fontSize": 58.0}
  ↳ run “and exactly why.”: {"fontFamily": "Test Tiempos Fine", "fontWeight": 400, "italic": true, "fontSize": 58.0, "lineHeightPx": 70.2959976196289, "letterSpacing": -1.16, "color": ["#28201F"]}
- GROUP `Group 2087330667` (191:465) [x-120.0 y130.0 2160.0×410.0] 
  - ELLIPSE `Ellipse 96` (191:466) [x755.0 y130.0 410.0×410.0] fills=["#78563D"]
  - RECTANGLE `image` (191:467) [x760.0 y135.0 400.0×400.0] fills=["IMAGE(ref=da18476568dd2b6ab6a3f9dc1701196fb6aca4c5, scaleMode=FILL)"] radius=500.0
  - RECTANGLE `image` (191:468) [x1800.0 y215.0 240.0×240.0] fills=["IMAGE(ref=89e6709f45e59e1961021c57c2b1545723f626a1, scaleMode=FILL)", "IMAGE(ref=0ca26c4c8999d6900178bd5c5a22610baf535beb, scaleMode=STRETCH)"] radius=500.0
  - RECTANGLE `image` (191:469) [x-120.0 y215.0 240.0×240.0] fills=["IMAGE(ref=d43977f4b6a2f1696c7c2d91bb3af7aebafe7747, scaleMode=FILL)"] radius=500.0
  - RECTANGLE `image` (191:470) [x318.0 y185.0 300.0×300.0] fills=["IMAGE(ref=34a97845f6ce0aecd2ad8ed44ed6b86640221fdc, scaleMode=FILL)"] radius=500.0
  - RECTANGLE `image` (191:471) [x1303.0 y185.0 300.0×300.0] fills=["IMAGE(ref=7a676a09316cd91948ce651abc35051f9695a8c4, scaleMode=FILL)"] radius=500.0
- **TEXT** `LACTOBACILLUS FERMENT LYSATE 1%` [x736.0 y570.0 448.0×34.0]  
  “LACTOBACILLUS FERMENT LYSATE 1%”  
  → Blauer Nue 500 24.0px / lh 33.6px (140.0%) / ls -0.48px / CENTER / color ['#28201F'] / case UPPER
- **TEXT** `Postbiotic active that helps maintain a ` [x784.0 y618.0 352.0×100.0]  
  “Postbiotic active that helps maintain a comfortable, conditioned skin surface. Inactivated ferment lysate — not a live culture.”  
  → Blauer Nue 200 18.0px / lh 25.2px (140.0%) / ls -0.36px / CENTER / color ['#28201F @ 85%']
- GROUP `Group 1321321714` (191:474) [x1186.0 y645.0 46.0×46.0] 
  - ELLIPSE `Ellipse 6` (191:475) [x1186.0 y645.0 46.0×46.0] fills=["#78563D"]
  - FRAME `Frame` (191:476) [x1200.0 y659.0 18.0×18.0] clips=true
    - VECTOR `Vector` (191:477) [x1203.7 y662.7 10.61×10.61] rotation=0.79 stroke={"paint": ["#FFFFFF"], "weight": 1.5, "align": "CENTER"}
    - VECTOR `Vector` (191:478) [x1203.7 y662.7 10.61×10.61] rotation=0.79 stroke={"paint": ["#FFFFFF"], "weight": 1.5, "align": "CENTER"}
- GROUP `Group 1321321715` (191:479) [x688.0 y645.0 46.0×46.0] 
  - ELLIPSE `Ellipse 6` (191:480) [x688.0 y645.0 46.0×46.0] fills=["#F6F3EE"]
  - FRAME `Frame` (191:481) [x702.0 y659.0 18.0×18.0] clips=true
    - VECTOR `Vector` (191:482) [x705.7 y662.7 10.61×10.61] rotation=2.36 stroke={"paint": ["#28201F"], "weight": 1.5, "align": "CENTER"}
    - VECTOR `Vector` (191:483) [x705.7 y662.7 10.61×10.61] rotation=2.36 stroke={"paint": ["#28201F"], "weight": 1.5, "align": "CENTER"}

## Build notes

All numbers below come from the node tree above, `07-whats-inside.json`, or `figma-raw-node-191-36.json`. y is measured from the section top (page y 3786 = the heading's top). x is measured from the frame's left edge.

### Layout

- **Background:** none. The page colour `#FFFCF9` shows through.
- **Full-bleed carousel.** The image row is wider than the viewport: `Group 2087330667` (191:465) runs x −120 → 2040 (2160 px). Figma clips its render to x 0–1920, so the section needs `overflow: hidden`. The text block is centred on x 960; no `.main-container` columns are used.
- **Section padding:**
  - **Top 100 px.** Section 06 ends at page y 3686; this heading starts at 3786.
  - **Bottom 100 px.** The body text ends at y 718 (page 4504); section 08's card starts at page y 4604.
  - Total height 918 = 100 + 718 + 100, which matches the crop 3686–4604.
- **Heading:** single line, auto width 775 px (x 573–1348), centred (box centre 960.5).
- **Carousel row:** five circles, all vertically centred on **y 335**.

| Slot | Node | Box (x, y, size) | Centre x | Visible |
|---|---|---|---|---|
| far-left (prev-2) | 191:469 | x −120, y 215, 240 × 240 | 0 | right half only (render 0–120) |
| left (prev-1) | 191:470 | x 318, y 185, 300 × 300 | 468 | full |
| **active** | 191:467 (image) + 191:466 (ring) | image x 760, y 135, 400 × 400; ring x 755, y 130, 410 × 410 | 960 | full |
| right (next-1) | 191:471 | x 1303, y 185, 300 × 300 | 1453 | full |
| far-right (next-2) | 191:468 | x 1800, y 215, 240 × 240 | 1920 | left half only (render 1800–1920) |

- **Size scale:** active 400 → neighbours 300 (×0.75) → outer 240 (×0.6).
- **Horizontal gaps between circle edges:**
  - far-left → left: 120 → 318 = **198 px**.
  - left → active image: 618 → 760 = **142 px** (137 px to the ring at 755).
  - active image → right: 1160 → 1303 = **143 px** (138 px from the ring at 1165).
  - right → far-right: 1603 → 1800 = **197 px**.
- **Centre-to-centre pitch:** 468, 492, 493, 467 px. That is almost uniform, ≈ 480 ± 13.
- **Text block under the carousel**, centred on x 960:
  - Ingredient title: auto width 448 px (x 736–1184).
  - Description: fixed width **352 px** (x 784–1136), height grows with the text (`textAutoResize: HEIGHT`). Use `max-width: 352px`.
- **Arrows:** two 46 × 46 buttons on the same row as the description, vertically centred on it.
  - Description y 618–718 has centre 668; arrows y 645–691 have centre 668.
  - Prev: x 688–734. Next: x 1186–1232.
  - Gap arrow → description = **50 px** on both sides (784 − 734, 1186 − 1136).
  - Arrow group span 688–1232 (544 px), centred on 960.
- **Vertical rhythm:**

| From → to | Gap |
|---|---|
| section top → heading top (0) | 100 px (section padding) |
| heading (0–70) → active ring top (130) | **60 px** (65 px to the active image at 135; 115 px to the 300 px circles at 185; 145 px to the 240 px circles at 215) |
| active ring bottom (540) → title top (570) | **30 px** (35 px from the image bottom at 535) |
| title (570–604) → description top (618) | **14 px** |
| description (618–718) → section bottom | 100 px |

- **Alignment:** everything is centred.

### Text roles

| Role | Sample | CSS font-family | Weight | Size | Line-height | Letter-spacing | Transform | Colour |
|---|---|---|---|---|---|---|---|---|
| Section heading (roman part) | "What's inside, " | `'Blauer Nue MD'` | 500 | 58px | 69.58px (120%) | -1.16px (-0.02em) | none | `#28201F` / `#28201FFF` / rgba(40,32,31,1) |
| Section heading (italic run) | "and exactly why." | `'Test Tiempos Fine Italic RG'` (italic) | 400 | 58px | 70.296px (121.2%) | -1.16px (-0.02em) | none | `#28201F` / `#28201FFF` / rgba(40,32,31,1) |
| Ingredient title | "LACTOBACILLUS FERMENT LYSATE 1%" | `'Blauer Nue MD'` | 500 | 24px | 33.6px (140%) | -0.48px (-0.02em) | uppercase (textCase UPPER) | `#28201F` / `#28201FFF` / rgba(40,32,31,1) |
| Ingredient description | "Postbiotic active that helps maintain a comfortable, conditioned skin surface. Inactivated ferment lysate — not a live culture." | `'Blauer Nue TH'` | 200 | 18px | 25.2px (140%) | -0.36px (-0.02em) | none | `#28201F` @ 85% / `#28201FD9` / rgba(40,32,31,0.85) |

Notes on the text:
- Figma sets the heading's `textAlignHorizontal` to LEFT, but in an auto-width box that is centred on the page. Use `text-align: center`.
- The title and description are CENTER-aligned.
- The heading uses the `h2.class_h2` + `<em>` pattern, overridden to 58px / 1.2 / -0.02em.

### Components & states

- **Ingredient circle (inactive):**
  - Image rectangle with `cornerRadius 500`, so it renders as a circle (`border-radius: 50%`).
  - Image fill mode FILL, which maps to `object-fit: cover`.
  - No border, no shadow.
  - Sizes: 300 px next to the active slide, 240 px for the outer slides.
- **Ingredient circle (active):** a 400 × 400 circular image plus a **progress-ring arc** `Ellipse 96` (191:466).
  - The ring box is 410 × 410, offset −5 px on every side of the image.
  - Fill `#78563D`. `arcData.innerRadius 0.97`, so the ring is 205 × 0.03 ≈ **6.15 px thick**: it runs from radius 198.85 to 205, against an image radius of 200. That leaves about 5 px of brown visible outside the image and about 1.15 px underneath its edge.
  - Arc from −94° to +50° (Figma angles, clockwise from 3 o'clock). In screen terms it starts just left of 12 o'clock and runs clockwise to about 4:30, a **144° sweep (40% of the circle)**. The render bounds confirm this: x 945.7–1165, y 130–492.
  - It is drawn only on the active circle.
  - Build it as an SVG `<circle>` with `r ≈ 201.9`, `stroke-width ≈ 6.15`, `stroke-dasharray` equal to the circumference, and `stroke-dashoffset` animating. Rotate it −94° so it starts at the top.
  - `strokeWeight 4.1` appears in the raw node, but no stroke paint exists, so ignore it.
- **Arrow buttons** (`Group 1321321714`, `Group 1321321715`):
  - 46 × 46 circles.
  - Glyph: an 18 × 18 frame at a 14 px inset holding two vectors (chevron + shaft), stroke 1.5 px, round caps and joins.
  - **Prev (191:479):** fill `#F6F3EE`, glyph `#28201F` (the inactive/default look).
  - **Next (191:474):** fill `#78563D`, glyph `#FFFFFF` (the active/hover look).
  - This matches the theme's `.arrow-slider` (`#F6F3EE` → hover `#78563D`, white icon). The theme button is 48 px, so set `width/height: 46px` here.
  - The glyph paths match `snippets/arrow-left.liquid` and `arrow-right.liquid` exactly (18 × 18, stroke 1.5, same path coordinates), so reuse the snippets.
- **No dots or pagination.**

### Assets

| File | Element |
|---|---|
| `assets/07-whats-inside/da18476568dd2b6ab6a3f9dc1701196fb6aca4c5.png` (500 × 500, blue bacteria render) | Active circle 191:467, Lactobacillus Ferment Lysate |
| `assets/07-whats-inside/34a97845f6ce0aecd2ad8ed44ed6b86640221fdc.png` (1200 × 720, blue gel texture) | Left circle 191:470 |
| `assets/07-whats-inside/7a676a09316cd91948ce651abc35051f9695a8c4.png` (1200 × 1680, beige powder) | Right circle 191:471 |
| `assets/07-whats-inside/d43977f4b6a2f1696c7c2d91bb3af7aebafe7747.png` (736 × 1104, clear gel swirl) | Far-left circle 191:469 |
| `assets/07-whats-inside/0ca26c4c8999d6900178bd5c5a22610baf535beb.png` (1237 × 619, aloe slices on green) | Far-right circle 191:468, **top** fill (the visible one), STRETCH with a 90° rotation transform |
| `assets/07-whats-inside/89e6709f45e59e1961021c57c2b1545723f626a1.png` (600 × 500, RGBA white powder) | Far-right circle 191:468, **bottom** fill, fully covered by the aloe image, so it is not visible |
| `assets/07-whats-inside/icons/191-479-group-1321321715.svg` | Prev arrow button (46 px, `#F6F3EE` circle + dark arrow) |
| `assets/07-whats-inside/icons/191-474-group-1321321714.svg` | Next arrow button (46 px, `#78563D` circle + white arrow) |

### Interactions (inferred)

- *(inferred)* A **centre-mode infinite carousel**. Prev/next (and swipe) move the ring of circles, and the centred item becomes the active slide: it grows to 400 px, gets the brown progress arc, and its title and description appear below.
  - Swiper 11: `centeredSlides: true`, `loop: true`, `slidesPerView: 'auto'`, `speed ≈ 600`, `slideToClickedSlide: true`.
  - Use a fixed-width slide (≈ 400 px layout box, spaceBetween ≈ 80 px for the ≈ 480 px pitch) and size the slides with `transform: scale()`: `.swiper-slide-active` 1, `-prev`/`-next` 0.75, the rest 0.6.
- *(inferred)* The 144° arc is an **autoplay progress indicator**: it fills 0 → 360° over the autoplay delay, then advances. Use Swiper's `autoplayTimeLeft` event to drive `stroke-dashoffset`. Without autoplay, show a static decorative arc.
- *(inferred)* Title and description cross-fade on `slideChange`. Read them from the active slide's data attributes or from hidden per-slide markup.
- *(inferred)* Arrows: either both always look the same (`#F6F3EE` default, `#78563D` hover), or prev is shown disabled-looking. With loop on, both should be enabled.
- Re-init on `shopify:section:load`; on `shopify:block:select`, `slideToLoop(index)`.

### Suggested customizer schema

Section settings:

| id | type | default / notes |
|---|---|---|
| `heading` | richtext | `<p>What's inside, <em>and exactly why.</em></p>` |
| `show_progress_ring` | checkbox | `true` |
| `autoplay` | checkbox | `true` |
| `autoplay_speed` | range 3–10 s | `5` |
| `color_background` | color | `#FFFCF9` |
| `color_text` | color | `#28201F` |
| `color_accent` | color | `#78563D` (ring, next-arrow / hover fill) |
| `color_arrow_bg` | color | `#F6F3EE` |
| `active_size` | range 240–480 px, step 10 | `400` |
| `padding_top` / `padding_bottom` | range 0–200 px | `100` / `100` |
| `mobile_padding_top` / `mobile_padding_bottom` | range 0–100 px | `50` / `50` |
| `custom_class` | text | "" |

Block type `ingredient` (limit 12):

| id | type | default |
|---|---|---|
| `image` | image_picker | — (uploaded in the customizer) |
| `name` | text | `Lactobacillus Ferment Lysate 1%` (CSS uppercases it) |
| `description` | textarea | `Postbiotic active that helps maintain a comfortable, conditioned skin surface. Inactivated ferment lysate — not a live culture.` |

Preset: 5 ingredient blocks (the design shows 5 circles).
- Figma only provides copy for the active one (Lactobacillus).
- Placeholder names for the others could reuse section 09's ingredient list (Glycerin 6%, Cocamidopropyl Betaine 17%, Aloe Barbadensis 5%). That copy is taken from section 09, not from this design.

### Responsive suggestions (Figma is desktop-only; these are suggestions)

- **≤1400:**
  - Active 340 px; neighbours 255; outer 204 (same 0.75 / 0.6 ratios).
  - Pitch ≈ 410 px.
  - Heading 48 px.
- **≤990:**
  - Active 300 px; neighbours 225; outer slides hidden or peeking.
  - Heading 40 px; title 20 px; description 16 px.
- **≤768:**
  - Heading 28 px (theme mobile h2), line-height 120%, wrapping allowed. Heading → carousel gap 32 px.
  - Active 220 px (ring 6 px → 4 px); neighbours 150 px peeking at the edges.
  - Title 18 px / 140%; title → description 10 px. Description 16 px / 140%, max-width ~280 px.
  - Arrows 36 px (theme `.arrow-slider` mobile size), either beside the description or moved under it with an 8 px gap.
  - Side gutter 16 px for the text; the carousel itself stays full-bleed.

### Gotchas

- **Two image fills on the far-right circle (191:468).** The visible top layer is the aloe image (`0ca26…`), STRETCH with `imageTransform [[0,-0.5004,0.7502],[1,0,0]]`: the centre square of a 2:1 landscape image, **rotated 90°**. Beneath it is the white powder (`89e67…`), which is fully hidden. Export or crop the aloe image to a square before uploading.
- **The ring is an arc, not a full ellipse.** `arcData` gives start 0.8727 rad (50°), end −1.6406 rad (−94°), innerRadius 0.97. The tree above lists it only as an ellipse with fill `#78563D`. Rendered as a full disc, it would look like a brown 410 px circle behind the image.
- **Radius 500** on the image rectangles is just "fully round". Use `border-radius: 50%`.
- **The ingredient title uses textCase UPPER**, and the source string is already uppercase. Store natural case in the setting and apply `text-transform: uppercase`.
- **The description weight is 200 (Figma "ExtraLight").** The theme maps 200 to `'Blauer Nue TH'`, whose file is named *Blauer-Nue-Thin*. Check visually that it is not lighter than the design.
- **Mixed-style heading:** Blauer 500 roman + Tiempos 400 italic run, with slightly different line-heights (69.58 vs 70.296).
- **The arrow vectors carry `rotation 0.79` / `2.36` rad (45° / 135°)** in the tree because they were drawn as rotated chevrons. Use the exported SVGs or the theme snippets, not a hand-rotated path.
- The heading uses the straight apostrophe in "What's", and the description uses an em dash "—".
- **Spacing asymmetry:** neighbour gaps are 142 vs 143 px and edge gaps 198 vs 197 px. Treat them as equal.
- **The carousel group is wider than the frame** (x −120 → 2040). Without `overflow: hidden` on the section wrapper you get horizontal page scroll.
