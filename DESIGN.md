# Dealer Pushback design system

Based on the Mercury style from Refero Styles, adapted for a static site on Porkbun hosting. Every token below lives as a CSS variable at the top of `assets/css/site.css`. Change it there, not per element.

## Principles

- **No divider lines.** Separate things with a step in background shade and with space. No `border-top`, `border-bottom` or hairline rules between sections or items.
- **No shadows, no gradients.** Depth comes only from the three surface shades.
- **One accent.** Cobalt is the only color. Use it for one phrase in the hero, step numbers and links. Never for body text or large fills.
- **Static only.** Plain HTML and CSS, no build step, no JavaScript, self-hosted fonts.

## Color

| Token | Hex | Use |
|---|---|---|
| `--canvas` | `#15151d` | Page background; hero and process sections |
| `--band` | `#1c1c27` | Alternating section background (questions, footer) so sections separate without lines |
| `--card` | `#1f1f2b` | Cards on the canvas |
| `--card-on-band` | `#262633` | Cards on a band, one step lighter |
| `--text` | `#f2f2f6` | Headings, primary text |
| `--muted` | `#d0d0d9` | Body copy, lede, tagline (9:1+ on every surface) |
| `--faint` | `#a9a9b7` | Caption role, footer (6:1+ on every surface) |
| `--cobalt` | `#5266eb` | Fills: logo tile, step-number badges, skip link |
| `--cobalt-text` | `#8f9cf5` | Blue text on dark: hero accent, links. Same tint as "PUSHBACK" in the logo |
| `--cobalt-deep` | `#222a66` | Portrait backdrop |

Blue appears in exactly two shades, both taken from the logo. No other hues.

## Type

One family: **Archivo** variable, self-hosted at `assets/fonts/archivo-latin-variable.woff2`. Body text is weight 430, slightly heavier than regular, because thin strokes fade on dark backgrounds.

| Role | Size | Weight | Tracking |
|---|---|---|---|
| H1 | 50–76px fluid (40–60 phone) | 540 | -0.045em |
| H2 | 32–46px fluid (30–38 phone) | 540 | -0.04em |
| H3 | 21–22px (20 phone) | 620 | -0.02em |
| Lede | 19–21px (18 phone) | 430 | 0 |
| Body | 18px (17px phone) | 430 | 0 |
| Caption role | 13px uppercase | 600 | 0.14em |
| Footer | 13px (12.5px phone) | 430 | 0 |
| Step number | 13px in a 32px cobalt badge | 650 | 0 |

Nothing on the page is smaller than 12px. Body paragraphs cap at 62 characters per line (`--measure`).

## Space and shape

- Max width `1200px`, gutter 24–64px fluid (20px on phones).
- Section rhythm `--section`: 72–112px fluid (56px on phones). Stacked sections share one gap, not two.
- Card padding `--card-pad`: 32px (22px on phones). Gap between cards `--gap`: 12px.
- Radius: `--radius-card` 14px for cards, `--radius-photo` 24px for the portrait, `--radius-badge` 8px for number tiles, `--radius-pill` 32px for the skip link, `--radius-sm` 4px for focus rings.

## Components

- **Sections:** alternate `--canvas` and `--band` backgrounds (hero canvas, questions band, process canvas, footer band). This is the only section separator.
- **Card:** `--card` (or `--card-on-band`) fill, 14px radius, no border. Used for the three questions and the process steps.
- **Portrait:** a transparent cutout (hair and beard edges keyed strand by strand from the original gray backdrop) that fades into the canvas at the shoulders, lit from above so the body falls into shadow. No frame or box: a soft cobalt radial glow (`.hero-person::before`) sits behind the head. The image is cropped to 480:545 from the top so the empty fade is trimmed, and the caption sits 14px below it, shifted 5.5% right (`left:5.5%`) so it centers under the chin, since the head is turned slightly. No shift on phones. Served as WebP with transparency; the JPEG fallback (also the social preview image) has the glow baked in. On phones it shrinks to 112px beside the name and the roles stack.
- **Name caption:** the logo's lettering: "RYAN PASCAL" in Archivo condensed caps (width 75, weight 760, 30px; 24px phones) with "PASCAL" in `--cobalt-text`. Roles below in 13px condensed caps `--faint`, separated by 5px cobalt squares.
- **Step number:** 32px cobalt tile with a white number, echoing the logo mark.
- **Question cards:** a three-column grid using subgrid, so numbers, headings and answers start on the same line in every card. Keep answers about the same length.
- **Section heading:** centered over its grid, `text-wrap: balance`. The process section carries one eyebrow above its heading: "Evidence first. Conclusions second." in uppercase `--cobalt-text`.
- **Process steps:** 2 × 2 grid of cards (one column on phones), number in a 32px left column.
- **Hero copy:** headline, one-sentence lede in `--text`, then three chips (icon + label: Repair records, Coverage rules, Past messages) on `--card`. From tablet width down the chips become three equal columns with the icon above the label.
- **Header:** sticky, frosted band (`rgba(28,28,39,.82)` + 14px backdrop blur), 80px tall (64px phones). Logo left at 46px (34px phones, 30px under 360px). Nothing on the right. No navigation links.
- **Footer:** compact band (28px/24px padding). Two columns: legal disclaimer (13px) and copyright (12px) on the left in `--faint`; the "Closed to new requests." notice on the right (15px heading in `--text`, 13px body in `--muted`). On phones they stack with the notice first.

## Brand marks

All in `assets/img/brand/` (favicon at the site root). Letters are outlined from Archivo, so the files need no font.

- **Mark, the "Pushback D":** a cobalt `#5266eb` tile (24% corner radius) holding a white D whose counter is a left-pointing arrow. The arrow is cut out (negative space), so the tile color shows through.
- **Wordmark:** "DEALER PUSHBACK" in Archivo condensed caps (width 75, weight 760, +0.02em tracking). "DEALER" in ivory `#ededf3` on dark or canvas `#171721` on light; "PUSHBACK" in cobalt (`#8f9cf5` on dark, `#5266eb` on light).
- **Clear space:** keep at least half the tile's height empty around the lockup.

| File | Use |
|---|---|
| `logo-primary.svg` | Mark plus wordmark for dark backgrounds. Used in the site header (46px tall, 34px on phones, 30px under 360px) |
| `logo-on-light.svg` | Same for light backgrounds: documents, email, print |
| `icon.svg` | Mark alone |
| `favicon.svg` | Mark at 32px |
| `apple-touch-icon.png` | 180px square, no rounding (iOS rounds it) |
| `icon-512.png`, `email-signature-icon.png` | Rounded mark at 512px and 104px |

When the logo changes, bump the `?v=` on its references in `index.html` and `404.html` so browsers fetch the new file.

## Cache busting

`site.css` is referenced with `?v=` set to the first 10 characters of its SHA-256. After any CSS edit, run:

```
H=$(sha256sum assets/css/site.css | cut -c1-10)
sed -i -E "s/site\.css\?v=[A-Za-z0-9]+/site.css?v=$H/" index.html 404.html
```

Then grep both files to confirm the new tag is there. Never bump versions with a broad find-and-replace like `?v=2` → `?v=3`, which can also hit the stylesheet tag.
