# ReSinJo (English site)

Source for **www.resinjo.com** – static one-page website for the ReSinJo shelving-systems brand (HERATEC Export u. Beteiligungsges. mbH).

Plain HTML/CSS/vanilla JS, no build step, no framework. Open `index.html` directly in a browser to preview locally.

- Design spec: [`docs/superpowers/specs/2026-09-11-resinjo-onepager-design.md`](docs/superpowers/specs/2026-09-11-resinjo-onepager-design.md)
- German sister site: [resinjo.de](https://github.com/heralabs-code/resinjo.de) → www.resinjo.de

## Structure

- `index.html` – the one-page site
- `impressum.html` – legal notice
- `styles.css`, `script.js` – shared styling/behaviour (mobile nav)
- `assets/` – placeholder favicon; `logo-placeholder.svg` is a reference copy only (not referenced by any page)
- `sitemap.xml`, `robots.txt`, `CNAME` – hosting/SEO config for GitHub Pages

## Known placeholders

Search for `PLACEHOLDER` in `index.html` and `impressum.html` — contact details and legal register data still need to be filled in. This also finds the `PLACEHOLDER: swap this inline wordmark` comments marking where the real logo goes (it's inlined directly in the HTML in 2 places per file, not a swappable asset file).

**Before going live:** also remove the italic disclaimer paragraph at the top of `impressum.html` ("This page is a draft template, not legal advice...") — it is plain text, not a `PLACEHOLDER` marker, so the search above will not find it.

## Publishing changes

This site has no build step — GitHub Pages serves the files in this repo exactly as committed. To publish a change: edit the file (directly on github.com, or however you prefer), commit it to the `main` branch, and it goes live at www.resinjo.com within about a minute. Don't delete or rename the `CNAME` file — that's what tells GitHub which domain to serve this site on.
