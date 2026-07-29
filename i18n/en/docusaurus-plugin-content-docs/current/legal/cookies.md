---
title: Cookies and Recommendation Technologies
sidebar_label: Cookies and recommendations
sidebar_position: 4
---

Effective date: 29.07.2026

This document describes the cookies and similar technologies used by Pir2Pir, and sets out the rules
for applying recommendation technologies, published pursuant to Article 10.2-2 of Russian Federal
Law No. 149-FZ of 27.07.2006 "On Information, Information Technologies and Information Protection".

Personal data processing is governed by the separate [Consent](./consent.md) and
[Privacy Policy](./privacy_policy.md).

:::note[Translation]
The Russian version is the legally binding one. This translation is provided for convenience.
:::

## 1. Operator

| | |
| --- | --- |
| Operator | Sole proprietor Aigiz Iskuzhin |
| INN | 024803896842 |
| OGRNIP | 326028000044859 |
| Roskomnadzor operator register | [No. 2-26-056967](https://pd.rkn.gov.ru/operators-registry/operators-list/?id=2-26-056967) |
| Contact | legal@pir2pir.ru |

This document covers https://pir2pir.ru, https://app.pir2pir.ru and https://docs.pir2pir.ru, as well
as the Telegram bot [@pir2pirbot](https://t.me/pir2pirbot).

# Part I. Cookies and similar technologies

## 2. Strictly necessary and functional technologies

The interface relies on browser local storage (`localStorage`) — a technology similar in purpose to
cookies, but one that is not sent to the server automatically:

| Resource | Entry | Purpose | Lifetime |
| --- | --- | --- | --- |
| pir2pir.ru | `pir2pir.locale` | the chosen interface language | until site data is cleared |
| app.pir2pir.ru | session token and timestamp | staying signed in to the web app | until sign-out or site data is cleared |
| docs.pir2pir.ru | theme and language settings | documentation appearance | until site data is cleared |

Without these entries the interface cannot remember a language or keep you signed in, so they are
always applied and require no separate consent.

## 3. Analytics technologies

**Yandex Metrica** is used to measure traffic and interface quality. It sets its own cookies:

| Cookie | Purpose | Lifetime |
| --- | --- | --- |
| `_ym_uid` | anonymised visitor identifier | 1 year |
| `_ym_d` | date of the first visit to the site | 1 year |
| `_ym_isad` | whether an ad blocker is present | 2 days |
| `_ym_visorc` | current behaviour-recording session | 30 minutes |

The data collected is anonymised: pages requested, referral source, device and browser type, and an
approximate region derived from the IP address. It is used in aggregate and is not applied to make
decisions about an individual visitor.

With respect to the data Metrica collects, the operator is YANDEX LLC under the
[Yandex Metrica Terms of Use](https://yandex.ru/legal/metrica_termsofuse/).

## 4. How to opt out

Cookies and local storage are managed in the browser: site settings can block them, and stored data
can be removed ("clear site data").

Yandex Metrica can be declined separately using
[Yandex's official opt-out](https://yandex.ru/support/metrica/general/opt-out.html).

Declining analytics does not restrict access to the service. Blocking the strictly necessary
technologies in section 2 does not break https://pir2pir.ru, but it does make it impossible to keep
a session in the web app — you would have to sign in again every time you open it.

## 5. Third-party technologies

The bot and the mini app run inside Telegram. Telegram is an independent operator with respect to
the data it collects and applies its own privacy policy, which this document does not cover.

# Part II. Rules for applying recommendation technologies

## 6. General

These Rules are published pursuant to Article 10.2-2(3) of 149-FZ and describe the processes and
algorithms used to present information based on data about the service's participants.

Recommendation technologies are applied in exactly one function — **matching participants for peer
reviews of study projects**. That purpose is stated in item 2 of section 4 of the
[Consent](./consent.md).

Searching for a participant by login is not a recommendation technology: it is a deterministic
lookup by exact match and by login prefix, and its result does not depend on the preferences of the
person searching. Searching by first or last name is not performed.

## 7. Data used for recommendations

Matching uses the data listed in section 3 of the [Consent](./consent.md):

| Data | Source |
| --- | --- |
| Project list and project status | School 21 public API, participant profile sync |
| Campus and wave | School 21 public API |
| Review points and feedback score | School 21 public API |
| The project and campus stated in a review request | provided by the participant |
| Notification settings | provided by the participant |

Data collected by the analytics technologies in section 3 plays no part in matching: recommendations
are built only on study-profile data and on the request the participant made themselves. The
contents of participants' conversations, special categories of personal data (Article 10 of 152-FZ)
and biometric data (Article 11) are not used for recommendations.

## 8. How matching is formed

Candidates are selected and ordered by the following rules:

1. **Project** — a hard filter on an exact project code match. Participants who cannot review that
   project are not included.
2. **Reciprocity** — pairs where both participants are waiting for a review of the same project are
   preferred, because such a pair resolves the need of both.
3. **Campus** — a soft preference for the same campus; cross-campus matching is allowed and is not
   restricted.
4. **All else being equal** — review points and feedback score are taken into account as indicators
   of review experience.

The operator makes no decisions producing legal consequences for a participant on the basis of
matching. A match is a recommendation: the participant may decline the proposed pair, and the review
itself takes place on the School 21 platform, outside the operator's control.

## 9. Participant control

Matching is only possible after registration and giving [Consent](./consent.md). A participant may
at any time:

- change or switch off notifications about review requests;
- decline a proposed pair;
- delete their account in the Telegram bot, which stops the application of recommendation
  technologies and withdraws the Consent.

There is no separate "recommendations off" switch: without matching the service does not perform its
only function.

## 10. Complaints

Enquiries and complaints about the application of recommendation technologies go to
legal@pir2pir.ru and are answered within 30 days of receipt.

## 11. Changes

The current version is published at https://docs.pir2pir.ru. Changes affecting the technologies
applied or the data used are announced through the Telegram bot.
