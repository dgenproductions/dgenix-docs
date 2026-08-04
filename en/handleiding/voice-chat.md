# Voice Chat

You can talk to your assistant instead of typing. dGENIX has two voice modes: **Voice Memo** (quick dictation) and **Voice Call** (a fully spoken conversation).

---

## Voice Memo, quick dictation

**When to use it?** When you want to send a question or command quickly without typing. Your assistant replies with text in the chat.

**How it works:**

1. Click the **microphone icon** to the right of the text field in the chat
2. Speak your question or command
3. Click again to stop
4. Your question is converted to text and processed
5. The answer appears as text in the chat

**Credit cost:** transcription + AI processing, roughly 25-200 cr depending on the command.

---

## Voice Call, a fully spoken conversation

**When to use it?** When you really want a conversation with your assistant, ask, listen, respond, without typing. The assistant speaks its answers aloud.

**How it works:**

1. Click the **sound-waves icon** to the right of the text field
2. An animated orb screen opens, this is the Voice Call interface
3. Speak your question or command
4. The assistant processes and speaks the answer back
5. After the answer it listens again straight away, no clicking needed
6. Click "Hang up" to end the call

**The orb:** the animated sphere reacts to sound, it pulses when you speak, settles when you are quiet and moves while the assistant is thinking.

**Text shown in parallel:** while the assistant speaks, its answer also appears as text on screen.

**Voice Call credit cost:**

| Action | Credits |
|---|---|
| Transcribe your question | ~5-20 cr |
| AI processing (Haiku) | ~25-50 cr |
| Spoken answer ~500 chars | ~1,375 cr |
| Spoken answer ~1,000 chars | ~2,750 cr |

Voice Call uses more credits than typing, mainly because of text-to-speech.

---

## Setting a voice

You choose which voice your assistant uses for Voice Chat. Go to **Settings -> AI Assistant -> Voice**.

There are two groups:

- **Dutch voices**, for use on `app.dgenix.nl`
- **English voices**, for use on `app.dgenix.com`

The voices are powered by ElevenLabs, one of the most realistic text-to-speech systems available.

---

## Voice messages via Telegram

If you have the Telegram add-on, you can also send voice messages via Telegram:

1. Send a voice message to @dGENIXbot
2. The assistant transcribes it automatically
3. It processes the command and replies as text in Telegram

Telegram voice messages do not return a spoken answer (that is only in Voice Call via the dashboard).

---

## Tips

**For the best transcription:**
- Speak clearly and not too fast
- Be in a quiet environment
- Finish your sentence before you stop

**Voice Memo or Voice Call?**
- Use **Voice Memo** for short commands ("create a calendar appointment", "write an email")
- Use **Voice Call** for a full conversation, brainstorming or discussion

**Be credit-aware:** Voice Call is the most expensive channel. It is most enjoyable for longer conversations. For short commands, typing or Voice Memo is more efficient.

---

## What you see

You open a Voice Call and ask out loud what is on today. The orb pulses while
you speak, settles when you stop, and moves while GENI is thinking. Then you
hear the answer and read along:

> You have three appointments today. At ten you are calling De Vries about the
> quote, at half past one you are at the supplier, and at four you have a team
> meeting. Between twelve and half past one is your only free block.
>
> Shall I prepare the De Vries call?

You do not have to click anything: after the answer it listens again straight
away. Say nothing more and it waits quietly until you hang up.

## Limits

- **Voice Call is the most expensive channel.** Text-to-speech costs the most credits; for short requests typing or a Voice Memo is cheaper.
- **Telegram does not speak back.** There you get text; only the Voice Call in the dashboard talks.
- **Background noise costs you accuracy.** In a busy room or on speaker it degrades noticeably.
- **There is no live interruption.** You cannot override GENI mid-answer; wait until it finishes or hang up.
- **The voice follows the domain.** Dutch voices on `app.dgenix.nl`, English on `app.dgenix.com`.
- **Confirmations do not work by voice.** If you ask for something irreversible, GENI points you to the chat, because that is where the button is.

## Troubleshooting

**You are not being heard.** Grant your browser microphone permission and check that the right microphone is selected in your system settings.

**The transcription is wrong.** Speak more slowly and finish your sentence before stopping. Jargon and proper names go wrong more often; type those instead.

**You hear no answer.** Check your volume and whether the tab is muted. If it stays silent while the text does appear, the speech conversion failed; try again.

**It uses credits faster than expected.** That is correct: a spoken answer of a thousand characters costs about 2,750 credits. For short requests Voice Memo is considerably cheaper.

**The wrong language comes out.** The voice follows the domain you work on. Use `app.dgenix.com` for English.

## Frequently asked questions

**What is the difference between Voice Memo and Voice Call?**
A memo is recording once and getting a text answer back. A call is a running
conversation where GENI answers out loud and then listens again.

**Can GENI do everything it does in chat?**
Yes, the same skills and the same memory. Only confirmations for irreversible
actions go through the chat.

**Is my voice stored?**
The recording is used to turn your words into text; we keep the conversation as
text, like any chat.

**Does it work on my phone?**
Yes, in the browser. Make sure you allow the microphone.

---

Next: [AI assistant](../functies/ai-assistent.md) · [The credit system](../hoe-het-werkt/credits.md) · [Settings](../functies/instellingen.md)
On the site: [all skills](https://dgenix.com/skills) · [pricing](https://dgenix.com/pricing)

*dGENIX Docs, Voice Chat, updated August 2026*
