# YouTube Manager

With the YouTube Manager GENI reads the figures from your own channel, analyses your comments and audience, and works out from that what you should make next.

Available from **Growth**. You need a connected YouTube account. The skill reads
only; uploading is not possible.

## What can GENI do with it?

- **Analyse your channel** , subscribers, views, which videos land and which do not
- **Generate video ideas** based on what works on your channel
- **Build an upload checklist** , title, description, tags, thumbnail advice
- **Fetch video statistics** for a specific video
- **Analyse comments** , what viewers ask, where the criticism sits, which topics keep coming back
- **Build an analytics report** over a period
- **Give audience insights** , who watches, when, and how long they stay

## Example: what you ask, what you get

```
Analyse my comments from the last month
```

> **312 comments across 6 videos**
>
> **What gets asked most**
> - "Does this work without a subscription?" , 23 times, mostly under the tutorials
> - "Where do I find the file?" , 18 times. Your link is in the description but
>   below the fold; viewers do not see it.
>
> **Where the criticism sits**
> - The audio in video 4 is too quiet, 9 separate remarks
> - Two viewers find the intro too long (46 seconds)
>
> **Topics viewers suggest themselves**
> - A comparison with the free version (mentioned 11 times)
> - A follow-up to the installation video (7 times)
>
> Answering that first question in the opening 30 seconds probably halves your
> comment load.

## Requirements

- **Plan:** Growth and up
- **Connection:** YouTube through **Dashboard -> Connectors**. See [Connecting YouTube](../connectors/youtube.md)

## Activating

1. Go to **Dashboard -> Skills** and activate **YouTube Manager**
2. Connect your YouTube account through **Dashboard -> Connectors**
3. Ask for a channel analysis

## What it costs

| Action | Credits |
|---|---|
| Analyse channel | 10 |
| Video statistics | 25 |
| Audience insights | 30 |
| Analyse comments | 35 |
| Upload checklist | 40 |
| Analytics report | 40 |
| Generate video ideas | 50 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Read-only.** GENI uploads no videos, changes no titles and replies to no comments.
- **Your own channel only.** Someone else's analytics are not public; public statistics for a single video are.
- **Analytics lags by a day or two**, which is YouTube itself.
- **A new channel returns little.** Below a few hundred views there is too little data for a meaningful pattern.
- **No thumbnail creation.** It advises on them; the image you generate with [AI Image Generation](ai-beeldgeneratie.md).

## Troubleshooting

**"No access to analytics".** The connection was made before the analytics scope was added. Disconnect and reconnect.

**The figures differ from YouTube Studio.** Analytics lags and Studio sometimes uses a different period. Name the period explicitly.

**It cannot find my video.** Give the video URL or the exact title.

**The ideas do not fit my channel.** Say who you make for and what you do not want; without that it fills in with what works on average.

## Frequently asked questions

**Can it upload videos?**
No. The connection is deliberately read-only.

**Does this work with Shorts?**
Yes, Shorts sit in the same statistics. For *making* shorts there is the
[Short Generator](short-generator.md).

**Can I get a weekly report?**
Yes, through [Scheduled tasks](../handleiding/geplande-taken.md), for example an
analytics report in your inbox every Monday.

**What is the difference with the AI Content Engine?**
[That one](ai-content-engine.md) cuts clips from your videos. The YouTube
Manager analyses your channel and thinks along about what you make.

---

Back to [Skills marketplace](README.md)
See also: [Short Generator](short-generator.md) · [AI Content Engine](ai-content-engine.md) · [Connecting YouTube](../connectors/youtube.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, YouTube Manager, updated August 2026*
