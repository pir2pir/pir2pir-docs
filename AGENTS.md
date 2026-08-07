# AGENTS

This repository supports human and AI-assisted documentation work.

## Purpose
- Keep edits focused on documentation content in `docs/`, `i18n/`, and `registry/`.
- Preserve Russian (`ru`) as the default locale unless a task explicitly targets translations.
- Keep changes small, reviewable, and safe for production deploys.

## Working Rules
- Prefer direct Markdown edits over structural churn.
- Keep routes and slugs stable unless the task explicitly requires route changes.
- Keep `registry/links.json` in sync with any docs structure change, including new, removed, renamed,
  or re-routed pages.
- When adding or changing legal docs, verify matching links in `registry/links.json` and in the
  Telegram bot's consent screen.
- Do not commit local cache artifacts.

## Changelogs
- `docs/changelog/` and its translations are mirrors. The source of truth is the repository of the
  thing being described, each keeping its own `docs/changelog/{ru,en,uz}.md`:
  `web-app.md` from pir2pir-web-app, `tg-bot.md` from pir2pir-tg-bot, `max-bot.md` from
  pir2pir-max-bot.
- Fix wording there, not here: an edit made here is overwritten the next time that repository
  publishes, and it leaves the two copies disagreeing until then.
- Everything below the front matter is copied verbatim, including the deliberately unwrapped lines.
  Do not reflow them to this repository's 100-column prose width.
- `.github/workflows/publish-changelog.yml` here is the machine that does it, called by each of
  those repositories. It writes to both `develop` and `production`, so an entry is on the site as
  soon as it is written and the staging branch never trails behind it.
- The destination paths, the front matter and the locale layout live in that workflow, which is why
  it is in this repo: they are facts about how the site is arranged. A caller supplies only its page
  name, its sidebar position and three labels. Adding a fourth product means a caller in its
  repository and a route in `registry/links.json` — nothing else here, and nothing in the site repo.

## Legal Documents
- `docs/legal/consent.md` must stay a standalone document. 152-FZ (from 01.09.2025) requires consent
  to be executed separately from other documents; merging it into `terms.md` would breach that.
- Russian is the binding version. Translations must carry the precedence note and be updated only
  after `docs/` changes land.
- Changing the data list, purposes, or recipients in `consent.md` is a substantive legal change, not
  a copy edit — flag it for review rather than applying it silently.

## AI Context Layout
Use the tracked `ai/` directory for shareable project context:
- `ai/index.json`: pointers to key files and operating assumptions.
- `ai/context.md`: concise project memory for recurring tasks.
- `ai/README.md`: maintenance notes for this context set.

Use local `.ai/` for ephemeral cache and per-machine indexes; it is git-ignored.

## Standard Flow
1. Read `README.md` and `ai/index.json`.
2. Apply the smallest valid change for the task.
3. Verify links/paths when touching navigation pages.
4. Update `ai/context.md` if the change alters long-term project conventions.
5. Commit with a clear, scoped message.
