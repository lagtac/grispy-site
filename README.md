# grispy-site

The public web pages for **Grispy**, a Chrome and Firefox extension that saves and
refills web forms.

This repository is public **only** so that GitHub Pages can serve it. Grispy's source
code is not here and is not open source — it lives in a private repository and is
covered by a proprietary licence.

## What is here

| Path | Serves | Why it exists |
|---|---|---|
| `index.html` | the site root | Landing page. Grows into the product page when there is something to sell. |
| `privacy/index.html` | `/privacy/` | **The privacy policy.** Both the Chrome Web Store and addons.mozilla.org require a public, stable privacy-policy URL on the listing form. This is that URL. |
| `.nojekyll` | — | Serve the files as written; skip GitHub's Jekyll build. |

## Editing the privacy policy

The policy makes factual claims about the extension's behaviour. Each one is checkable,
and each was checked before publication:

- **"makes no network requests"** — the built bundle contains no `fetch(`,
  `XMLHttpRequest`, `WebSocket`, `sendBeacon` or `EventSource`. Rule 8 of the extension
  repository's `scripts/check.js` fails the build if any appears in the source.
- **"never uses sync storage"** — every storage call in the extension is
  `chrome.storage.local`.
- **"no third-party code ships"** — the extension has no runtime dependencies.
- **"not encrypted at rest"** — true today, and deliberately disclosed. If on-disk
  encryption ships, §2 must be rewritten in the same release.

**If the extension's behaviour changes, this page changes first.** A privacy policy that
overstates what the software does is worse than no policy, and the Chrome Web Store's
data-usage disclosure form must agree with it exactly.

## Deployment

Pushing to the default branch publishes the site. There is no build step.
