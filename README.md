# matthewsburns.com

Source for [matthewsburns.com](https://matthewsburns.com) — the portfolio and pricing site for Matthew Burns, a web developer based in Pittsburgh, PA, building custom websites for local businesses.

A single-page static site: no build step, no framework, no dependencies to install.

## Contents

```
.
├── index.html          # the site (hero, work, pricing, process, contact)
├── 404.html            # custom not-found page
├── styles.css           # all styling
├── media/               # favicons, apple touch icon, Open Graph image
├── CNAME                # custom domain for GitHub Pages
├── robots.txt            # crawler rules + sitemap reference
└── sitemap.xml           # sitemap for search engines
```

## Tech

- Plain HTML5 + CSS3, no JavaScript
- Google Fonts: IBM Plex Mono and Inter
- Open Graph, Twitter Card, and JSON-LD (`ProfessionalService`) structured data for SEO/social previews
- Hosted on GitHub Pages with a custom domain via `CNAME`

## Local development

No build tools required. Clone the repo and open `index.html` directly in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deployment

Pushing to the default branch deploys automatically via GitHub Pages. The `CNAME` file points the custom domain (`matthewsburns.com`) at this repo — don't remove it, or the custom domain mapping will break.

## Updating content

- **Site copy / sections**: edit `index.html` directly (hero text, work samples, pricing tiers, process steps, contact info).
- **Styling**: `styles.css`.
- **Social preview image**: replace `media/og-image.png` (1200×630).
- **Favicons**: replace files in `media/`.
- **SEO metadata**: update the `<meta>` tags and JSON-LD block in `index.html`'s `<head>`, and bump `<lastmod>` in `sitemap.xml` when content changes meaningfully.

## Contact

For inquiries about the business itself (not the code): webdev@champsentertainment.com

## License

© 2026 Matthew Burns. All rights reserved — this is a commercial business site, not an open-source project intended for reuse.
