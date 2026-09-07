# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

`grispy-site` is the **public** GitHub Pages site for Grispy, a Chrome + Firefox
MV3 extension that saves and fills web forms. The extension's source lives in a
separate **private** repository, `lagtac/grispy`, and is not open source. This
repository is public only so Pages can serve it, and it holds **every word a user
or a store reviewer reads** — because the other repository is private, nothing
written to be read from outside it can live there. `README.md` has the path-by-path table.

## Pushing publishes

**There is no build step and no CI gate: pushing to `main` puts the change on the
live public web.** Treat a push here as an outward-facing action, not a save.
`CHANGELOG.md`'s `[Unreleased]` therefore means *live, but not yet pointed at* —
the boundary is the moment a store listing starts sending people to these URLs.

## The privacy policy is the load-bearing page

`/privacy/` and `/support/` are typed into the Chrome Web Store and
addons.mozilla.org listing forms. Once a listing is live, **renaming or moving
either path 404s a link that is no longer ours to fix from here** — see the
Publication Contract in `CHANGELOG.md` before touching a URL.

The policy makes checkable factual claims about the extension's behaviour: no
network requests, no sync storage, no runtime dependencies, encryption at rest
with stated limits. `README.md` lists each claim and how it was verified.
**Re-verify against the extension's `src/` by hand before editing** — it is checked
out as a sibling directory in the usual working layout. The extension's `pnpm
check` enforces some of these, but it is a separate command from `pnpm build` and
nothing runs it automatically.

When the extension's behaviour changes in a way the policy describes, **this page
changes first**, and the Chrome Web Store's data-usage disclosure form must agree
with it exactly. A policy that overstates what the software does is worse than no
policy.

## `docs/copy.md` is the single source for wording

It holds the landing page, both store listings, and a claims-check table in §6
recording where each factual claim was verified. **A claim with no row in §6 is
not ready to publish.** Where the privacy policy already has a sentence for
something, the copy borrows that sentence rather than inventing a second wording.

Two documents held the listing copy between 2026-08-28 and 2026-09-01 and drifted
within three days. Do not create a second copy of any user-facing text anywhere —
including in the extension repository, which deliberately keeps no mirror of
`/guide/`.

**Not everything in `copy.md` is publishable.** §1 (pricing) is settled wording
that may not reach a page while nothing can be bought; §8 lists gates the
extension must clear before the copy can honestly go up. Read a section's own
header note before lifting text from it.

## Records, not plans

`ROADMAP.md` is forward-looking, `CHANGELOG.md` backward-looking, and they meet at
the commit that ships a page. **There is no `docs/plans/` here and that is
deliberate** — a page is small enough that a roadmap row plus its linked CHANGELOG
entry is the whole record. Do not create one for routine page work; if a change
genuinely warrants a plan, ask first.

## Git workflow

GitHub, not GitLab. The remote is a backup, not a review surface: **no PRs or MRs,
no `gh`, no `glab`.** Integrate a branch with a local squash-merge into `main` —
`git merge --squash <branch>` plus one Conventional Commit — then push. After
merging, remove the worktree but **keep the branch** as a record of the approach.
