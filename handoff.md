# Handoff: dealerpushback.com

Read this first in any new session. It covers the website only. Details about people Ryan helps never go in this repo, because the repo is public.

Last updated: October 21, 2026

## What Dealer Pushback is

Ryan Pascal, Pell City, Alabama, is a free consumer advocate for car owners when a dealer or manufacturer won't cover a repair. He is not an attorney, gives no legal advice, takes no payment, tips or gifts, works by email only, and never appears in court or arbitration. He refers people to a lawyer when something turns legal.

## Site status

- One page, live from this repo's `main` branch through Porkbun static hosting with GitHub Connect.
- Plain HTML and CSS. No build step, no framework, no JavaScript.
- Every push to `main` goes live. Use a `dev` branch for work in progress if needed.

### Changes on October 21, 2026 (evening)

- Logo added. Wordmark is "Dealer Pushback" in Archivo 650, width 84%, with "Pushback" on a yellow highlighter swipe. Icon is "DP" on a highlighter bar inside an ink square; it drops to "D" at favicon size. Tagline, where used: "Free consumer advocacy for car owners."
- The site header keeps the plain ink wordmark (no yellow), so the "I'm not a lawyer" line stays the only yellow on the page.
- `favicon.svg` replaced with the new icon. Added `assets/img/brand/` (logo, icon, apple-touch icon, email signature icon) and an apple-touch-icon link.
- The email signature loads `https://dealerpushback.com/assets/img/brand/email-signature-icon.png`. Don't move or rename that file.
- Phone layout reworked (720px and below): the photo is now a small byline beside the name instead of a full-screen image, section spacing is tighter, headline sizes and word spacing are tuned, and the numbered steps use a narrower number column.
- All browsers: more word spacing in the large headlines, and `color-scheme: light only` so Samsung Internet and Android Chrome don't force their own dark mode onto the page.
- Checked with no sideways scrolling at 320, 390 and 430 px phones, phone landscape, tablet and 1280 px desktop (Chromium). Not yet checked on a real iPhone in Safari.

### Still open

1. Headline. Current draft: "The dealer said no. Let's put the facts in writing." Ryan hasn't approved it yet.
2. Ryan to confirm the bio line: "I'm not a lawyer. Every decision is yours. I research the facts, put everything in writing, and make sure you're heard."
3. Ryan to confirm the "How it works" steps and the contact paragraph (written by Claude, not in the original brief).
4. Font: the plan named Switzer from Fontshare, but Fontshare couldn't be reached from the build environment, so the site uses Archivo (self-hosted, SIL Open Font License). Switching to Switzer would mean adding its woff2 files to `assets/fonts/` and updating the `@font-face` rule.
5. Email setup for ryan@dealerpushback.com: SPF, DKIM and DMARC.
6. Later: a site-style authorization form; an Alabama attorney's review of the site wording.

## Content rules

The page has nine parts, in this order: headline, photo, bio, the "I'm not a lawyer" line, what I do, always free, how it works, contact, footer disclaimer.

- Bio: business degree from UAB's Collat School of Business; B2B sales and account management in construction software, RFID, construction materials, hospital printing systems and steel distribution e-commerce; trained in legal research, data analysis and technical writing. Never mention law school.
- "What I do" is one list. No tiers, no prices.
- "Always free": "I'm selective about what I take on, and I see it through to the end." No number of spots.
- Footer disclaimer is fixed text. Don't edit it without Ryan's approval.
- Never use: lawyer, attorney, legal advice, counsel, represent, legal representative, cases, clients, except inside the disclaimers that say Ryan is not one. Also avoid: disputes, tiers, and phrasing like "until there's an answer" that hints at court.
- Use: consumer advocate, authorized to communicate on your behalf, research.
- No invented numbers, testimonials, star ratings or "as seen in" logos. Only sourced figures.
- No filler words (elevate, unlock, seamless, empower, journey, "Get started"), three-part slogans, "It's not X, it's Y" lines, or heavy dashes.
- No AI-written sources, ever.

## Design

See `DESIGN.md`.

## Files

```
index.html              the page
404.html                missing-page screen
favicon.svg             tab icon
robots.txt              search engines allowed
assets/css/site.css     all styles; tokens at the top
assets/fonts/           Archivo variable font + licence
assets/img/             headshot, 480px and 960px, JPG and WebP
assets/img/brand/       logo, icon and email-signature image
handoff.md              this file
DESIGN.md               design rules
CLAUDE.md               points new sessions here
```

## Headshot

Source photo approved by Ryan. Processing: 4:5 crop, light contrast, color slightly reduced, fine film grain. No face edits, no AI retouching, ever. The top of the head sits close to the frame edge in the original; don't fake extra background.

## Planning documents (Ryan's claude.ai account)

- Full 59-task website plan, for a later multi-page site: https://claude.ai/code/artifact/2910e1ad-37ce-4a9b-a8b8-36f395ade709
