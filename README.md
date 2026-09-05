# QuietRate public website — v1

Static, dependency-free pre-release website for `quietrate.app`.

QuietRate 1.0 is in TestFlight/internal pre-release testing and is not yet publicly available on the App Store.

## Pages
- `/` — product landing page
- `/privacy/` — pre-release privacy policy
- `/support/` — support and contact
- `/sources/` — source and methodology transparency

## V1 production source architecture
- Production source architecture is frozen as **European Central Bank (ECB) + Taiwan Futures Exchange (TAIFEX)**.
- ECB reference-rate observations are retrieved through `api.frankfurter.dev` with the provider explicitly pinned to `ECB`.
- Frankfurter is transport/API infrastructure for the ECB path, not the source institution.
- TWD uses TAIFEX Daily Foreign Exchange Reference Rates.
- Cross rates that require observations from both source families are calculated by QuietRate and must remain identified as derived.
- Effective date and retrieval time are distinct concepts and must not be conflated.

## Technical and brand choices
- No JavaScript
- No external fonts
- No analytics or tracking scripts
- No cookies set by QuietRate
- No live, real-time, or most-accurate rate claims
- No App Store badge before public App Store availability
- Responsive, semantic HTML and keyboard-visible focus behavior
- QuietRate deep navy `#08192D`
- Official Q geometry and production `[Q]uietRate` lockup are locked
- Production lockup asset: `assets/brand/QuietRate-Lockup-Integrated-Dark.svg`
- Optical favicon asset: `favicon.svg`
- PNG favicon fallbacks: `favicon-16x16.png`, `favicon-32x32.png`, `favicon-48x48.png`
- Apple touch icon: `apple-touch-icon.png`

## Deployment
Established deployment is GitHub Pages from the existing repository and `main` publication root, with `quietrate.app` as the custom domain. `CNAME` and `.nojekyll` are included.

Do not change DNS, domain ownership, hosting provider, or deployment architecture without explicit owner approval.

## Release-content maintenance
The current public source, methodology, attribution, and privacy wording reflects the frozen V1 production configuration.

Re-review these pages if the production source architecture, source terms, privacy practices, or App Store release state changes. Do not change, add, substitute, or broaden production providers without explicit owner approval.

Do not add an App Store download badge or link until the app is publicly available.
