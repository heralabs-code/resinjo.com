# ReSinJo (English site)

Source for **www.resinjo.com** – static one-page website for the ReSinJo shelving-systems brand (HERATEC Export u. Beteiligungsges. mbH).

Plain HTML/CSS/vanilla JS, no build step, no framework. Open `index.html` directly in a browser to preview locally.

- Design and implementation notes are kept locally outside Git tracking.
- German sister site: [resinjo.de](https://github.com/heralabs-code/resinjo.de) → www.resinjo.de

## Structure

- `index.html` – the one-page site
- `impressum.html` – legal notice
- `datenschutz.html` – privacy information
- `styles.css`, `script.js` – shared styling/behaviour (mobile nav)
- `assets/` – original RESINJO logo and favicon
- `sitemap.xml`, `robots.txt`, `CNAME` – hosting/SEO config for GitHub Pages

**Before going live:** STRATO says its data processing agreement is included automatically for contracts entered into since 18 July 2022; check older contracts in the account. Clarify which privacy agreement actually covers GitHub Pages, assess international transfers, and define the internal retention period for enquiries. The operator says no data protection officer is currently appointed. Dealer links lead to independent shops.

## Publishing changes

This site has no build step. Publishing with GitHub Pages requires Pages to be enabled and the domain's DNS records to point to GitHub Pages. The `CNAME` file only names the intended domain; it does not configure DNS.

**Checked 24 September 2026:** `www.resinjo.com` currently resolves to STRATO and redirects over HTTP to `www.palettenregal.net`; HTTPS on `www.resinjo.com` fails. `https://heralabs-code.github.io/resinjo.com/` returns 404. The files in this repository are therefore not currently published at the ReSinJo domain. A commit to `main` alone will not change this.
