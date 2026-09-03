# Marketing copy

The words Grispy is described in, kept in one place so the landing page, the two
store listings, the Chrome Web Store's data-usage form and the pages under
`/guide/` cannot drift apart.

**The guide joined that list on 2026-09-01**, when its six pages shipped. They
are not marketing copy and their wording is not settled here — but they make
checkable claims about extension behaviour at far higher density than the landing
page does, which is exactly what [§6](#6-claims-check) exists to catch. The guide
rows in that table are the load-bearing ones: the messages a page quotes verbatim,
and the claims a user could be harmed by relying on.

Nothing here is served. This is a source document: copy is written and settled
here, then poured into `index.html` and into each store's submission form when
there is something to submit. Presentation is deliberately out of scope — no
markup, no layout, no decisions about what a page looks like.

## How to use this document

1. **The privacy policy is authoritative.** Where the policy already has a
   sentence for something — what encryption covers, what it does not, what
   happens to a forgotten passphrase — the copy borrows that sentence rather
   than inventing a second wording. A claim phrased three ways across three
   surfaces is a claim that will eventually disagree with itself, and the Chrome
   Web Store rejects a listing whose disclosure form contradicts its policy URL.
2. **Every factual claim has a row in [§6](#6-claims-check).** If a claim is not
   in that table, it is not ready to publish.
3. **[§8](#8-gates-before-submitting) is not for readers.** It lists what has to
   be fixed in the extension before any of this copy can honestly go up.
4. **Links are written as the destination needs them, absolute.** A store
   listing takes no relative path, so every link below is the full public URL.
   `index.html` is served from the site root and links to `privacy/` relatively
   today — shorten on paste rather than copying the absolute form into it.
   **The base URL is confirmed: `https://lagtac.github.io/grispy-site/`.**
   Checked on 2026-09-02 by fetching it — it served this repository's
   `index.html`, and `/privacy/`, `/support/` and `/guide/` each answered 200.
   That confirms the URL a store listing would be given actually resolves,
   which is what the listing needs; it is not a reading of the Pages settings
   panel, so a custom domain configured later would still change every link
   below, and this note with them.

---

## 1. Price, settled 2026-09-03 — **not publishable**

> **Bracketed 2026-09-03, the same day, and kept rather than deleted.** Every
> tier sentence below is settled and will be needed. None of it may reach a page
> yet: nothing in the extension can be bought, so a page describing what a
> licence covers describes software that does not exist. That is the mistake
> `/terms/` made — see [§7](#7-corrections-owed-to-live-copy) item 5 and roadmap
> row 6g. The reasoning is in the extension repository's private
> `docs/plans/2026-09-03-free-release-cut-spec.md`. **Read §1.2 before writing
> anything from this section: its first rule is now reversed.**

**The price question this section held open is decided.** What follows is the
wording every other surface takes from; nothing here may be paraphrased into a
page without matching it, because the promises below are the ones a reader will
quote back.

The decision itself, and the arithmetic behind it, is the extension
repository's `docs/product/2026-09-03-revenue-model.md`. That document is
private. This section is the public half of it, and it is deliberately shorter
than the decision it serves — a reader needs the terms, not the reasoning.

### 1.1 The three tiers, in the words the pages use

| Tier | The one sentence |
|---|---|
| **Free** | Grispy is free for personal use — every form, every preset, no limit and no account. |
| **Pro** | For one person using Grispy as part of their paid work. |
| **Team** | For a business, billed for the people who use it. |

**The figures are deliberately not written here.** This repository is public and
this file is served — `/docs/copy.md` returns 200 — so a price written in it is
a published price, and §1.2's rule against that applies to this file as much as
to any page. The amounts live in the extension repository's private
`docs/product/2026-09-03-revenue-model.md` §3 until the gates in §1.3 close, at
which point row 6e's page carries them and this table gains the column back.

~~**Paid features are free for the first seven days after installing**, then stop
until a licence key is entered.~~ **Not publishable, 2026-09-03.** There are no
paid features, no key to enter and no clock. This sentence was published on
`/terms/` and withdrawn the next day; see [§7](#7-corrections-owed-to-live-copy)
item 5.

### 1.2 What may not be said

- ~~**Never "Grispy is free" without qualification.** It is free *for personal
  use*.~~ **Reversed 2026-09-03.** The unqualified form is now the correct one,
  and this rule is what would put the wrong sentence back. Grispy is free for
  every use, including work: `LICENSE` grants it, and nothing exists to charge
  for. Restore the qualification only when a licence can actually be bought.
  **Also do not restore "with no paid tier"** — a paid tier is announced as
  coming, so that clause would be wrong in the other direction.
- **Never imply the free tier is a trial, a demo, or time-limited.** It is a
  complete product that does not expire. The seven-day clock applies only to
  the paid capabilities layered on top.
- **Never advertise how the licence is checked**, or that it is not enforced
  beyond the key. The terms state what a licence covers; they do not describe
  the mechanism.
- **Never let a price appear anywhere in this repository while §1.3's gates are
  open** — not on a page, and not in this file. A price is an offer; an offer in
  the EU carries a withdrawal right and an identified trader, which rows 6c and
  6d cover and which do not exist yet. The repository is public and `docs/` is
  served, so "not on a page" is not the boundary. **This rule was broken on
  2026-09-03 and repaired the same day**, which is why it now names the file it
  is written in.

### 1.3 What this does not settle

Three of the four things selling requires are still missing, and the price
wording above cannot ship without them — roadmap row 6b splits into 6b, 6c, 6d
and 6e for exactly this reason:

- **A right-of-withdrawal and refund policy.** EU consumer law gives a
  fourteen-day withdrawal right on distance sales; digital content can be
  excepted from it, but only where the buyer expressly consents and
  acknowledges losing the right, which is a checkout-flow requirement and not
  only a page. **Undecided, and not a decision this document can make.**
- **Trader identification.** A trader selling into the EU must identify itself:
  legal name, address, contact, and tax registration. **Blocked on the sole
  proprietorship existing** — there is nothing to identify yet.
- **The payment provider**, which roadmap row 6 says the privacy policy must
  name once money moves through it.

---

## 2. What Grispy is, in one paragraph

The frame that everything below is written against, recorded so a future edit
does not quietly drift off it:

> Grispy is not for filling a form you have never seen. Your browser's autofill
> and your password manager already do that, badly, from one stored identity.
> Grispy is for the form you fill **again** — where the value is not guessing
> what goes in the box, but remembering what you put there last time, and having
> more than one answer available.

Two consequences for the copy:

- **Never use the words "form filler" as the headline category.** It invites a
  comparison Grispy loses, on reach, in the reader's first two seconds.
- **The cold start is the mechanic, not an apology.** Grispy does nothing useful
  on first run. Copy that hides this earns "doesn't work" reviews from people who
  installed it, pressed Fill on a fresh page, and got nothing. Copy that leads
  with it — *save once, fill every time after* — sets the expectation correctly
  and costs nothing.

---

## 3. Landing page

Replaces the copy in `index.html`. Section headings are content, not layout
instructions.

**Poured into `index.html` on 2026-09-02** (ROADMAP row 1b). The live page and
this section now say the same thing; an edit to one is owed to the other.

### Headline

> **Grispy**
>
> Save a web form once. Fill it again in one click, as often as you need.

### Opening

> Your browser's autofill knows *you* — one address, one email, one card. Grispy
> knows the *form*, and holds as many different sets of answers against it as you
> need, each under a name you choose.
>
> Grispy asks for no standing access to any website. It has no account, no server and no
> analytics, and it makes no network requests of any kind. It runs on the page in
> front of you, only after you click it, and what it saves stays in your browser.

### Who it is for

> If you fill the same form over and over, with different answers each time:
>
> - the same application form, a different applicant every week
> - the same supplier or client onboarding, twelve suppliers deep
> - the same claim, booking or registration form, a new file each time
> - a five-step portal wizard you work through every month
>
> The more often you return to one form, the more Grispy is worth. If you fill a
> form once and never again, it is not for you.

### What it does that autofill does not

> - **Many answers per form.** Save as many named sets as you need against one
>   form and switch between them. Autofill has exactly one identity.
> - **Multi-step forms.** Grispy follows a form across the pages it spans and
>   fills each step as you reach it — including wizards that redraw themselves
>   without ever changing the address in the bar.
> - **The awkward controls.** Search-as-you-type dropdowns, tag pickers, and the
>   checkboxes and radios that modern web frameworks manage themselves are driven
>   the way a person would drive them, not written past. A value that looks filled
>   but that the page never registered is the failure Grispy is built to avoid: it
>   checks each field afterwards and tells you which ones it could not confirm.

### Your data stays yours

> What Grispy saves is written to your browser's own storage on your computer, and
> **can be encrypted with a passphrase only you know**. You are asked once, you can
> decline, and you can turn it on later.
>
> Encryption conceals what you saved, not which sites you saved it on.
>
> There is no sync: Grispy holds nothing on a server, so nothing follows you to a
> second computer on its own. You can export everything to a file and import it
> wherever you want it.
>
> [Read the privacy policy](https://lagtac.github.io/grispy-site/privacy/).

### What it cannot do yet

> Stated plainly, because finding out afterwards is worse:
>
> - **It starts empty.** Grispy has nothing to offer on a form you have not saved.
> - **It acts only when you click it.** No filling on page load, by design — it is
>   the same choice that lets it ask for no access to any site.
> - **Some fields it cannot see.** Rich-text editors, fields built inside a web
>   component's shadow DOM, and custom pickers with no ordinary form control
>   underneath are invisible to it.
> - **One kind of wizard defeats it.** A multi-step form that *hides* its earlier
>   steps instead of removing them looks like a single long form, and Grispy will
>   treat it as one.
> - **No sync, and no recovery.** A forgotten passphrase cannot be recovered, by
>   you or by us. Export while you can.

### Availability

> Grispy is not yet published. This page will carry the Chrome Web Store and
> Firefox Add-ons links when it is.

### Contact

Unchanged from the live page — one address, best effort, link to `/support/`.
See [§1](#1-price-settled-2026-09-03) before repeating "free" here.

---

## 4. Chrome Web Store listing

> **Character limits below are from memory and are not verified. Check each one
> against the live submission form before pasting.**

### Short description — target ~110 characters, cap believed 132

> Save a web form once, then fill it again in one click — many named sets of
> answers, multi-step wizards included.

### Detailed description

> **Grispy saves a web form the way you filled it, so you can fill it again.**
>
> Your browser's autofill knows you: one address, one email, one card. Grispy
> knows the form. Save it once under a name you choose, then bring those answers
> back in a single click — and keep as many different sets against the same form
> as you need.
>
> **It is built for the form you fill over and over:** the same application with a
> different applicant every week, the same onboarding for the twelfth supplier,
> the same claim form for a new file, the five-step portal wizard you work through
> every month.
>
> **What it does**
>
> - Saves and refills any number of named answer sets per form
> - Follows a form across every page it spans, including wizards that never change
>   their address
> - Drives search-as-you-type dropdowns and tag pickers, and correctly fills the
>   checkboxes and radios that web frameworks manage themselves
> - Checks each field after filling and tells you what it could not confirm
> - Encrypts what it saves behind a passphrase, if you want one
> - Exports and imports everything, so your data is portable and yours
>
> **It asks for no standing access to any site — it can read the page only
> after you click its button.** No account, no server, no analytics,
> no network requests of any kind. Grispy runs on the page in front of you, only
> after you click its button, and everything it saves stays in your browser.
>
> **Before you install, know this:** Grispy starts empty. It has nothing to offer
> on a form you have not saved yet — save a form once, and it is there every time
> after. It also cannot see rich-text editors, fields inside a web component's
> shadow DOM, or custom pickers with no ordinary form control underneath.
>
> Privacy policy: <https://lagtac.github.io/grispy-site/privacy/>
> Support: <https://lagtac.github.io/grispy-site/support/>

**Note, 2026-09-03 — "Grispy starts empty" has an expiry date.** It is true of
the build being submitted and can ship as written. It stops being true when the
extension's roadmap row 16 (global presets) ships, which is what that row exists
to change: a first visit to a portal will have something to offer. Rewrite this
paragraph and retake the screenshots in the same release, not after it.

### Data-usage disclosure form

Must agree with the privacy policy exactly. The answers the policy supports:

- **Data collected:** none. The extension makes no network requests, so nothing
  is transmitted to the developer or to any third party.
- **Data stored locally:** whatever the user chooses to save from a form, which
  may include personal and financial information. Held in the browser's own
  local extension storage, optionally encrypted with a user passphrase.
- **Sold to third parties:** no. **Used for purposes unrelated to core
  functionality:** no. **Used to determine creditworthiness or for lending:** no.

---

## 5. Firefox Add-ons (AMO) listing

The description is the Chrome one; AMO's summary field is the only piece that
needs its own draft.

### Summary — 234 characters; cap believed 250, verify

> Save a web form once, then fill it again in one click. Grispy holds many named
> sets of answers per form, follows multi-step wizards across every page, and
> asks for no standing access to any site — nothing it saves leaves your browser.

### Source-code note for reviewers

Grispy's source is not public and its licence is proprietary. AMO's source-code
requirement is satisfied by a private upload to reviewers, which needs no public
repository. This repository holds the site pages only, and no extension source.

---

## 6. Claims check

Every factual claim the copy makes, and where it was checked. Re-verify the whole
table before each submission; there is no CI enforcing any of it.

| Claim as written | Verified against | Checked | Notes |
|---|---|---|---|
| "makes no network requests of any kind" | `scripts/check.js` rule 8 over `src/`; no `fetch`, `XMLHttpRequest`, `WebSocket`, `sendBeacon` or `EventSource` in `src/` or a built `dist/` | 2026-08-29 | `pnpm check` is separate from `pnpm build` and nothing runs it automatically — re-run by hand |
| "asks for no standing access to any site" | `manifest.config.js` ships `permissions: ["storage", "activeTab", "scripting"]`; `check.js` rejects `host_permissions` and declared `content_scripts` | 2026-08-29 | **Do not upgrade this to a claim about what Chrome's install dialog says** until someone has installed a packaged build and read the dialog. The repo asserts "no install-time warning" but nobody has recorded seeing the prompt |
| "runs only after you click it" | `activeTab` is scoped to the tab the action was invoked on; `scripting` injects only into that tab | 2026-08-29 | This is also the honest limit: no fill on page load |
| "never uses sync storage" | every storage call is `chrome.storage.local` | 2026-08-28 (policy) | Policy §2 |
| "can be encrypted with a passphrase only you know" | encryption at rest shipped 2026-08-28 | 2026-08-28 | Opt-in. **Never write "is encrypted"** — the user is asked once and may decline |
| "conceals what you saved, not which sites you saved it on" | `ENCRYPTED_PREFIXES = ["form:", "formpreset:"]` in `src/core/storage.js:44`; `stepindex:` and `active:` are plaintext by design | 2026-09-01 | Wording is lifted verbatim from policy §2 — keep it that way. Re-checked after the form-preset rename moved the second prefix from `profile:` |
| "follows a form across every page it spans" | multi-step wizard attach/split/detach, plus step identity for wizards that do not change their address | 2026-08-29 | Bounded by the hidden-step limit, which the copy states |
| "drives search-as-you-type dropdowns and tag pickers" | widget drive with per-field deadline; verification reads the widget's own display | 2026-08-29 | |
| "correctly fills the checkboxes and radios that frameworks manage" | framework write-path fidelity shipped | 2026-08-28 | |
| "tells you what it could not confirm" | fill reports an `unverified` outcome and the toast carries the count | 2026-09-01 | **Ungated 2026-09-01.** The framed-page miscount that held this back is fixed — extension roadmap row 5d, shipped 2026-08-29 |
| "exports and imports everything" | export and import both shipped | 2026-08-28 | Whole-store file replaces; single-form file adds |
| Cannot see contenteditable, shadow DOM, custom pickers | asserted deliberately as characterization tests in the extension's smoke suite | 2026-08-29 | These are tests that assert the *absence* of support, so they will fail loudly if it ever arrives |

**Guide pages** (`/guide/`), added 2026-09-01. Each page ends with an "Every
message, in one place" table quoting the extension's own strings; a string that
changes falsifies the row that quotes it.

| Claim as written | Verified against | Checked | Notes |
|---|---|---|---|
| `Filled 7 of 10 fields.` and `2 could not be verified.` are the whole of what a fill reports | `fillForm` in `src/popup/popup.js`; the second sentence is appended only when the count is above zero | 2026-09-01 | The guide states the limit these two sentences carry: `not-found`, `refused` and `unchanged` all fold into the denominator, so a user cannot tell which happened |
| The five outcome constants are never shown to a user | `src/shared/outcomes.js` defines five; the popup surfaces only the FILLED and UNVERIFIED counts | 2026-09-01 | **Do not write the constant names into a page.** ROADMAP row 9b was first drafted from this file rather than from the screen and got it wrong twice |
| A first save creates a preset named "Default"; `+` creates "Save 2", "Save 3" | `confirmSave` (`presetId ?? "default"`, name `"Default"`) and `nextPresetName` in `src/popup/popup.js` | 2026-09-01 | |
| The ⋯ menu appears only with two or more presets, and Delete is disabled on the last one | `overflowIsUseful` and `syncOverflowMenu` in `src/popup/popup.js` | 2026-09-01 | |
| The row question preselects the non-destructive answer | `renderRowChoices` sets `keep` checked | 2026-09-01 | The guide's advice to choose *Save just these* after a mid-list deletion follows from the position-matching limit (extension ROADMAP row 8c), not from the code preselecting it |
| Grispy does not add repeat rows for you | extension ROADMAP row 8d, open | 2026-09-01 | Stated in the guide as a limit with a workaround, not as a defect |
| Rows built from checkbox or radio groups are not recognised as a group | extension ROADMAP row 8e, characterized in the smoke suite | 2026-09-01 | |
| Export needs the store unlocked; Clear everything works while locked | `render()` disables export while locked; the Danger zone button is deliberately not disabled | 2026-09-01 | The guide leans on the second: reset is the only way back from a forgotten passphrase |
| The four encryption limits | lifted verbatim from policy §2 rather than reworded, per rule 1 of this document | 2026-09-01 | If §2 changes, the passphrase page changes with it |
| The four status-line readings: `Step 2 of 3`, `Part of a saved form`, `Which step is this?`, `Not part of a saved form` | `stepContextLabel` in `src/popup/popup.js` | 2026-09-01 | The multi-step page's whole mechanism hangs off these four |
| The save-guard titles `Save to Step 2?` and `Replace what's saved here?` | the `askStep` branch of the save dialog in `src/popup/popup.js` | 2026-09-01 | |
| Detached-page data is listed under *Unreachable records* on the **Settings** page | `src/core/audit.js` finding "F"; the options page has been four tabs called Settings since 2026-08-28 | 2026-09-01 | **The ported page said "Manage" and was wrong.** Corrected during the port. A page named in the guide that no longer exists under that name is the cheapest kind of drift to introduce and the hardest for a reader to recover from |
| The step-marker example is a heading like `Step 2: Payment` | `STEP_SHAPED` in `src/content/content.js` requires punctuation immediately after the ordinal, so `Step 2 of 3` is rejected | 2026-09-01 | An earlier draft of the guide used `Step 2 of 3`, which would have told a reader their wizard was served when it is not. The published page uses the accepted form |

---

## 7. Corrections owed to live copy

Lines currently published that this positioning does not support. This site has
withdrawn claims before rather than let them stand.

**Corrections 1 to 3 were made on 2026-09-02**, when `index.html` was rewritten
against [§3](#3-landing-page). They are struck rather than deleted, so what was
published and why it changed stays on the record.

1. ~~**`index.html`** — *"Grispy follows a form across every page it spans and
   refills the whole thing."*~~ **Cleared 2026-09-02.** The first half held;
   "the whole thing" overclaimed, because a wizard that hides its earlier steps
   is not followed and some field types are not reached at all. The capability
   now sits in *What it does that autofill does not* with its edge stated, and
   the hidden-step wizard is named outright in *What it cannot do yet*.
2. ~~**`index.html`** — the no-network claim sits in its own box below the
   fold, under a heading.~~ **Cleared 2026-09-02.** It is the strongest thing
   on the page and the only claim a reader can check *before* installing. It is
   now the second paragraph of the opening, above the first heading.
3. ~~**`index.html`** — no mention of encryption at rest, which shipped on
   2026-08-28.~~ **Cleared 2026-09-02.** *Your data stays yours* carries the §3
   wording verbatim — "can be encrypted with a passphrase only you know",
   never "is encrypted", because the user is asked once and may decline.
4. ~~**`support/index.html`** — "free to everyone, with no paid tier."~~
   **Cleared 2026-09-03.** [§1](#1-price-settled-2026-09-03) settled the price,
   which made the sentence wrong rather than merely unsupported. Both it and the
   landing page's unqualified "free" now read *free for personal use*, and the
   correction was made in the same push as `/terms/` — publishing a terms page
   requiring a licence for commercial work, beside a support page promising there
   is no paid tier, would have left the site contradicting itself.

   The landing page's own "Grispy is free and is written by one person" was
   corrected in the same pass, to the same wording, for the same reason. Neither
   page carries a price — only the qualification. Prices appear when row 6e's
   page is written and the gates §1.3 names are closed.

5. ~~**`/terms/`** — "using Grispy as part of your work needs a paid licence",
   the Pro and Team tier table, and "paid features work for seven days after you
   install".~~ **Withdrawn 2026-09-03, the day after it was published.** This is
   item 4's correction being corrected: §1 settled the price, item 4 made the
   live pages agree with it, and none of it was true of the software. There is no
   licence key surface, no capability a key could gate, and `LICENSE` grants every
   installer commercial use for nothing — so the page did not merely anticipate a
   ladder that does not exist, it contradicted the licence that ships.

   The site got ahead of the product. Both stores read the linked terms, so a
   terms page describing gating the submitted build does not contain is a
   listing/build mismatch, which is why this was fixed before registration rather
   than at leisure. `/terms/` is rewritten rather than removed — four footers link
   it — and now says Grispy is free, that nothing you can do today will ever
   start needing a licence, and that capabilities for professional use are being
   built and will need one. No prices, no named paid features, no dates.

   **This is the second correction to the same page in two days**, and it is on
   the record for that reason. The rule it produced is in §1's bracket: settled
   wording is not publishable wording until the software it describes exists.

---

## 8. Gates before submitting

Not copy. Things that must be true in the extension before this copy is honest.

- ~~**A fill on a page built from frames reports the wrong outcomes.**~~
  **Cleared 2026-09-01.** Only one frame's answers were counted, measured at 20 of
  21 fields reported as not-found on a page that had actually filled them, so any
  listing promising that Grispy tells you what it filled was contradicted on
  screen. Fixed as extension roadmap row 5d, shipped 2026-08-29: the fill asks each
  frame by explicit `frameId` and merges to one outcome per field. The two
  sentences this gated — §3's "checks each field afterwards" and §4's "tells you
  what it could not confirm" — are unbracketed, and the §6 row is re-dated.

  Kept rather than deleted because it is the one gate that has cleared, and
  because it stood for three days after the fix landed while the sentence it
  blocked is the differentiator §2 names.
- ~~**Settle the price question** ([§1](#1-one-open-decision-price)) and write the
  wording here before it appears anywhere.~~ **Cleared 2026-09-03, by removing the
  dependency rather than by answering it.** The first release is free and has
  nothing to sell, so no price has to be settled before submitting. §1 stays
  bracketed until there is.
- **Install a packaged build and read Chrome's permission dialog**, so the
  strongest claim on the page can be written from observation rather than from the
  manifest.
- **Re-run `pnpm check` by hand** and re-date the §6 table.
