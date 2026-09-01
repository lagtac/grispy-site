# Marketing copy

The words Grispy is described in, kept in one place so the landing page, the two
store listings and the Chrome Web Store's data-usage form cannot drift apart.

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
   The public URL is derived from the repository (`lagtac/grispy-site` on GitHub
   Pages) and **has not been confirmed against the live Pages settings**; a
   custom domain would change every one of them.

---

## 1. One open decision: price

**The copy below says nothing about price, and that is deliberate — it is not an
oversight to fill in.** The live pages already take a position, and it is a
position that is expensive to walk back:

| Where | What it says today |
|---|---|
| `support/index.html`, opening paragraph | "Grispy is free to everyone, with no paid tier and no separate support product" |
| `privacy/index.html` §7 | "if a licence is ever sold" — leaves the door open |
| `ROADMAP.md` row 6 | a payment provider to be named in the policy, "nothing to name yet" |

The extension repository's own working notes assume licence keys are the plan.
Two of the three surfaces above are compatible with that; the support page's
promise is not, and it is the one a reader is most likely to quote back.

Adding a third instance of "free" to a landing page and two store listings makes
that promise four times harder to retract. So this document stays silent until
the question is settled. **Settle it before submitting anything**, then add the
wording here first.

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
See [§1](#1-one-open-decision-price) before repeating "free" here.

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

---

## 7. Corrections owed to live copy

Lines currently published that this positioning does not support. This site has
withdrawn claims before rather than let them stand.

1. **`index.html`** — *"Grispy follows a form across every page it spans and
   refills the whole thing."* The first half holds. "The whole thing" overclaims:
   a wizard that hides its earlier steps is not followed, and some field types are
   not reached at all. Amend to the §3 wording, which keeps the capability and
   states its edge.
2. **`index.html`** — the no-network claim sits in its own box below the fold,
   under a heading. It is the strongest thing on the page and the only claim a
   reader can check *before* installing. Move it into the opening.
3. **`index.html`** — no mention of encryption at rest, which shipped on
   2026-08-28. A reader comparing the landing page to the policy finds the policy
   describing a protection the landing page does not know about.
4. **`support/index.html`** — "free to everyone, with no paid tier." Blocked on
   [§1](#1-one-open-decision-price); no edit until the question is settled.

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
- **Settle the price question** ([§1](#1-one-open-decision-price)) and write the
  wording here before it appears anywhere.
- **Install a packaged build and read Chrome's permission dialog**, so the
  strongest claim on the page can be written from observation rather than from the
  manifest.
- **Re-run `pnpm check` by hand** and re-date the §6 table.
