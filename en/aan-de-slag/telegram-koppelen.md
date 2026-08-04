# Connect Telegram (optional)

dGENIX is **dashboard-first**: you do not need Telegram to start. Telegram is a **free, optional add-on** that lets you reach GENI on the go. Everything stays in sync with your dashboard: the same assistant, the same memory, the same skills.

> You set up your assistant (name, working style) during the **intake** in the dashboard, not via Telegram. See [Getting started](README.md).

---

## Activate Telegram

1. Go to **Dashboard -> Skills**
2. Find the **Telegram** add-on and activate it (free)
3. Follow the linking steps below

---

## Option A, shared dGENIX bot (easiest)

Available on every plan.

1. Open **@dGENIXbot** in Telegram
2. Send the command `/start` with your personal link code (shown in the dashboard after activating the add-on)
3. Your account is linked automatically

## Option B, your own Telegram bot (Pro+)

Want GENI under your own bot name and handle? On **Pro** and up, your own bot is included.

1. Create a bot via [BotFather](https://t.me/BotFather) in Telegram (command `/newbot`)
2. Copy the bot token you receive
3. Paste the token in **Dashboard -> Skills -> Own Telegram Bot**
4. dGENIX validates the connection and puts your own bot live

[More about skills](../skills/README.md)

---

## What can you do via Telegram?

The same things as in the dashboard: send a command, ask a question, record a voice message. GENI replies in Telegram and keeps everything in the same memory and conversations as your dashboard.

Examples:

- "Give me an overview of my unread emails"
- "Schedule a meeting with Jan Friday at 2pm"
- "Summarise this voice message and add the action items to my calendar"

---

## Commands in Telegram

Besides ordinary requests, the bot knows a few fixed commands:

| Command | What it does |
|---|---|
| `/start` | Activate the assistant and enter your link code |
| `/credits` | Check your current credit balance |
| `/help` | Short list of available commands |

---

## Voice messages

Send a voice message in Telegram and GENI transcribes it automatically, then
handles it like any other request. Nothing to set up. Handy on the move: say
what needs to happen and GENI takes it from there.

---

## Web and Telegram stay in sync

What you send in the web chat also appears in Telegram, and the other way
around. Your conversation history, your memory and your active skills are the
same in both channels. So you start a conversation at your desk and finish it
on the go.

---

## Troubleshooting

**GENI does not reply in Telegram.** Check that the connection is still active
via **Dashboard -> Skills -> Telegram**, and that your credit balance is not at
zero (you see the balance top right in the dashboard).

**Lost the connection after switching phones.** Your Telegram account is linked
to your dGENIX account, not to a device. Send `/start` again with the link code
from your dashboard.

**Wrong bot.** If you use your own bot, `@dGENIXbot` no longer responds to your
account. Chat with your own bot instead.

---

## Disconnect Telegram

Go to **Dashboard -> Skills**, open the Telegram add-on and disconnect. Your account, credits and history are kept, you simply keep working from the dashboard.
