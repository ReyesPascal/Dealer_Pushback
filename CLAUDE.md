# CLAUDE.md — Dealer Pushback (PUBLIC website repository)

This file is the first read for Claude Code or any AI coding assistant operating in this repository. **This repository is public.** It contains website source only, never an owner's records or internal strategy.

## Read order / authority
1. Read `DESIGN.md` (approved current design direction) and the **current files** `index.html`, `assets/css/site.css`, `404.html`, `README.md`. Current source outranks descriptions of historical layouts.
2. Review the user's **latest explicit instruction** and do only the authorized task. Do not deploy changes just because a plan or older approval exists.
3. If the user grants access to the separate **private** case repository `ReyesPascal/LT_DP`, read its root `CLAUDE.md`, `GOGOGO.md` and `project/conduct.md` for relevant strategic/conduct constraints. Do NOT reproduce its private content in this public repository. If inaccessible, do not infer its contents.
4. Honor the stricter of the latest specific user boundary and the applicable confidentiality/conduct controls. Do not assume a legal role or impersonate the owner.

## What the site IS
- `dealerpushback.com`: a one-page, personally maintained, unpaid and permanently closed volunteer research undertaking.
- Its thesis is **"A diagnosis is not a coverage decision."** The page explains the difference between a repair diagnosis, a manufacturer's published criteria and a written coverage decision, plus separate possible goodwill review.
- Ryan's role is research and record analysis; **the vehicle owner writes their own outbound messages and alone decides repairs, costs and offers**.
- The site is **not** a profession, business, intake funnel, law firm, customer review site, or a public case record.

## Current page anatomy — follow the actual DOM
1. Header: wordmark and two in-page links (`#approach`, `#background`), not a contact or intake button.
2. Hero: specific thesis, brief evidence-led explanation, existing **real portrait** and factual caption "Technical research · Record analysis".
3. `#approach`: three differentiated questions—technician findings, the exact covered condition, the manufacturer's actual decision.
4. Process: four source-grounded steps—original terms, diagnostic records, omissions, written scope/cost/coverage versus goodwill.
5. `#background`: specific qualifications and constraints, with a prominent accurate non-attorney disclaimer.
6. Owner boundaries: source provenance and owner authority; private communications stay private.
7. One "Always free" section preserving the exact no-benefit policy.
8. Permanent closure, then legal/role disclaimer footer.
Avoid repeated multi-paragraph versions of the same point. Hierarchy and brevity are more important than a long checklist.

## Non-negotiable public-content boundaries
- **NEVER** put an owner's name, dealership, manufacturer connected to a particular request, vehicle/VIN, repair order, case number, quote, correspondence, records, incident dates, legal argument, private strategy, private book text, transcript or attachments in this repository. No reviews, testimonials, success stories or allegations about any dealer.
- Do not imply a guarantee of coverage, goodwill, a response, professional accreditation, law degree, legal practice, agency relationship, or official manufacturer association.
- Keep documented undergraduate degree distinct from Auburn **graduate coursework**, which is not an asserted master's degree. Other credentials or law-school attendance are described narrowly. Verify before adding claims.
- The original site money language is fixed: **"Always free. No payment, tips, gifts or donations. No ads, sponsors or affiliate links. No referrals to law firms, repair shops or car buyers, and nothing accepted from them. No reviews, testimonials or success stories. Not now, and not later."** The footer must retain **"I accept no payment, tips, gifts or benefit of any kind."**
- Maintain "not a vocation, business or profession", no new work, no intake, and the non-attorney/non-legal-advice boundaries.
- The user specifically removed the dated public edit-history sentence and `records@dealerpushback.com` footer invitation. **Do not restore it**, even if old historical instructions mention it.
- Do not add "family" to the public description unless newly directed. If asked a factual question, answer truthfully.
- Avoid pressure, threats, aggressive imagery, fabricated authority or "scare tactics". Specific evidence and professional restraint convey seriousness.

## Files, runtime and deployment
- `index.html`: entire one-page site; `404.html`: missing-page view.
- `assets/css/site.css`: all styles, design tokens, responsive breakpoints; no separate portrait overlay stylesheet.
- `assets/fonts/archivo-latin-variable.woff2`: self-hosted font, license `assets/fonts/ARCHIVO-OFL.txt`.
- `assets/img/ryan-pascal-480.jpg`, `ryan-pascal.jpg` and matching WebP images: real portrait at alternate sizes. Preserve aspect ratio and identity. Do not swap in placeholder screenshots or AI faces.
- `favicon.svg`, `assets/img/brand/`, `robots.txt`: static assets.
- **Porkbun static hosting with GitHub Connect**: repository-root `index.html` is the entry point; pushes to connected `main` are configured for deployment. No framework, Node build, SSR, Python backend, JavaScript dependency, third-party font/image CDN, forms, analytics, external APIs or hosting configuration invented by the assistant.
- A GitHub commit verifies source state; **it does not prove Porkbun has deployed the change**. Confirm live site separately if accessible.
- Commit only changes requested/authorized; use clear commit messages and verify the exact file SHA or content after writes.

## Visual and technical QA required before claiming completion
- Inspect the *actual* site or a faithful local browser render at 1440, 1024, 768, 390 **and 320 px**. Ensure no horizontal overflow, clipping, tiny text, cramped header, broken anchoring or awkward portrait balance.
- Test with the **real portrait assets**, not a gray placeholder; if you cannot access them, disclose that specific limitation. Earlier "passing" layout scores failed to detect a bad-looking page.
- Keep one simple editorial visual language: paper, ink, restrained yellow rule, ample spacing, no heavy blocks, generic feature cards, neon/gradients, stock illustrations, radial portrait masks or decorative motion. Follow `DESIGN.md`.
- Check semantic headings, label/anchor targets, image alt, focus-visible keyboard behavior, tap targets and reduced-motion handling.
- Recheck exact no-money/no-benefit wording, attorney disclaimer, closed intake, privacy, and absence of accidental case identifiers.
- If testing or publication is blocked, report the blocker and what did/didn't ship. Do not invent passing audits, independent "agents" or deployment confirmation.

## History and continuity
Previous designs (particularly revisions 3–4) were rejected after a visual review despite static checklists passing. The current release is the simpler **revision 5** design with one stylesheet. Never roll back to "Everything in writing", the "Advocate" caption, artificial portrait masks, repetitive legal/compliance blocks or a public edit-history request without a new explicit user direction.

Case history, source PDF/video preservation, book-specialist workflow, and cross-session handoff belong **only** in private `ReyesPascal/LT_DP`. This public CLAUDE.md intentionally contains none of them.
