# Voice Message

With the Voice Message skill, GENI listens to a spoken message and tells you what is
being asked, how it sounds and what you should do about it.

Available from **Growth**. No connection needed; you share a file or provide a link.

## What can GENI do with a voice message?

The difference with a transcript is the word "listening". A transcript puts the words
on paper and the tone disappears with it: whether someone was hesitant, rushed or
making a commitment is nowhere to be found. With this skill the recording itself goes
to the model, so that information comes along.

You get back:

- **The gist** in one sentence, what does this person want
- **The tone**, and what you can hear it in
- **What was said**, in short bullets, not a word-for-word transcript
- **What you need to do**, or an explicit note that no action is needed
- **How urgent it is**, with the reason

## Example: what you ask, what you get back

```
Listen to this message from a customer and tell me what I should do
```

> **Gist:** he wants to know whether Friday's delivery is still on.
>
> **Tone:** businesslike but tense. He speaks quickly, repeats the date twice and
> ends with "just let me know, alright".
>
> **What was said**
> - Last week's order was confirmed, but he has not seen a shipping date
> - His own customer expects the product on Monday
> - He briefly mentions it was late the previous time as well
>
> **Action:** call back today with a firm shipping date, or tell him if Friday will
> not happen.
>
> **Urgency:** high. He has a commitment of his own towards Monday and refers to an
> earlier delay.

If you add context, for example who the message is from or what it concerns, the
analysis gets sharper.

## Requirements

- **Plan:** Growth and higher
- **Connection:** none

## Activate

1. Go to **Dashboard → Skills** and activate **Voice Message**
2. Send the message along in the chat, or provide a link to the audio file

## What it costs

**60 credits per message**, regardless of length. A twenty second message therefore
costs the same as a ten minute one. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits and boundaries

- **Built for short messages.** Up to roughly fifteen minutes. For an hour-long
  meeting, use [Audio Transcription](transcriptie.md).
- **Three formats:** WAV, MP3 and M4A. Other formats are rejected.
- **Maximum 25 MB** per file.
- **No word-for-word transcript.** You get a summary with tone and action. If you
  want the exact words, Audio Transcription is the right skill.
- **Speakers are not identified by name.** With multiple voices, GENI refers to them
  as Speaker 1 and Speaker 2.
- **Tone is an estimate.** It remains an interpretation of how something sounds, not
  a fact about how someone feels.

## Troubleshooting

**The file cannot be retrieved.** Check that the link is publicly reachable and
points directly at the audio file, not at a page around it.

**It says the format is not supported.** Convert the recording to WAV, MP3 or M4A.
WhatsApp often delivers a different format.

**No analysis comes back.** The recording is probably silent or unintelligible. In
that case the credits are refunded.

**I wanted the literal text.** Use [Audio Transcription](transcriptie.md); that one
writes it out word for word.

## Frequently asked questions

**What is the difference with Audio Transcription?**
Transcription gives you the words, this skill gives you the meaning and the tone.
Transcription charges per minute and is built for long recordings; this skill has a
fixed price and is built for short messages.

**Can I forward a WhatsApp voicemail directly?**
You can send the file along in the chat or provide a link. See
[Files](../functies/bestanden.md).

**What if several people are talking?**
That works, but without names. GENI distinguishes the voices as Speaker 1 and 2.

**Which language do I get the answer in?**
In the language you work in, even if the message was recorded in another language.

---

→ Back to [Skills marketplace](README.md)
→ See also: [Audio Transcription](transcriptie.md) · [WhatsApp Business](whatsapp-business.md) · [Files](../functies/bestanden.md)
→ On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Voice Message, updated August 2026*
