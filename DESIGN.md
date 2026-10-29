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
| `--canvas` | `#171721` | Page background |
| `--card` | `#1e1e2a` | Cards, photo frame |
| `--raised` | `#272735` | The one emphasized block (closure notice) |
| `--text` | `#ededf3` | Headings, primary text |
| `--muted` | `#c3c3cc` | Body copy, lede, header tagline |
| `--faint` | `#9696a3` | Eyebrow labels, caption role, footer |
| `--cobalt` | `#5266eb` | Filled accents (skip link) |
| `--cobalt-text` | `#8f9cf5` | Cobalt for text on dark: hero accent, numbers, links |

## Type

One family: **Archivo** variable, self-hosted at `assets/fonts/archivo-latin-variable.woff2`. (Mercury's own face, Arcadia, isn't licensed for us. Archivo at medium weights carries the same calm feel.)

| Role | Size | Weight | Tracking |
|---|---|---|---|
| H1 | 52–80px fluid | 520 | -0.05em |
| H2 | 32–48px fluid | 520 | -0.045em |
| H3 | 20–21px | 600 | -0.02em |
| Lede | 19–21px | 400 | -0.01em |
| Body | 17px (16px mobile) | 400 | 0 |
| Eyebrow / role | 12px uppercase | 600 | 0.16em |
| Number | 13px tabular | 600 | 0 |

Headlines stay medium weight. Don't go back to 700+ heavy display type.

## Space and shape

- Max width `1200px`, gutter 24–64px fluid (20px on phones).
- Section rhythm `--section`: 72–112px fluid (56px on phones). Stacked sections share one gap, not two.
- Card padding `--card-pad`: 32px (22px on phones). Gap between cards `--gap`: 12px.
- Radius: `--radius-card` 12px for cards and blocks, 8px for the photo, `--radius-pill` 32px for buttons and the skip link, `--radius-sm` 4px for focus rings.

## Components

- **Card:** `--card` fill, 12px radius, no border. Used for the three questions, the process steps and the photo frame.
- **Question cards:** a three-column grid using subgrid, so numbers, headings and answers start on the same line in every card. Keep answers about the same length.
- **Process step:** card with the number in a 40px left column.
- **Emphasis block:** `--raised` fill, 12px radius, inside the page width. Only one per page.
- **Header:** wordmark left, tagline right, no bar or border.
- **Footer:** plain text in `--faint` on the canvas.
