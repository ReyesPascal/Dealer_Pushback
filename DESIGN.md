# Design rules: dealerpushback.com

The look should read as expensive and serious, never as an AI template. The concept is the marked-up file: paper, ink and one highlighter.

## Sources

The style blends three Refero design systems (styles.refero.design), structure only, never a copy of any brand:

- Ramp: off-white paper, black ink, one yellow highlighter as the only color; hierarchy from size, not decoration; hairlines, no shadows.
- Brex: gray body text at a short measure; one full-width dark band.
- shadcn/ui: solid black button; tight tracking on display type.

## Tokens (top of `assets/css/site.css`)

| Token | Value | Use |
| --- | --- | --- |
| `--paper` | `#F7F7F5` | page background |
| `--ink` | `#0E0E10` | headings, buttons, rules |
| `--graphite` | `#4A4A50` | body text |
| `--ash` | `#77777C` | captions, fine print |
| `--hairline` | `#DCDCD7` | dividers inside lists |
| `--band` | `#141416` | the one dark band |
| `--mark` | `#FFE600` | highlighter, used once |

## Type

- Archivo variable, self-hosted. One family only.
- Display: weight 600, width 84%, tracking -0.035em, line height 0.98.
- Section headings: weight 600, width 88%, tracking -0.025em.
- Body: weight 400, normal width, 18px (17px on phones), line height 1.6.
- Banned: Inter, Roboto, Geist, Satoshi, General Sans, Clash Display, Space Grotesk, Fraunces.

## Rules

- Yellow is only ever a background behind black text, and appears once: the "I'm not an attorney" line.
- One motion moment: the highlighter sweeps across that line once on load. Off when the device asks for reduced motion. Nothing else moves.
- Text is left-aligned. No centered hero, pill badges, logo rows, three floating feature cards or "Most popular" badges.
- No gradients, glass blur, glows, drop shadows, or a soft rounded card used everywhere.
- Corners: buttons 6px; photos and documents square.
- No all-caps labels over headings, no decorative monospace, no emoji, no icon on every heading.
- Imagery: Ryan's real photo and real data only. No stock photos, AI images, or illustrations of handshakes, shields or gavels.
- No cream backgrounds, terracotta, purple or blue gradients, or a near-black page with one neon accent.
- Layout must work at 390px phone width with no sideways scrolling; buttons go full-width on phones.
