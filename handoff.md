# Handoff: dealerpushback.com

Read this first in any new session. It covers the website only. Details about people Ryan helps never go in this repo, because the repo is public.

Last updated: October 21, 2026

## What Dealer Pushback is

Ryan Pascal, Pell City, Alabama, is a free consumer advocate for car owners when a dealer or manufacturer won't cover a repair. He is not an attorney, gives no legal advice, takes no payment, tips or gifts, works by email only, and never appears in court or arbitration. He refers people to a lawyer when something turns legal.

## Site status

- One page, live from this repo's `main` branch through Porkbun static hosting with GitHub Connect.
- Plain HTML and CSS. No build step, no framework, no JavaScript.
- Every push to `main` goes live. Use a `dev` branch for work in progress if needed.

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
handoff.md              this file
DESIGN.md               design rules
CLAUDE.md               points new sessions here
```

## Headshot

Source photo approved by Ryan. Processing: 4:5 crop, light contrast, color slightly reduced, fine film grain. No face edits, no AI retouching, ever. The top of the head sits close to the frame edge in the original; don't fake extra background.

## Planning documents (Ryan's claude.ai account)

- Full 59-task website plan, for a later multi-page site: https://claude.ai/code/artifact/2910e1ad-37ce-4a9b-a8b8-36f395ade709
