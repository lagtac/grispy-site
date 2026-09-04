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
| 1b | **Landing page rewritten against the settled copy** — the live page buried its strongest claim below the fold, never mentioned encryption at rest, and promised to refill "the whole thing", which a wizard that hides its earlier steps falsifies. Shipped as [`docs/copy.md`](docs/copy.md) §3 poured out: all three §7 corrections are struck, and the page gained two sections it never had — who it is for, and what it cannot do yet. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-09-02 |
| 1c | **Three live surfaces said Grispy has nothing to offer on a form you have not saved** — the landing page, the guide's opening page and the Chrome listing copy all carried it, and the extension's roadmap row 16 falsified all three on 2026-09-04. This is row 6g's mistake in the other direction: there the site got ahead of the software, here the software got ahead of the site, which is the safer error and still drift. The section note above takes the rule from the privacy policy — *when behaviour changes, the page here changes first* — and it was not followed. Corrected the same day; the screenshots it also invalidated are not retaken and are held in [`docs/copy.md`](docs/copy.md) §8. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-09-04 |
| 2 | **Privacy policy** — the public, stable URL both stores require on their listing forms, written so a reader can check it rather than trust it. Shipped; §2 now describes encryption at rest. | ✅ | — | [changelog](CHANGELOG.md) 2026-08-28 |
| 2b | **The policy covers global presets** — a global preset holds facts about a subject who may not be the user, so the roster can carry third parties' names, tax numbers and passport numbers; §1, §2, §6 and §7 all needed real edits rather than an appended bullet, and §7's is the one the feature really needs: the user may themselves be a controller for data we can never see. Written and pushed on 2026-09-02, ahead of the code, which left the served policy describing a feature no released build had — the same defect row 6g corrected on `/terms/`, and milder only because a policy that over-describes what is stored errs safe. **Closed 2026-09-04**, when the extension's roadmap row 16 shipped and the policy was corrected for what the feature turned out to do: it categorises what a value *is*, which §2 had promised it does not, and it never named the store that holds the details a user adds. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-09-04 |
| 3 | **Support page** — one address for bugs, questions and ideas, and a plain statement that support is best effort on a free product written by one person. Shipped; linked from the landing page, both footers and §10 of the policy. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-08-28 |
| 3b | **"Free to everyone" on the support page** — the page promised no paid tier while the policy left a licence open at §7, so one of the two had to move before a reader could quote either back. **Closed 2026-09-03 by row 6g.** The decision it waited on is made: the first release is free and nothing can be bought, so the page says *free* plainly — without the *with no paid tier* clause, which a licence announced as coming would contradict a second time. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-09-03 |
| 4 | **Store links on the landing page** — the Availability section promises the Chrome Web Store and addons.mozilla.org links and currently carries neither, so the page tells a visitor to come back without saying when. Blocked by the extension's publication. | 💭 | P1 | — |
| 5 | **Product page** — the landing page is a single screen of prose, which is the right size for a thing nobody can install yet. Absorbs the feature breakdown, screenshots and FAQ rather than letting each become its own row; nothing beyond that is decided. | 💭 | P3 | — |
| 6 | **Payment provider named in the policy** — §7 already promises to name the provider here if a licence is ever sold, since the payment would be handled under that provider's own privacy policy rather than this one. Nothing to name yet. | 💭 | P2 | — |
| 6b | **Licence terms** — the page saying what is free, what a licence covers and what it does not, at `/terms/`. Shipped. It carries no price: prices wait for row 6e and the gates [`docs/copy.md`](docs/copy.md) §1.3 names. Its wording is §1 of that file poured out. **Withdrawn by row 6g the following day** — what it published was true of a planned product, not of the one that ships. The ✅ stands: it records what was genuinely published. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-09-03 |
| 6c | **Right of withdrawal and refund policy** — an EU distance sale carries a fourteen-day withdrawal right. Digital content can be excepted, but only where the buyer expressly consents and acknowledges losing it, so this is a checkout-flow requirement as much as a page. Undecided; [`docs/copy.md`](docs/copy.md) §1.3 records why it is not a decision that document can make. | 💭 | P1 | [copy](docs/copy.md) §1.3 |
| 6d | **Trader identification** — a trader selling into the EU must name itself: legal name, address, contact and tax registration. Blocked on the sole proprietorship existing; there is nothing to identify yet. | 💭 | P1 | [copy](docs/copy.md) §1.3 |
| 6e | **A page carrying the price** — the three tiers side by side with what each includes. The prices are settled and the page is not written; it is also the page a store listing's paid-gate disclosure will point at. | 💭 | P1 | [copy](docs/copy.md) §1.1 |
| 6f | **Two live pages said Grispy is free without qualification** — the support page's "free to everyone, with no paid tier" and the landing page's "Grispy is free". Both now read *free for personal use*. Shipped with row 6b rather than after it: a terms page requiring a licence for commercial work, published beside a support page promising no paid tier, contradicts itself. **Reversed by row 6g the following day**, once the terms page it was made to agree with was itself withdrawn. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-09-03 |
| 6g | **The licence terms are withdrawn** — rows 6b and 6f published a page stating that work use needs a paid licence, describing Pro and Team licences, and promising that paid features stop seven days after install. None of it exists in the extension, and `LICENSE` grants every installer commercial use for nothing, so the page contradicted the software it governs. `/terms/` is rewritten rather than removed, because four footers link it: the work-use requirement, the tier table and the trial section are gone, *free for personal use* reverts to plain *free* on all three pages, and one new section says that capabilities for professional use are being built and will need a licence — no prices, no named paid features, no dates. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-09-03 |
| 8 | **A 404 page** — a mistyped or stale URL lands on GitHub's own generic 404, which reads as a broken site rather than a wrong address. A store listing's URLs are typed once and are awkward to correct afterwards, which is the case for having one before a listing points here. | 💭 | P2 | — |
| 9 | **Guide: forms that span several pages** — multi-step wizards: the line saying which step Grispy thinks you are on, the click that corrects it, and the two kinds of wizard it cannot follow. Shipped as the port the note below settled, both halves in one change — the page is served here and the extension repository's copy is deleted, so there is one copy rather than two. A stale line was corrected on the way: it still called the options page **Manage**, which it stopped being on 2026-08-28. | ✅ | P2 | [changelog](CHANGELOG.md) 2026-09-01 |
| 9b | **The rest of the guide** — row 9 moved the only page that existed. Shipped as five more: the core loop, what a fill reports, the passphrase, the Settings page, and repeating rows, behind an index at `/guide/`. What a fill reports is the one it existed for — [`docs/copy.md`](docs/copy.md) §3 and §4 advertise that Grispy "tells you what it could not confirm" and nothing explained the two sentences it shows. Every quoted string was read out of the extension's source, which is what caught this row's own first draft naming four outcome constants a user is never shown. | ✅ | P2 | [changelog](CHANGELOG.md) 2026-09-01 |
| 9c | **Guide: details that fit any form** — the extension's roadmap row 16 shipped a whole user-facing surface on 2026-09-04 and the guide covered none of it: a second row of chips, a picker, a reviewed learn-from-this-page list, a line stating what a fill will write, and a fifth Settings tab. Shipped as a seventh page plus corrections to three existing ones. It carries the hazard nothing on screen reports after the fact — filling a set of details and then a form's own preset writes one subject's name over another's — and states the safe order. | ✅ | P1 | [changelog](CHANGELOG.md) 2026-09-04 |

**Where the user guide lives, settled 2026-09-01 (row 9).** This site is the
source. The extension repository does not keep a copy, and nothing renders one
across the boundary.

Three things decided it. **The repository boundary is the rule everywhere else:**
anything a user or a store reviewer has to read is public-facing and lives here,
because the extension repository is private — that is what makes a guide there
unreadable by the only people it is written for. **A mirror would be a manual
copy**, since Pages serves these files as written and there is no build step to
render one; the same shape produced two listing-copy documents that disagreed
within three days, which is the drift this decision exists to avoid. **And the
guide's readers are here already** — a store listing sends people to `/support/`,
not into a repository.

The cost is real and belongs on the record: the guide describes extension
behaviour, and extension behaviour changes in the *other* repository. That is
the coupling the privacy policy already carries, and it takes the same rule —
**when behaviour changes, the page here changes first.** The extension's
`CLAUDE.md` names the policy in that rule; the guide joins it.

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
