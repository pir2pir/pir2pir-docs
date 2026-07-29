# pir2pir-docs

Content for the Pir2pir documentation site. This repo holds Markdown only — the Docusaurus engine,
build and deploy live in [pir2pir-docs-site](https://github.com/pir2pir/pir2pir-docs-site).

## Layout

| Path | Contents |
| --- | --- |
| `docs/` | Russian source (default locale) |
| `i18n/en/docusaurus-plugin-content-docs/current/` | English translations |
| `i18n/uz/docusaurus-plugin-content-docs/current/` | Uzbek translations |
| `registry/links.json` | canonical routes, kept in sync with the bot's links |
| `ai/` | shareable project context for AI-assisted work |

Locales: `ru` (default), `en`, `uz`. A page missing a translation falls back to the Russian version.

## Publishing

Push to `production` triggers a rebuild in the site repo via `repository_dispatch`. Nothing else is
required — the site clones this repo during its build.

## Legal documents

`docs/legal/` holds the operator's legal documents. Two rules matter there:

- **Consent is a separate document.** Since 1 September 2025, 152-FZ requires consent to personal
  data processing to be executed separately from other documents — it must not be merged into the
  Terms of Use.
- **Russian is authoritative.** Translations carry a precedence note; update `docs/` first.

Any change to these files should be reviewed by a lawyer before it reaches `production`.
