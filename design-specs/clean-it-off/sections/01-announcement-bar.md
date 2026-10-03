# Announcement bar

- Figma node ids: 191:62, 191:63
- Section top in page frame: y=0.0px (screenshot crop y 0–26)
- Screenshot: `../screenshots/01-announcement-bar.png`
- Raw JSON: `01-announcement-bar.json`

## Typography used in this section

| Font | Weight | Italic | Size | Line-height px | Letter-spacing px | Count |
|---|---|---|---|---|---|---|
| Blauer Nue | 300 |  | 14.0 | 16.8 | -0.56 | 1 |

## Colors used

- `#BB9A82` ×1
- `#FFFFFF` ×1

## Full node tree (positions in px, x from frame left, y from section top)

- RECTANGLE `Rectangle 5` (191:62) [x0.0 y0.0 1920.0×26.0] fills=["#BB9A82"]
- **TEXT** `Save 20% on your first order` [x867.0 y4.0 185.0×17.0]  
  “Save 20% on your first order”  
  → Blauer Nue 300 14.0px / lh 16.8px (INTRINSIC_%) / ls -0.56px / LEFT / color ['#FFFFFF']

## Build notes

All numbers below come from the node tree above, `01-announcement-bar.json`, or the raw Figma file (`figma-raw-node-191-36.json`). Desktop frame = 1920 px. Fonts follow the README mapping.

### Layout

- Full-bleed bar, **1920 × 26 px** (`Rectangle 5`, 191:62), background `#BB9A82`. No container or side padding: the text is centred on the page.
- Single line of text `Save 20% on your first order` (191:63), box 185 × 17 at x=867, y=4. Its centre is x=959.5, so it is centred in the 1920 frame (allow for the 0.5 px rounding).
- Vertical rhythm: bar top → text top = **4 px**; text bottom (y=21) → bar bottom (y=26) = **5 px**. Build it as `height: 26px; display:flex; align-items:center; justify-content:center` and don't use padding. The 17 px text box is 16.8 px line-height rounded.
- Next element: the header group starts at page y=46, so there is **20 px** between the bar's bottom (y=26) and the header content. That 20 px is the header's top padding (see `02-header.md`), not the bar's.
- Alignment: center.

### Text roles

| Role | Sample | CSS font-family | Weight | Size | Line-height | Letter-spacing | Transform | Color |
|---|---|---|---|---|---|---|---|---|
| Announcement text | `Save 20% on your first order` | `'Blauer Nue LT'` | 300 | 14px | 16.8px (120%) | -0.56px (-0.04em) | none (sentence case in source) | `#FFFFFF` = `#FFFFFFFF` = `rgba(255,255,255,1)` |

Background: `#BB9A82` = `#BB9A82FF` = `rgba(187,154,130,1)`.

### Components & states

- One component: a solid bar with no border, radius, shadow or effects (`effects: []` in raw).
- No link, icon, close button, arrows or rotating messages are drawn in Figma.

### Assets

- None. It's pure CSS and text, with no images or icons in `assets/` for this section.

### Interactions (inferred)

- *Inferred:* the whole bar could link to a discount or collection URL (optional `link` setting).
- *Inferred:* the theme's `sections/announcement.liquid` already supports multiple messages with autoplay/marquee. If the client wants rotating messages, reuse it and restyle it to the values above. Figma shows a single static message.

### Suggested customizer schema

Section `announcement-bar-cio` (or restyle the existing `announcement.liquid`):

| id | type | default | notes |
|---|---|---|---|
| `text` | `richtext` (or `text`) | `Save 20% on your first order` | |
| `link` | `url` | blank | wraps the bar when set |
| `color_background` | `color` | `#BB9A82` | |
| `color_text` | `color` | `#FFFFFF` | |
| `font_size` | `range` 10–20, step 1, unit px | `14` | |
| `bar_height` | `range` 20–60, step 1, unit px | `26` | desktop |
| `mobile_bar_height` | `range` 20–60, step 1, unit px | `26` | |
| `custom_class` | `text` | blank | theme convention |

Optional block `message` (`text`, `link`) for rotating messages, `max_blocks: 5`.

### Responsive suggestions (Figma is desktop-only, so these are suggestions)

- ≤1400 / ≤990: no change, since the bar is centred and full width.
- ≤768: keep 14px (or drop to 12px if the copy gets longer), and add `padding: 0 16px` to match `.main-container` mobile gutters. Let the text wrap with `min-height: 26px` rather than a fixed height, so a long message isn't clipped.

### Gotchas

- **Letter-spacing is -4% here** (-0.56px on 14px), not the page-wide -2%. The header nav uses -0.28px on the same 14px size, so don't copy one into the other.
- Line-height is Figma "INTRINSIC" (auto). 16.8px = 120% of 14px.
- The text box isn't vertically centred to the pixel (4 px above, 5 px below). Use flex centring.
- The bar's 26px height doesn't include the 20px gap above the header. That gap belongs to the header section.
