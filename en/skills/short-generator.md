# Short Generator

With the Short Generator you send a video URL and GENI cuts short clips out of it automatically, suitable for Shorts, Reels and TikTok.

Available from **Starter**. No connection needed.

## What can GENI do with the Short Generator?

- **Analyse a video** and propose the usable fragments before anything is cut
- **Produce the clips** based on that analysis
- **Check the status** while processing runs

That first step is worth using: you see what it wants to cut before spending
credits on the cutting itself.

## Example: what you ask, what you get

```
Analyse this video and make 3 shorts from it
```

> **12-minute video, 5 usable moments found**
>
> | Fragment | Time | About |
> |---|---|---|
> | 1 | 1:14-1:52 | The remark about scaling too early |
> | 2 | 4:03-4:41 | The example of the failed campaign |
> | 3 | 7:28-8:02 | Concrete tip on pricing |
>
> These three have a clear opening line and do not cut off mid-sentence. Shall I
> cut them? That costs about 1,850 credits.

## Requirements

- **Plan:** Starter and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **Short Generator**
2. Give a video URL and say how many clips you want

## What it costs

| Case | Length | Clips | Credits |
|---|---|---|---|
| Short test | 5 min | 1 | ~1,000 |
| Standard | 10 min | 3 | ~1,850 |
| Podcast excerpt | 30 min | 5 | ~3,950 |
| Long video | 60 min | 10 | ~7,400 |

The price depends on the source video's length *and* the number of clips. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **The video has to be publicly reachable.** Private, unlisted or behind a login does not work.
- **Spoken content works best.** Detection leans on the transcript, so music without speech yields little.
- **No automatic publishing.** You download the clips and post them yourself.
- **The crop is optimised for vertical**; widescreen gets cropped.
- **Processing takes minutes, not seconds.**
- **Failed runs are refunded.**

## Troubleshooting

**The video cannot be fetched.** Test the URL in an incognito window; if you cannot see it there, neither can we.

**Clips start mid-sentence.** Ask for the analysis first and pick the fragments yourself.

**Few moments are found.** With a video without clear statements or stories there is little to cut.

**It costs more than expected.** Both the source video's length and the number of clips count. Analyse first, cut after.

## Frequently asked questions

**What is the difference with the AI Content Engine?**
The Short Generator cuts clips. The
[AI Content Engine](ai-content-engine.md) adds a virality score, three title
variants, a caption and hashtags, so you get a ranking and ready-to-use copy.
That one sits in Pro.

**Which sources are supported?**
YouTube URLs and direct links to a video file.

**Where do the clips end up?**
In your Workspace, Files tab.

**May I make clips from someone else's video?**
Technically you can, legally it is your responsibility.

---

Back to [Skills marketplace](README.md)
See also: [AI Content Engine](ai-content-engine.md) · [Content Repurposing](content-repurposing.md) · [Files](../functies/bestanden.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Short Generator, updated August 2026*
