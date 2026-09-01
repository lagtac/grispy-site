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
| `support/index.html` | `/support/` | **The support page.** Both stores' listing forms take a support URL alongside the privacy one; this is that URL. States the single contact address and that support is best effort on a free, one-person product. |
| `.nojekyll` | — | Serve the files as written; skip GitHub's Jekyll build. |
| `ROADMAP.md` | — | What the site serves now and what it grows into. Rows link to the CHANGELOG entry that records them. |
| `CHANGELOG.md` | — | What changed on these pages, and the **Publication Contract**: the URLs a store listing will hold, and the announcement §9 of the policy owes before a protection narrows. |
| `guide/` | `/guide/` | **The user guide.** One page per topic, plus an index. The source, not a mirror: the extension repository keeps no copy — see `ROADMAP.md` row 9 for why, and rows 9/9b for what is written and what is not. |
| `docs/` | — | **Copy, not pages.** `docs/copy.md` holds the words Grispy is described in — landing page, both store listings, and the claims-check table each one is verified against — so those surfaces and the Chrome Web Store's data-usage form cannot drift apart. Serves nothing; a source document. |

## Editing the privacy policy

The policy makes factual claims about the extension's behaviour. Each one is checkable,
and each was checked before publication:

- **"makes no network requests"** — neither `src/` nor a freshly built `dist/` contains
  `fetch(`, `XMLHttpRequest`, `WebSocket`, `sendBeacon` or `EventSource`. Rule 8 of the
  extension repository's `scripts/check.js` enforces this over `src/`, but **`pnpm check`
  is a separate command from `pnpm build` and there is no CI running it** — so re-verify
  by hand before each release rather than assuming the build caught it. The policy
  deliberately claims only the checkable fact, not the process.
- **"never uses sync storage"** — every storage call in the extension is
  `chrome.storage.local`.
- **"no package is installed and nothing is fetched at runtime"** — the extension has no
  runtime dependencies. It is *not* true that no third-party material ships: the icon path
  data is vendored under ISC and MIT. The policy was corrected on 28 August 2026 to claim
  only the first, which is the part that bears on privacy.
- **"can be encrypted with a passphrase only you know"** — encryption at rest shipped, and
  §2 was rewritten in the same window to describe it along with its four limits. The one to
  keep checking is that the readable part stays as small as §2 says: the addresses Grispy
  holds data for, and nothing else.

**If the extension's behaviour changes, this page changes first.** A privacy policy that
overstates what the software does is worse than no policy, and the Chrome Web Store's
data-usage disclosure form must agree with it exactly.

## Deployment

Pushing to the default branch publishes the site. There is no build step.
