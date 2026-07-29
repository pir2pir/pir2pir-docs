# Project memory — pir2pir-docs

## What this is
Content repo for https://docs.pir2pir.ru. Markdown only. The Docusaurus engine lives in
pir2pir-docs-site and clones this repo at build time.

## Operator
Pir2Pir is run by IE Aigiz Iskuzhin (INN 024803896842, OGRNIP 326028000044859, OKVED 62.01),
registered with Roskomnadzor as a personal data operator under No. 2-26-056967.

Pir2Pir is an independent service. It is not School 21 and does not act on its behalf — every legal
document states this explicitly, because the service cannot inherit School 21's legal basis for
processing and relies on its own consent instead.

## Locales
`ru` is the source and the binding version. `en` and `uz` are translations under
`i18n/<locale>/docusaurus-plugin-content-docs/current/`, each carrying a precedence note. Missing
translations fall back to Russian.

## Legal structure
Four documents, deliberately separate:
- `consent.md` — consent to personal data processing. Standalone by law (152-FZ, from 01.09.2025).
- `privacy_policy.md` — published under art. 18.1(1)(2).
- `terms.md` — service rules, no personal data provisions.
- `cookies.md` — cookies and similar technologies, plus the recommendation-technology rules required
  by 149-FZ art. 10.2-2(3). Written to describe analytics as applied so it does not need revising
  when Yandex Metrica is switched on; the operator's decision, recorded here so it is not "fixed"
  back to the current state by someone checking the sites for a Set-Cookie header.

Consent covers matching and participant search only. Advertising and any transfer to commercial or
recruiting services are explicitly excluded and would need separate consent.

## Consumers
The Telegram bot's consent screen links to these pages. Route changes must be mirrored in
`registry/links.json` and in the bot's localization files.
