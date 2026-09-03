# Changelog

All notable changes to the pages this repository serves are documented here.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Reformatting, whitespace passes and anything else a reader of the pages cannot
see is not recorded.

There is no release step here: pushing to `main` publishes. `[Unreleased]`
therefore means *live, but not yet pointed at* — everything below is already on
the web, and the boundary it is measured against is the moment a Chrome Web
Store or addons.mozilla.org listing starts sending people to these URLs.

## [Unreleased] — 2026-09-02

### Publication Contract

This site has no operators to deploy it. What replaces the usual deployment
contract is the set of URLs other systems will hold, and the promises the pages
themselves make.

- **`/privacy/` and `/support/` are typed into store listing forms.** Both the
  Chrome Web Store and addons.mozilla.org take a privacy-policy URL, and both
  take a support or homepage URL. Once a listing is live, renaming or moving
  either path 404s a link that is no longer ours to fix from here — the listing
  has to be edited to match. Add pages freely; do not move those two.
- **A change that narrows the protections the policy states must be announced
  in the extension's release notes before the version making it ships.** §9 of
  the policy promises exactly that. It is a sequencing obligation spanning two
  repositories — the change lands here, the announcement lands in the
  extension's release notes — and nothing but this bullet records it.
- **The policy's effective date is its version number.** Any edit to
  `/privacy/` moves the date in the line under the heading, and a store
  reviewer checking a listing's data-usage disclosure against the policy is
  matching that date.
- **`.nojekyll` stays.** It is what makes Pages serve these files as written
  instead of running a Jekyll build over them.

### 2026-09-03 — Licence terms, and the price question closed (Roadmap #6b)

`docs/copy.md` §1 had held the price open since the file was written, under the
heading *One open decision: price*, and instructed every page to say nothing
until it closed. It is closed. The extension repository's revenue model settles
three tiers — Free at €0, Pro at €9 a month, Team at €10 per person — and §1 is
now the public half of that decision: the tier table the pages take their wording
from, and four things that may never be said.

The three that matter most, because each is a promise that is expensive to
retract:

- **Never "Grispy is free" unqualified.** It is free *for personal use*. That
  unqualified form is exactly the debt §7's item 4 exists to pay off, and
  repeating it anywhere rebuilds it.
- **Never imply the free tier is a trial or a demo.** It does not expire and it
  does not count anything. The seven-day clock applies only to the paid
  capabilities layered on top of it.
- **Never describe how the licence is checked.** The terms say what a licence
  covers; the mechanism is not a selling point and not the reader's problem.

**`/terms/` is live, and it carries no price.** It was first written to be held
back on row 2b's reasoning — a page describing what the extension cannot do yet.
That reasoning was overridden deliberately: the page states what a licence
*covers*, not what it costs, and no price appears on this site until row 6e's
page is written and §1.3's gates are closed. It is linked from every footer.

What the page says, beyond the tier table: free is the whole product rather than
a trial of it; a licence is granted to people rather than to computers; paying
changes nothing about the network position, because there is no account, no login
and no server, and the privacy policy is the same document for a paying customer
as for anyone else. The last section states the consequence plainly — we cannot
recover anything from an installation we cannot see, and paying does not change
that.

**Row 6b splits, as it always said it would.** It named four things selling
requires and treated them as one row because they arrive together; with the price
settled they no longer do. Terms are written (6b). A right-of-withdrawal and
refund policy is undecided and is a checkout-flow question as much as a page
(6c). Trader identification is blocked on the sole proprietorship existing, since
there is nothing yet to identify (6d). A page carrying the price is unwritten
(6e). And the two live pages that said "free" without qualification are
corrected in this same change rather than a later one (6f) — publishing a terms
page that requires a licence for commercial work, beside a support page promising
there is no paid tier, would have left the site contradicting itself. Both now
read *free for personal use*; neither carries a price.

### 2026-09-02 — The policy covers global presets (Roadmap #2b)

The extension's spec for global presets lists exactly one blocking dependency,
and it is this page: the policy has to change before any of that code is
written. The reason is that a global preset is a different kind of record from
anything Grispy has stored before. A saved form holds **your**
answers to a form. A global preset holds a named set of facts about a subject who
may not be you — a client, a colleague, an applicant, a customer — and the people
whose names, tax numbers and passport numbers end up in one never installed
anything and cannot be asked here.

Four edits, none of which narrows a protection:

- **§1 gains global presets as a second thing Grispy stores**, stated separately
  from saved form values rather than folded into them, and says outright that a
  preset may hold someone else's details. The point of the feature is that it
  usually will.
- **§2's list of limits goes from four to five.** The roster first went into the
  existing "conceals what you saved, not which sites" bullet and read as two
  limits stitched together, because they are two: which sites you saved on is a
  readable list by design, whereas a global preset has no readable list at all —
  its *name* sits inside the encrypted record with its contents, deliberately,
  since a plaintext index of other people's names is the thing most worth
  protecting. All a reader of your files can work out is how many you have. It is
  now its own bullet, and the declining-the-passphrase limit names global presets
  too, since that is the choice that leaves identity records readable on disk.
