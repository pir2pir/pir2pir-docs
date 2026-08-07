---
title: How to sign in
sidebar_label: How to sign in
sidebar_position: 1
---

# How to sign in

Pir2Pir has no password. A sign-in is confirmed with your school login and a one-time code — that is
how the service knows you really are a School 21 participant, without keeping yet another password
you could lose.

You can sign in through the web app or through the Telegram bot. It is the same account either way:
sign in to the bot and you are signed in to the app.

The screenshots below show the Russian interface; both the app and the bot have the same screens in
English.

## Where the code arrives

Both ways of signing in ask the same thing — where to send the code.

- **Rocket.Chat** — a message in the school chat, to your login. Arrives at once, bypassing email.
- **Email** — a letter to `@student.21-school.ru`. Works for everyone, but it can be delayed, and the
  school's mail server often files it as spam.

A code lasts 10 minutes and works once.

## The web app

Open [app.pir2pir.ru](https://app.pir2pir.ru).

### 1. Enter your school login

The login only — `@student.21-school.ru` is filled in for you. The buttons stay inactive while the
field is empty.

<img src="/faq/sign-in/app/01-login.jpg" alt="Sign-in screen with an empty login field" width="280" />
<img src="/faq/sign-in/app/02-login-filled.jpg" alt="The same screen with a login entered" width="280" />

### 2. Choose where the code should go

Press **Код в Rocket.Chat** (code to Rocket.Chat) or **Код на почту** (code to email).

Below them is a row headed "or sign in with" — Telegram, MAX and the app. Those are the same accounts
approached from another side; the "скоро" tag means that route is not working yet.

### 3. Fetch the code and enter it

**If you chose Rocket.Chat** — open the school's Rocket.Chat. The message arrives as a direct
message, from your own login.

<img src="/faq/sign-in/app/03-rocket-chat-code.jpg" alt="The «check the school chat» screen with a code field" width="280" />
<img src="/faq/sign-in/app/04-rocket-chat-message.jpg" alt="The message carrying the code in Rocket.Chat" width="280" />

**If you chose email** — open your school mail. If nothing has arrived after a minute, look in spam
before requesting another: a second code cancels the first.

<img src="/faq/sign-in/app/05-email-code.jpg" alt="The «check your email» screen with a code field" width="280" />
<img src="/faq/sign-in/app/06-email-letter.jpg" alt="The letter carrying the confirmation code" width="280" />

Type the six digits and press **Войти** (sign in). Wrong login? "Изменить логин" takes you a step
back.

## The Telegram bot

Open [@pir2pirbot](https://t.me/pir2pirbot).

### 1. Press "Start"

<img src="/faq/sign-in/tg-bot/01-start.jpg" alt="The bot's page in Telegram with the Start button" width="280" />

### 2. Choose a language and press "Начать"

<img src="/faq/sign-in/tg-bot/02-language.jpg" alt="Language choice: RU, EN, UZ" width="280" />

### 3. Accept the terms

The bot shows three documents — the [Terms of Use](/en/legal/terms/), the
[Privacy Policy](/en/legal/privacy_policy/) and the
[Consent to Personal Data Processing](/en/legal/consent/). Your account cannot be connected without
that consent: the service is not part of School 21 and processes data on your consent rather than on
its behalf.

<img src="/faq/sign-in/tg-bot/03-consent.jpg" alt="The consent screen with «agree» and «decline» buttons" width="280" />

### 4. Choose where the code should go

<img src="/faq/sign-in/tg-bot/04-code-channel.jpg" alt="Choosing a channel: Rocket.Chat or email" width="280" />

### 5. Send your login as an ordinary message

Just type the login into the chat. The code arrives wherever you chose at the previous step, and it
goes back the same way — as a message.

<img src="/faq/sign-in/tg-bot/05-login.jpg" alt="The bot asking for the 21School login" width="280" />

## If the code does not arrive

- **No letter.** Look in spam. If your school mail is forwarded to mail.ru it may not arrive at all —
  use Rocket.Chat instead.
- **No message in Rocket.Chat.** The code goes to the school login you typed. If it was somebody
  else's, or misspelled, the message went to them — go back and correct it.
- **The code is rejected.** It lasts 10 minutes and works once. If you requested a second one, only
  that one works.
- **None of this helped.** Write to [support@pir2pir.ru](mailto:support@pir2pir.ru).
