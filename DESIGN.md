# Dealer Pushback — static editorial design rules
Revision: October 29, 2026, reflecting the user's removal of the Background section.

## Direction
A quiet, serious document-first website. Credibility comes from exact distinctions, restrained typography, evident source discipline and clear boundaries—not badges, aggressive language or decorative effects.

## Architecture
1. Opening: the difference between a repair diagnosis and a coverage determination, plus Ryan's real portrait and factual byline.
2. Three questions: dealer observation, manufacturer criteria, manufacturer decision.
3. Method: original terms, diagnosis/evidence, missing records, written terms.
4. Owner boundaries and confidentiality in one short paragraph, ending "The owner makes every decision."
5. Exact no-money/no-benefit commitment.
6. Permanent closure and footer attorney disclaimers.

The entire former Background/credentials section and its tinted background, padding, and navigation link were removed at the user's request. Do not reintroduce it or leave an empty spacer. The separate legal/role disclaimer in the footer must remain.

Do not repeat the same coverage/goodwill paragraph across multiple sections or let compliance text dominate the opening.

## Visual system
- Paper `#F7F7F5`, ink `#111113`, graphite `#49494B`, fine rules `#D2D2CF`, one deep charcoal band `#171719`.
- Self-hosted Archivo variable in `assets/fonts/archivo-latin-variable.woff2`; robust sans-serif fallback.
- Strong headline and short subhead; editorial section heads with generous width and space; 17–18px main reading text on desktops, readable 16px on phones.
- One restrained yellow `#FFE600` rule in the hero as the only accent, not a badge or neon decoration.
- Rules and white space, no cards or drop shadows, no stock imagery, gradients, animations, floaty buttons or artificial legal iconography.
- The portrait uses the **existing original photos**, preserving appearance. On wide screens it sits naturally with the hero; on phones it becomes a compact byline. Do not fake/replace the portrait with a placeholder or apply an aggressive radial mask. A subtle multiply blend is allowed solely to match the pale photographic background to the paper.
- No intake form, CTA, testimonial, external tracking or performance claims.
- The website's footer is not a public edit-history ledger. Keep internal Git history privately in the case repository.
- No backend, build tools, JavaScript or external dependency. Compatible with Porkbun static hosting.

## Responsive and accessibility
- Verify widths 1440, 1024, 768, 390 and 320 px. No horizontal overflow; single column at phone widths.
- Navigation is labeled and links only to the existing `#approach` anchor. Preserve semantic `main`, `section`, `h1–h3`, `ol` and descriptive portrait alt.
- All controls accessible by keyboard with visible focus. Reduced-motion preference avoids smooth scroll.
- Preserve the exact footer no-benefit line and original money paragraph, as required by the site's existing public commitments and current private case rules.

## Confidentiality
This repository is PUBLIC. Never commit owner identity, dealership/manufacturer case specifics, VIN, repair order, correspondence, strategic workflow or personal transcripts and letters. Private notes go in `ReyesPascal/LT_DP` only.
