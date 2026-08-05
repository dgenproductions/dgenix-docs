# Meeting Assistant

With the Meeting Assistant GENI turns a recording or transcript into a summary with decisions and action items, so taking minutes no longer falls to someone.

Available from **Pro**. No connection needed.

## What can GENI do with it?

- **Process a meeting recording or transcript** into a summary with decisions, action items and open points

The distinction it draws is what makes it usable: what was decided, what has to
happen and by whom, and what nobody actually settled.

## Example: what you ask, what you get

```
Take minutes from this recording
```

> **Project meeting De Krent , 47 minutes, 4 participants**
>
> **Decided**
> - Website and POS integration go ahead, delivery week 40
> - Maintenance contract will not be renewed
>
> **Action items**
> - **You** , revise the quote to the new scope, before Friday
> - **Sanne** , supply the copy, by 15 August at the latest
> - **Nobody yet** , who tests the POS integration?
>
> **Still open**
> - An 8 percent price increase was mentioned but not decided
> - Unclear whether the old site stays online after delivery
>
> Shall I put the action items in your Workspace?

That last block is usually the most useful: the things that got mentioned but
that nobody decided on otherwise disappear.

## Requirements

- **Plan:** Pro and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **Meeting Assistant**
2. Attach a recording or paste a transcript

## What it costs

| Action | Credits |
|---|---|
| Draft a follow-up message | ~60 |
| Extract action items | ~80 |
| Generate minutes | ~100 |

Working from an audio file adds transcription on top, which runs per minute. See
[Audio Transcription](transcriptie.md) and
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **It is not in your meeting.** You supply a recording or transcript; it does not listen in live.
- **Speakers are not identified by name** unless the conversation makes it clear.
- **Background noise and people talking over each other** noticeably reduce quality.
- **Action items are a proposal.** Who does what is yours to check; a wrongly assigned action just sits there.
- **It does not send minutes.** Sharing is yours, or through [Gmail](gmail.md).
- **No joining video calls.** There is no bot that sits in on Teams or Meet.

## Troubleshooting

**The minutes miss the point.** Say up front what the meeting was about; with context it pulls the right points out.

**Action items are assigned to the wrong person.** On a recording without clear names it guesses from context. Correct it before you share.

**The transcription is poor.** Background noise or overlapping speakers. Try the higher transcription quality; see [Audio Transcription](transcriptie.md).

**It costs more than expected.** With an audio file you also pay per minute of transcription. An hour-long meeting adds up.

## Frequently asked questions

**Can it listen in during the meeting?**
No. You record with your own tools and supply the recording afterwards.

**What is the difference with Audio Transcription?**
[That one](transcriptie.md) turns speech into text. This skill turns it into
minutes with decisions and action items.

**Can it stage the action items as tasks?**
Yes, ask it to put them in your [Workspace](../functies/werkruimte.md).

**Does this work with a transcript from Teams or Zoom?**
Yes, paste the transcript and you skip the transcription cost.

---

Back to [Skills marketplace](README.md)
See also: [Audio Transcription](transcriptie.md) · [Workspace](../functies/werkruimte.md) · [Google Calendar](google-calendar.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Meeting Assistant, updated August 2026*
