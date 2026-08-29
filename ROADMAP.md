# Roadmap

Forward-looking index of what this site serves, what is in flight, and what it
grows into. Keep rows short — the detail lives in the linked CHANGELOG entries.

**Status:** `✅ shipped` · `🚧 in progress` · `📋 planned` · `💭 discussed, not scheduled`

**Priority:** what to reach for next, keyed to the one event this site is
waiting on — Grispy's publication to the Chrome Web Store and addons.mozilla.org.

- `P1` — **must be true before a store listing points here.** A listing's URLs
  are entered once and are awkward to correct afterwards, and a reviewer reads
  these pages before anyone else does.
- `P2` — real, but publication neither helps nor hurts.
- `P3` — whenever. No effect on a reader who arrives today.

A page here is small enough to need no spec or plan of its own, so the Record
column points at the CHANGELOG entry that describes what shipped — or, for a row
whose substance is wording rather than a page, at the section of
[`docs/copy.md`](docs/copy.md) that settles it.

## Pages

| # | Page | Status | Priority | Record |
|---|---|---|---|---|
| 1 | **Landing page** — what Grispy is in the reader's own terms, and the claim that nothing leaves their computer. Shipped; it stands in for a product page until there is something to sell. | ✅ | — | [changelog](CHANGELOG.md) Added |
| 1b | **Landing page rewritten against the settled copy** — the live page buries its strongest claim below the fold, never mentions encryption at rest, and promises to refill "the whole thing", which a wizard that hides its earlier steps falsifies. The replacement wording and the corrections owed are written; what remains is the edit. | 📋 | P1 | [copy](docs/copy.md) §3, §7 |
| 2 | **Privacy policy** — the public, stable URL both stores require on their listing forms, written so a reader can check it rather than trust it. Shipped; §2 now describes encryption at rest. | ✅ | — | [changelog](CHANGELOG.md) 2026-08-28 |
| 3 | **Support page** — one address for bugs, questions and ideas, and a plain statement that support is best effort on a free product written by one person. Shipped; linked from the landing page, both footers and §10 of the policy. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-08-28 |
| 3b | **"Free to everyone" on the support page** — the page promises no paid tier while the policy leaves a licence open at §7, so one of the two has to move before a reader can quote either back. Blocked by the price decision row 6 records. | 💭 | P1 | [copy](docs/copy.md) §1 |
| 4 | **Store links on the landing page** — the Availability section promises the Chrome Web Store and addons.mozilla.org links and currently carries neither, so the page tells a visitor to come back without saying when. Blocked by the extension's publication. | 💭 | P1 | — |
| 5 | **Product page** — the landing page is a single screen of prose, which is the right size for a thing nobody can install yet. Absorbs the feature breakdown, screenshots and FAQ rather than letting each become its own row; nothing beyond that is decided. | 💭 | P3 | — |
| 6 | **Payment provider named in the policy** — §7 already promises to name the provider here if a licence is ever sold, since the payment would be handled under that provider's own privacy policy rather than this one. Nothing to name yet. | 💭 | P2 | — |
| 6b | **The pages selling requires** — terms of service, a right-of-withdrawal and refund policy, trader identification, and a page carrying the price. None exists, and the extension's proprietary licence is in a private repository, so there is no public terms document at all. One row because they arrive together or not at all; it splits the day the price question settles. | 💭 | P1 | [copy](docs/copy.md) §1 |
| 8 | **A 404 page** — a mistyped or stale URL lands on GitHub's own generic 404, which reads as a broken site rather than a wrong address. A store listing's URLs are typed once and are awkward to correct afterwards, which is the case for having one before a listing points here. | 💭 | P2 | — |
| 9 | **User guide** — `docs/guide/multi-step-forms.md` in the extension repository is already written for a user rather than a developer, and no user can read it: that repository is private. Open, and worth settling before the page exists: whether the site becomes the public source or renders a copy the extension repository still owns. | 💭 | P2 | — |

**Four pages this site will not have, recorded so the question is not reopened:**
a cookie notice, because there are no cookies and claiming one would contradict
the no-network promise every other page makes; an accessibility statement, which
no obligation here reaches; a release-notes page, since both stores carry release
notes of their own; and a vulnerability-disclosure page, which the one support
address already covers.

## Copy

Words rather than pages. Nothing in this section is served; it is where a claim
is settled and checked before it reaches a page or a store's submission form.

| # | Item | Status | Priority | Record |
|---|---|---|---|---|
| 7 | **Listing and landing copy** — the words Grispy is described in, kept in one place so the landing page, both store listings and the Chrome Web Store's data-usage form cannot drift apart. Shipped as a source document with a claims-check table; every claim in it names where it was verified. | ✅ | — | [copy](docs/copy.md) |
