# QuietRate public website — v1

Static, dependency-free pre-release website for `quietrate.app`.

## Pages
- `/` — product landing page
- `/privacy/` — pre-release privacy policy
- `/support/` — support and contact
- `/sources/` — source and methodology transparency

## Technical choices
- No JavaScript
- No external fonts
- No analytics or tracking scripts
- No cookies set by QuietRate
- No production-provider claims
- No App Store badge before release
- No app-icon asset because the icon is not final
- Responsive, semantic HTML and keyboard-visible focus behavior
- QuietRate deep navy `#08192D`

## Deploy
Deploy as-is to GitHub Pages, Cloudflare Pages, Netlify, Vercel static hosting, or a conventional web server.

For GitHub Pages, place these files at the publication root, enable Pages, set the custom domain to `quietrate.app`, and configure DNS according to GitHub's current instructions. `CNAME` and `.nojekyll` are included.

## Before App Store release
Re-review and update:
- production data-provider identity and attribution
- licence/source obligations
- provider-related privacy disclosures
- App Store Privacy answers
- Sources & Methodology production content
- all pre-release notices
- App Store download badge/link
- final app icon/social preview artwork

Do not publish a provider name or rights claim until that provider has actually been approved.
