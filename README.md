# dealerpushback.com

A public **one-page, static** personal volunteer research website. Source only: no client intake, backend, analytics, advertisements, JavaScript or build pipeline. The public content is about careful repair documentation and manufacturer coverage review, not about any identifiable owner or incident.

## For Claude and other editors
- **Read [CLAUDE.md](CLAUDE.md) first.** It describes boundaries, file ownership, quality checks and deployment.
- Read [DESIGN.md](DESIGN.md) before changing page structure or appearance.
- Read current `index.html` and `assets/css/site.css`, rather than an old screenshot or handoff. In particular, the current headline is *A diagnosis is not a coverage decision*.
- Private owner records and case-specific strategy live elsewhere; this **public** repository must never include them.

## Hosting and edits
The site uses **Porkbun static hosting with GitHub Connect**, sourced from the repository root on the `main` branch. `index.html` is the entry point. A push to `main` is configured to update the host; separately verify propagation when possible.

| Path | Purpose |
| --- | --- |
| `index.html` | Full page content, metadata, structured headings and in-page navigation |
| `404.html` | Static missing-page view using the same stylesheet |
| `assets/css/site.css` | All design tokens, typography and responsive rules |
| `assets/fonts/` | Self-hosted Archivo variable font and OFL license |
| `assets/img/` | Actual portrait in 480/960 JPG/WebP sizes and branding assets |
| `favicon.svg`, `robots.txt` | Static browser/search assets |
| `DESIGN.md`, `CLAUDE.md` | Design specification and editing/operating instructions |

No npm install, SSR, server functions, framework build, third-party fonts or runtime JS.

## Editing and release checklist
1. Verify explicit user authorization to modify/deploy this public site.
2. Make content changes to `index.html` and styles to `assets/css/site.css`. If assets change, preserve original portrait identity and license details.
3. Preserve exact **Always free** and no-benefit footer language, non-attorney disclosure, owner control, closure to new requests, and public confidentiality.
4. Check desktop, tablet and phone layouts, including 1440/1024/768/390/320px; use the **real** photo assets for visual approval. Verify navigation/anchors, image sources, accessibility, overflow and accurate claims.
5. Use meaningful commits. After pushing, read back `main` and confirm the actual changed files. Do not call a GitHub commit independent proof of the live Porkbun rendering.

**Previous revision warning:** older documentation mentioned a yellow animated attorney highlighter, a separate portrait overlay, the headline "Everything in writing" and the caption "Advocate". These describe **superseded designs**. Do not recreate them without new instruction.

## Copyright and licenses
Archivo: SIL Open Font License 1.1. See `assets/fonts/ARCHIVO-OFL.txt`. Retain existing font/image assets and credits as supplied.