- **§6 says an export of everything carries the roster.** The support page already
  asks people not to attach exports to bug reports; that request stops being
  hygiene the moment the file can contain a third party's passport number, so the
  policy now says so and links to it.
- **§7 gains the paragraph this feature really needs.** Our own GDPR position is
  unchanged and unchangeable — the data never reaches us. The user's position is
  not: someone holding clients' personal data in Grispy may carry a controller's
  responsibilities for it, and we cannot carry them on their behalf. The paragraph
  says that, and declines to give legal advice about it.

**§9's release-note gate does not fire.** It promises an announcement before any
change that *narrows* the protections stated here. Nothing narrows:
`globalpreset:` joins `form:` and `formpreset:` in the extension's encrypted
prefixes on the same terms. What changed is that a new category of data is
described, which that gate does not cover.

**This is committed, not published.** Pushing is what publishes, and the page now
describes a feature nobody can use yet. The push belongs beside the extension
shipping ROADMAP row 16 — and the effective date, which this repository treats as
the policy's version number, wants re-dating to that day rather than to this one.

### 2026-09-02 — The landing page says what the settled copy says (Roadmap #1b)

`docs/copy.md` §3 has held the landing page's replacement wording since
2026-08-29, and §7 has listed three things the live page said that the wording
did not support. The page is now rewritten against §3, and all three are
discharged.

- **"Refills the whole thing" is gone.** The multi-step claim was true in its
  first half and overclaiming in its second: a wizard that hides its earlier
  steps is not followed, and rich-text editors, shadow-DOM fields and custom
  pickers are not reached at all. The capability now sits under *What it does
  that autofill does not* with its edge stated, and the hidden-step wizard is
  named outright as a limit.
- **The no-network claim moved above the fold.** It was in a box below a
  heading, three sections down. It is the strongest thing on the page and the
  only claim a reader can check *before* installing, so it is now the second
  paragraph, ahead of every heading, and it carries the no-standing-access
  sentence with it.
- **Encryption at rest is mentioned at last.** It shipped on 2026-08-28 and the
  landing page never learned about it, so a reader comparing this page to the
  policy found the policy describing a protection the page did not know it had.
  The §3 wording is used exactly — *can be* encrypted, never *is* encrypted,
  because the user is asked once and may decline.

**Two sections the page never had.** *Who it is for* names the four situations
Grispy is worth having, and says plainly that someone who fills a form once
should not install it. *What it cannot do yet* lists five limits, including the
cold start — `docs/copy.md` §2 treats that one as the mechanic rather than an
apology, on the grounds that hiding it earns "doesn't work" reviews from people
who pressed Fill on a fresh page.

- **The last user-facing "profile" on the site is gone.** The meta description
  still described "named profiles you switch between"; the extension renamed
  that concept to a form preset on 2026-08-28 and the policy was swept the same
  week. The description is now §4's short-description wording, which is settled
  and already checked.
- **The page adopts the stylesheet the other nine pages share** — 44rem,
  `.lede`, the rule above each `h2`, list spacing. It was the last page still
  carrying the original block, and it now needs list styling it never had. The
  oversized `h1` and the larger tagline are kept: it is the front door. The
  disabled border on the old `.box` rule went with the rule; nothing was
  corrected in place.
- **"Grispy is free and is written by one person" was left untouched.**
  `docs/copy.md` §7 blocks the support page's "free to everyone" on the
  unsettled price question and does not list this sentence, so the rewrite kept
  it as it stands and added no second instance of the word.

### 2026-09-01 — The multi-step guide is published, and the copy is gone (Roadmap #9)

The sixth page. `/guide/multi-step-forms/` was written months ago for a user
and lived in the extension's private repository, where no user could read it.

- **Both halves in one change**, as row 9 required: the page is served here and
  the extension repository's copy is deleted. There is one copy, not two, which
  is the whole point of the decision recorded in `ROADMAP.md`.
- **One stale line corrected on the way.** The guide told readers that detached
  page data is listed on the **Manage** screen. The options page stopped being
  called Manage on 2026-08-28, when it became four tabs called Settings, and the
  guide was never swept. It now names Settings and links to that guide page.
- **Three things did not survive the port**, all of them links into a private
  repository: the "Shipped" banner citing extension roadmap rows, a link to
  ROADMAP.md in Known limits, and the trailing note deriving the page from two
  specs. A public page cannot cite documents its readers cannot open.

### 2026-09-01 — A user guide, at `/guide/` (Roadmap #9b)

Grispy had exactly one page of user documentation, it covered multi-step
wizards, and it lived in a private repository where no user could read it. Five
pages now cover the rest, with an index at `/guide/` linked from every footer.

- **`/guide/saving-and-filling/`** — the core loop. Save a form under a name,
  keep several sets of answers against it, switch, fill. Also every screen the
  popup can show and how values appear in the save list.
