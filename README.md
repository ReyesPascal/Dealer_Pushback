# dealerpushback.com

One-page static site for Dealer Pushback. Plain HTML and CSS: no build step, no framework, no JavaScript.

## Hosting

Porkbun static hosting with GitHub Connect. Porkbun serves the repo root as the site, so `index.html` must stay at the top level. A push to the connected branch (`main`) updates the live site.

## Files

```
index.html                 the page
404.html                   shown for missing pages
favicon.svg                browser tab icon
robots.txt                 lets search engines index the site
assets/css/site.css        all styles
assets/fonts/              Archivo variable font (self-hosted) and its licence
assets/img/                headshot: 480px and 960px, JPG and WebP
```

## Editing

- Words: edit `index.html`. Keep the footer disclaimer as written.
- Colours, spacing and type: the variables at the top of `assets/css/site.css`.
- Yellow highlighter (`--mark`) is used in one place only: the "I'm not an attorney" line.

## Licences

Archivo is licensed under the SIL Open Font License 1.1 (see `assets/fonts/ARCHIVO-OFL.txt`), which allows self-hosting on a business site.
