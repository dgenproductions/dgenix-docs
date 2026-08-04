# Audio Transcription

With the Transcription skill GENI turns audio and video into text, and summarises it right away if you ask.

Available from **Growth**. No connection needed; you give a URL or attach a file.

## What can GENI do with transcription?

- **Turn audio or video into text**, with a choice of two quality levels
- Then **summarise, extract action items or translate**, because once it is text
  GENI can do anything with it that it does with text

That second part is the point. A raw transcript of an hour-long meeting is still
an hour of reading; the summary is what you are after.

## Example: what you ask, what you get

```
Transcribe this recording and give me the action items
```

> **Meeting, 47 minutes, 4 speakers**
>
> **Decided**
> - The De Vries quote goes out this week, with a 10 percent discount
> - The maintenance contract will not be renewed
>
> **Action items**
> - **You** , finish the De Vries quote, before Friday
> - **Sanne** , call the supplier about the lead time
> - **Nobody yet** , who takes on customer communication?
>
> **Worth noting:** around minute 31 an 8 percent price increase is mentioned
> that was never formally decided.
>
> The full transcript is in your Workspace.

## Requirements

- **Plan:** Growth and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **Audio Transcription**
2. Give a URL to the file, or attach it in the chat

## What it costs

| Quality | Speed | Credits |
|---|---|---|
| Turbo, default | Fast | 12 per minute |
| Large | Slower, maximum quality | 20 per minute |

A 30-minute recording on Turbo therefore costs about 360 credits. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **The price runs per minute of audio.** A long recording adds up; check the length first.
- **Speakers are not identified by name.** GENI distinguishes voices but does not know who is who unless the conversation makes it clear.
- **Background noise and people talking over each other** noticeably reduce quality.
- **Up to 200 MB via a URL.** Larger files you split.
- **An attachment in chat is more limited**; for long audio use a URL.
- **Nothing is translated unless you ask.** The transcript follows the spoken language.

## Troubleshooting

**The transcript is full of errors.** Usually background noise or overlapping speakers. Try the Large quality; it is slower but noticeably better.

**It cost more credits than expected.** The price is per minute. An hour-long podcast is 720 credits on Turbo.

**The file cannot be fetched.** Check that the URL is publicly reachable and points directly at the file, not at a page around it.

**Jargon comes out wrong.** Mention the terms in your request and GENI takes them into account when summarising.

## Frequently asked questions

**Which file formats work?**
The common audio and video formats: mp3, mp4, wav, m4a and webm.

**What is the difference with attaching a file in chat?**
An attachment is transcribed too, at the same per-minute rate. This skill is
meant for longer recordings via a URL. See [Files](../functies/bestanden.md).

**Can it summarise a meeting while it is running?**
No, it works on a recording afterwards. For live meetings the
[Meeting Assistant](meeting-assistant.md) is the one.

**Where does the transcript end up?**
In your Workspace, so you can find it back later.

---

Back to [Skills marketplace](README.md)
See also: [Meeting Assistant](meeting-assistant.md) · [Files](../functies/bestanden.md) · [Workspace](../functies/werkruimte.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Audio Transcription, updated August 2026*