- **`/guide/what-a-fill-reports/`** — the page this set existed for. `docs/copy.md`
  §3 and §4 were ungated the same day and now advertise that Grispy "tells you
  what it could not confirm", with nothing anywhere explaining the two sentences
  a fill actually shows.
- **`/guide/passphrase/`** — what encryption covers, what it leaves readable, and
  that a forgotten passphrase is unrecoverable. The four limits are lifted
  verbatim from policy §2 rather than reworded, per rule 1 of `docs/copy.md`.
- **`/guide/settings/`** — the inventory, every deletion, export and import, and
  the reset that works while locked.
- **`/guide/repeating-rows/`** — add-a-row forms, the question asked before rows
  are dropped, and the position-matching limit that makes *Save just these* the
  safer answer after a mid-list deletion.

Two things about how these were written, both worth keeping:

- **Every quoted string was read out of the extension's source, not recalled.**
  That caught the error this row was first written on: ROADMAP row 9b originally
  said the guide must explain `filled`, `not-found`, `refused` and `unverified`.
  There are five such constants rather than four, and a user is shown none of
  them — `not-found`, `refused` and `unchanged` fold into one denominator, so
  the pages state that limit instead of teaching names the popup withholds.
- **`docs/copy.md` §6 now covers `/guide/` as well.** Nine rows record the
  load-bearing guide claims and where each was verified. The guide is a fourth
  surface making checkable claims about extension behaviour, at higher density
  than the landing page, and nothing was tracking it.

These five shipped before the multi-step page, which is why the index briefly
said that one was coming. Row 9 landed the same day and the index now lists all
six.

### 2026-08-28 — A support page, and the one address behind it (Roadmap #3)

Until now the only way to reach anyone was §10 of the privacy policy, which
names an address for privacy enquiries — so a bug report had to be filed under
a heading that does not cover it. `/support/` is now that heading, and the
landing page, both footers and §10 point at it.

- **One channel: email.** No contact form, no chat widget, no forum. A form
  would have to route a message through somebody else's server to reach us,
  which is the one thing every other page here promises does not happen. The
  page says so rather than leaving it to be noticed.
- **The offering is stated as it is** — free to everyone, no paid tier, written
  by one person, best effort. No response time is promised, because none can be
  kept.
- **It pre-empts the two requests that cannot be granted:** a forgotten
  passphrase is unrecoverable, and deletion is final. Both link to §2 of the
  policy, which now carries an `id` so the link lands on the passage rather
  than the top of the document.
- **A bug report has to carry what the software cannot send.** Grispy has no
  crash reporting or telemetry, so the page asks for browser, version, the
  form, the clicks and the outcome — and asks that saved data and export files
  are *not* sent, since those hold exactly what the extension is built never to
  transmit.

### 2026-08-28 — The policy describes encryption at rest, and withdraws two claims (Roadmap #2)

The extension can now encrypt saved form data behind a passphrase, so §2 says
so — and says the four things a reader needs in order to decide whether to rely
on it. Two claims elsewhere in the policy had quietly stopped being true and
were corrected in the same pass, since this document's whole value is that a
reader can check it rather than trust it.

- **§2 gained "Encryption, and why it is your choice".** Encryption is offered
  once and can be declined, the passphrase is entered once per browser session
  and never written to disk, and a forgotten passphrase is unrecoverable by
  anyone, us included.
- **The limit that matters most is stated rather than footnoted:** encryption
  conceals what you saved, not which sites you saved it on. Grispy has to answer
  "does this page have anything saved for it" without prompting on every page
  you visit, so the list of addresses it holds data for is deliberately left
  readable.
- **"No third-party code" is gone from the lede, and "all of its code is our
  own" from the §3 table.** Neither holds now that icon path data is vendored
  under ISC and MIT. Both now claim what still does hold: no package is
  installed and nothing is fetched at runtime.
- **§5 offered two ways to check the policy without trusting it; there are now
  three.** The encryption is the browser's own WebCrypto, so there is no
  cryptographic code of ours for a reader to have to audit.
- **The effective date moved to 28 August 2026,** as §9 requires of any change.

### Added

- **The site.** A landing page at `/`, and the privacy policy at `/privacy/` —
  the public, stable URL that both the Chrome Web Store and addons.mozilla.org
  require on their listing forms. Grispy's source is not in this repository; it
  is private and proprietary, and this repository is public only so that Pages
  can serve it.
- **§10 of the policy names a contact address** for questions about the policy
  and about Grispy's handling of data. A policy that describes rights without
  saying where to exercise them is incomplete.

### Changed

- **The policy no longer claims the build refuses to complete when a network
  primitive is added.** It does not: `pnpm build` runs typecheck and Vite, never
  `scripts/check.js`, and there is no CI — so that rule is a manually-run gate
  over `src/`, not a property of the shipped artifact. The underlying fact was
  verified live and still holds, so the reader-checkable bullet stays and only
  the process claim is gone. A policy that overstates what the software does is
  worse than no policy.
