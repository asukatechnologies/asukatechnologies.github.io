# asukatechnologies.github.io

Company website for **Asuka Technologies LLC** — an independent software company
building mobile applications and open-source tools.

Live at <https://asukatechnologies.github.io>.

## Structure

- `index.html` — home page (about, products, open source, contact)
- `support.html` — product support information
- `privacy.html` — website privacy policy
- `dando/index.html` — the Dando app page (kept general while the app is in internal
  testing)
- `dando/privacy.html` — Dando Privacy Policy
- `dando/delete-account.html` — how to delete a Dando account, in the app or by email
  (the account deletion URL for Google Play's Data safety form)
- `dando/terms.html` — Dando Terms of Use
- `dando/beta.html` — Dando Beta Test License Agreement (unlisted: not linked from
  the site, sent to invited testers by link)
- `dando/billing-return.html` — where Stripe checkout and the billing portal return
- `dando/wearables/index.html` — fallback page for the Meta glasses iOS Universal Link
  (`https://asukatechnologies.com/dando/wearables`, set in the Meta Wearables Developer
  Center); seen only when iOS does not open the app
- `.well-known/apple-app-site-association` — iOS Universal Link claim: lets Dando
  (`R4F328X67Y.com.asukatechnologies.dando`) open `/dando/wearables`. Published because
  `_config.yml` includes `.well-known` (Jekyll skips dot-folders otherwise). Must be
  served without redirects
- `dando/dando-logo.svg` — the app icon with rounded corners (wordmark at 52% of the
  width, 5% corner radius), drawn with the app repo's `scripts/brand-geometry.mjs`
- `dando/dando-icon.svg` — browser-tab icon, copied from the app repo's `brand/`
- `uprange/` — redirects to `dando/`, kept for links in older app builds
- `styles.css` — shared stylesheet (light/dark via `prefers-color-scheme`)

Plain static HTML/CSS, no build step. Served by GitHub Pages from the default
branch root.
