# QuietRate website implementation handoff

This repository is the approved QuietRate V1 pre-submission website baseline. Preserve these constraints:

## Brand and visual
- Public brand: QuietRate
- Domain: https://quietrate.app
- Visual direction: deep navy (#08192D), restrained azure, calm premium iOS utility
- Official Q geometry is locked; do not redraw, regenerate, or reinterpret it
- Primary integrated lockup is `[Q]uietRate`, production-final, using the supplied outlined SVG asset
- Website dark-background lockup: `assets/brand/QuietRate-Lockup-Integrated-Dark.svg`
- Favicon geometry is optical-size specific; preserve the supplied `favicon.svg`
- Preserve the approved PNG favicon fallbacks: `favicon-16x16.png`, `favicon-32x32.png`, `favicon-48x48.png`
- Preserve the approved `apple-touch-icon.png`
- Footer may remain text-only unless a separate footer-lockup decision is explicitly approved

## V1 production rate architecture
- Production V1 source architecture is frozen as **ECB + TAIFEX**
- Do not change, add, substitute, or broaden providers without explicit owner approval
- European Central Bank (ECB) reference exchange rates are the source observations for the ECB side of the shipping catalog
- `api.frankfurter.dev` is transport/API infrastructure for ECB-pinned observations, not the source institution
- ECB-path requests must remain explicitly pinned/filtered to `ECB`; do not describe or substitute Frankfurter's default blended rates as the V1 source
- TWD source observations come from Taiwan Futures Exchange (TAIFEX) Daily Foreign Exchange Reference Rates
- QuietRate-derived cross rates must remain identified as QuietRate-derived and must not be attributed to ECB or TAIFEX
- Effective date means the source calendar date to which an observation applies; retrieval time means when QuietRate obtained it
- Local caching must not change source values, effective dates, or provenance

## Legal, privacy, and release boundaries
- Do not claim live, real-time, most-accurate, executable, guaranteed, or tradable rates
- Do not imply ECB, TAIFEX, Frankfurter, or any government agency endorses QuietRate
- Use factual text attribution; do not add ECB or TAIFEX logos
- Do not add analytics, tracking, external fonts, or cookies without explicit approval
- Do not add JavaScript unless separately approved and necessary
- Do not add an App Store badge or download link before the app is publicly available
- QuietRate 1.0 may be described as pre-release, in TestFlight/internal testing, or coming to the App Store; do not describe it as publicly released
- Keep `/privacy/`, `/support/`, and `/sources/` stable URLs
- Support contact: support@quietrate.app

Re-review source/legal/privacy content if the production architecture, source terms, privacy practices, or public-release state changes.
