# LinkedIn

With the LinkedIn skill GENI writes and publishes posts on your profile, and fetches the figures for your recent posts.

Available from **Growth**. You need a connected LinkedIn profile; see
[Connecting LinkedIn](../connectors/linkedin.md).

## What can GENI do with LinkedIn?

- **Publish a text post** on your profile
- **Read your profile**: name, headline and profile photo
- **Fetch statistics** for your recent posts: views, likes and comments

The value is mostly in combining: have GENI turn a blog article, a weekly report
or a case study into a post that matches your tone.

## Example: what you ask, what you get

```
Turn my latest blog article into a LinkedIn post
```

> **Draft, 142 words**
>
> Last week a client called with a question I hear often: "why don't we show up
> in ChatGPT when someone asks about our field?"
>
> The answer turned out to be painfully simple. Their robots.txt was blocking
> exactly the bots that could have cited them. For two years.
>
> Three things I now check on every site: […]
>
> **Estimated reading time:** 40 seconds. No hashtags, they do little on
> LinkedIn these days.
>
> Shall I publish it?

And afterwards:

```
How did my last posts do?
```

> | Post | Views | Comments |
> |---|---|---|
> | "The mistake that cost me 40,000" | 4,820 | 31 |
> | "Why AI does not mention you" | 2,140 | 12 |
> | "Three years in business" | 890 | 4 |
>
> Personal stories get over five times the reach of general tips here.

## Requirements

- **Plan:** Growth and up
- **Connection:** a LinkedIn profile via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **LinkedIn**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Sign in to LinkedIn and grant permission
4. LinkedIn is usable right away

> **Note:** LinkedIn has to approve the publishing permission through their
> Developer Program, which can take 1 to 2 weeks. Reading your profile and
> fetching statistics works right away.

## What it costs

| Action | Credits |
|---|---|
| Fetch statistics | ~40 |
| Write and publish a post | ~120 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Publishing always asks for confirmation.** You read the text first.
- **Text posts only.** Images, video, documents and carousels are not supported.
- **Your personal profile only.** Posting to a company page is not supported.
- **GENI does not edit or delete existing posts.**
- **No comments, connection requests or messages.** This skill does not touch your inbox or network.
- **Statistics arrive with a delay.** For a fresh post an empty result is normal.

## Troubleshooting

**Publishing returns a permissions error.** The publishing permission has not been approved by LinkedIn yet. Reading already works; publishing becomes available once they approve.

**Statistics come back empty.** LinkedIn only supplies figures after a while.

**You want to post on your company page.** The connection does not support that. Have GENI write the text and post it yourself.

**The tone is off.** Record your writing style in [Settings](../functies/instellingen.md) or in your [memory](../functies/geheugen.md) and GENI sticks to it.

## Frequently asked questions

**Can GENI post automatically every week?**
Yes, as a scheduled task. You still see the text first; nothing ever goes out
unseen. See [Scheduled tasks](../handleiding/geplande-taken.md).

**Can it turn a blog into a post?**
Yes, that is the most-used combination. See also
[Content Repurposing](content-repurposing.md).

**Does it see my inbox or connections?**
No. The connection grants no access to those.

**What is the difference with the Social Media Manager?**
That schedules content across several channels. This skill is specific to
LinkedIn, including the figures afterwards. See
[Social Media Manager](social-media.md).

---

Back to [Skills marketplace](README.md)
See also: [Connecting LinkedIn](../connectors/linkedin.md) · [Content Repurposing](content-repurposing.md) · [Social Media Manager](social-media.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, LinkedIn, updated August 2026*
