---
sidebar_label: Web app
sidebar_position: 1
---

# What has changed — web app

The app updates itself. This is what arrived and what was fixed, newest first. Your version number is at the bottom of the Profile screen.

## 1.18.0 — 2026-08-06

**Notifications.** Everything that has happened to you, in one place — a bell on Home with the unread count, and each one opening at its own address. Reviews, chats, and the school's own reminders if you forward them. Kept for 90 days, and what appears there is never affected by which channels you have switched on. Opening one shows what it is about: the project and the hub, who wrote and an excerpt of what they wrote, how a search ended, which address a forwarded mail came from.

**Notification settings.** Under Profile: where each kind of message is allowed to reach you — Telegram, MAX, the open app, or a push to a closed one. Switching a channel off stops the interruption, not the record.

**Push, in a browser and on a home screen.** Turn it on from Profile and see an example of what one looks like. On iPhone and iPad the app has to be on the Home Screen first, which is Apple's rule; the settings say so where it applies.

**Notifications from the school.** Forward 21School's own mail to your address at pir2pir.ru and it arrives here as notifications. The confirmation your mail provider sends goes to us rather than to you, so the page shows it — including which mailbox it came from.

**Edit your profile.** Your name, surname and photo — what other peers see beside a request or in a chat header. The Edit button is now in the profile header, and everything you can change is on one page: the photo used to be two links at the top and the name a settings row at the bottom of the same screen. Everything else there comes from 21School.

**The sign-in code, by email or on Rocket.Chat.** Two buttons on the sign-in screen now. The school's mail sometimes files the code as spam, which is the commonest reason signing in fails at all; a direct message on the school's Rocket.Chat arrives without relays or filters. The code screen says where it actually went, rather than where it was asked to go.

**Joining review matching. Peer review works in both directions, and you are now asked before a search rather than refused after one: the app explains that a single switch turns on both — you can look for a reviewer, and other peers can ask you to review theirs. Turn it on and the search carries on with the project you picked. It can be switched off again in Notification settings.

**Feedback and invitations** gained a FAQ answer each, and How it works now covers six questions.

## Fixed — 2026-08-06

- Announcements from the school no longer arrive as a heading with nothing under it: each carries its project and the time the school wrote, in the school's own words.
- The app says so plainly when the service is briefly unavailable — a full screen that waits and returns by itself, instead of an error on whichever screen you happened to be on.
- Errors sometimes showed an internal name instead of a sentence.
- Notification settings no longer offer a switch for a messenger with nowhere to deliver: Telegram appears only once it is linked, and MAX — which cannot be linked here at all yet — does not appear. A channel switched on that leads nowhere is worse than one that is missing.
- Asking somebody you already have a chat with now opens it, instead of saying that one exists somewhere. It usually got there by itself — from a review match — so there was nowhere to go and look.
- A chat now follows a conversation down when a message arrives and you are reading the end of it — new ones used to land under the fold. Scrolled up, nothing moves, and loading older messages no longer shifts the place you were reading.
- The chat's input could fail to appear on a page that had been open since before an update, leaving an empty box where it belongs. The app now says it has been updated and offers to reload — the same for any screen it cannot finish fetching.

## 1.17.0 — 2026-08-02

**Invite a peer.** Your own code, and two links that carry it — one opens the app, the other opens the bot. Tap the code or either link to copy it. Anybody who signs up holding it is recorded as yours, and they appear under "Joined through you" as soon as their account exists.

**Who has brought the most.** A board of it, with the way off the board on the same screen: hiding takes your name off and leaves your place, so nobody moves up by you stepping back.

**Display and accessibility.** Under Profile: larger text, higher contrast, less motion, and reading screens aloud in Russian where your browser has a voice for it. Everything is off until you turn it on, nothing changes for anybody who does not, and the settings stay on your own device. The page also points at the screen reader already built into your phone — it reads this app better than any switch of ours could.

**Leave feedback.** Say what Pir2Pir is like to use, in a few sentences. It is read before it appears on the site, and it appears with your school login beside it — which the screen says before you write rather than after. Beside it, what other peers have said.

**Pir2Pir ID Chat Guard.** Its own page and an answer under How it works, with the whole procedure for turning the join gate on in a Telegram chat you administer: the two rights the bot asks for and why, the three commands, where notifications and request reviews can go, and what to try in a chat that does not matter first.

**Two ways to hand the link over.** One tap opens Telegram's own chat picker with the message already written — in the app, in a browser, and from an app on your home screen — and beside it, on a phone, your device's own share sheet for everywhere else.

**How it works** gained a third answer, on inviting.

## 1.16.0 — 2026-08-02

**How it works.** Short answers to the two things everybody asks — how to find a peer, and how the review search works. Each one ends on the button that does it.

**Faster to open.** The app fetched somebody else's script before it could draw anything, and shipped every screen in one file. That script is served from here now — which also means the app works where telegram.org is blocked — and screens arrive as they are opened.

**Two openings for a message.** Writing to somebody who is not here yet can start from one of two sentences, and everything after that is yours.

**Telegram links open Telegram.** From an app on your home screen a t.me link used to open a page about the chat rather than the chat.

**Home and Profile.** The figures come first and the features are cells rather than cards; the profile has a bigger picture, the experience beside the level, and peer review points.

**Reading the news.** The channel you are on is a name in the header that opens the list, instead of a row of tabs to drag sideways.

## Fixed — 2026-08-02

- Announcements read `:doge_dance:` where the school's own emoji belonged — about one headline in five.
- An error sometimes showed an internal name instead of a sentence.
- Not being able to write to somebody now says which of three reasons it is: your own allowance for the day, that you wrote to them recently, or that they have heard from enough people lately.
- On iOS the keyboard covered the message you were writing.
- The channel you are reading is a filled row rather than red text in a box.
- Choosing a language opens from the bottom, instead of a list that could land off the screen.
- The legal documents are in one place, under Profile.

## 1.15.0 — 2026-08-01

**School news.** Announcements from the school's own chats are readable in the app: channels across the top, and each announcement on its own page with an address you can send to somebody. There is a filter — words, author, date, pinned only, with a picture only.

**Community.** One screen for everything around the app: the chat and the channel on Telegram and MAX, the bots, the documentation, the source, the legal documents and how to reach the operator.

**Growth over the week.** Beside the figures at the foot of Home, how many of them are new in the last seven days.

## 1.14.0 — 2026-07-31

**An installed app keeps itself current.** An app added to the home screen could run an old version for weeks: it is resumed rather than reloaded, and nothing was checking for a new build. It checks now, every time it is opened, and reloads once the new one is ready — unless you are typing, in which case it waits for the next time.

## 1.13.0 — 2026-07-31

**Ask one peer to chat.** If you know their login, send them a request with a message. Reviews and chats are two lists now: a review came out of the queue and is about a project, a chat is a conversation about whatever the two of you want.

**Reaching somebody who is not here yet.** Where a peer is at the school but not on Pir2Pir, the app offers to pass one message on — by email or Rocket.Chat — and tells you what happened on each.

## Fixed — 2026-08-01

- A review search no longer ends the moment nobody is available. It keeps looking, and a match can arrive while you are away.
- A chat stopped calling itself a review: "Close this chat?" rather than "End this review?".
- Every conversation has a way out of it — a back arrow in the header, including in the app on your home screen, where there was none.
- The news feed no longer scrolls sideways on a long link, and pictures open at full size instead of as a blurred stand-in.
