# studio9-website

**Status:** Maintenance · last reviewed 2026-08-03

Teaser/landing page for **Studio 9 Design & Supply** (formerly ASA Tiles) — an
interior design studio and premium materials showroom in Fortitude Valley,
Brisbane.

Static site hosted on **GitHub Pages** at **s9d.com.au** (see `CNAME`). A full
WordPress build on the ArcHub theme is planned but not started.

Brand guidelines — colours, fonts, logo usage, tagline — and business details
are in [`CLAUDE.md`](CLAUDE.md). Follow them.

## Quick start

No build step. Open `index.html` directly, or serve the folder:

```bash
python -m http.server 8000
```

## Files

| File | What it is |
|---|---|
| `index.html` | The live landing page |
| `coming-soon.html` | Standalone holding page, with its own OG/description meta for link previews |
| `logo-9.jpg` | Logo asset |
| `CNAME` | Custom domain binding for GitHub Pages — **do not delete**, it's what maps s9d.com.au |

## Careful

- **Deploys are push-to-`main`.** GitHub Pages publishes automatically; there is
  no preview environment. Check rendering locally first.
- **Don't remove `CNAME`.** Losing it drops the custom domain and the site falls
  back to a `github.io` URL.
- Fonts are loaded from Google Fonts — keep the preconnect hints intact.

## Related

- [`../asatiles`](../asatiles) — the predecessor business (ASA Tiles) and its
  WordPress → Shopify migration
