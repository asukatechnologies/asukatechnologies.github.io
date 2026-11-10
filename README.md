# asukatechnologies.github.io

Company website for **Asuka Technologies LLC** — an independent software company
building mobile applications and open-source tools.

Live at <https://asukatechnologies.github.io>.

## Structure

- `index.html` — home page (about, products, open source, contact)
- `support.html` — product support information
- `privacy.html` — website privacy policy
- `dando/privacy.html` — Dando Privacy Policy
- `dando/terms.html` — Dando Terms of Use
- `dando/beta.html` — Dando Beta Test License Agreement (unlisted: not linked from
  the site, sent to invited testers by link)
- `dando/billing-return.html` — where Stripe checkout and the billing portal return
- `dando/dando-logo.svg` — the app icon with rounded corners (wordmark at 52% of the
  width, 5% corner radius), drawn with the app repo's `scripts/brand-geometry.mjs`
- `dando/dando-icon.svg` — browser-tab icon, copied from the app repo's `brand/`
- `uprange/` — redirects to `dando/`, kept for links in older app builds
- `styles.css` — shared stylesheet (light/dark via `prefers-color-scheme`)

Plain static HTML/CSS, no build step. Served by GitHub Pages from the default
branch root.
