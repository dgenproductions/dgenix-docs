# Slack

With the Slack skill GENI reads along in your workspace, summarises threads and posts on your behalf, so you do not have to follow everything yourself.

Available from **Growth**. You need a connected Slack workspace; see
[Connecting Slack](../connectors/slack.md).

## What can GENI do with Slack?

- **Read a channel** and fetch the recent messages
- **Summarise a thread**, including all replies
- **Search messages** for a term
- **List your channels** the connection can reach
- **Post a message** to a channel
- **Send a DM** to a specific colleague
- **React with an emoji** to a message
- **Create a channel**

## Example: what you ask, what you get

```
Summarise the discussion in #release, I was away two days
```

> **#release , 34 messages since Tuesday**
>
> **Decided**
> - The release moves to Thursday, because of the bug in the payment flow
> - Sanne picks up the release notes
>
> **Still open**
> - Who handles customer communication? Jan suggested you, nobody confirmed.
> - Whether the old API version stays up another month; three opinions, no decision.
>
> You were mentioned twice, both times about that customer communication.

That last part is usually why you ask: you want to know whether something is
waiting on you.

## Requirements

- **Plan:** Growth and up
- **Connection:** a Slack workspace via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Slack**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Pick your workspace and grant permission
4. Slack is usable right away

## What it costs

| Action | Credits |
|---|---|
| React with an emoji | ~15 |
| Search messages | ~25 |
| Send a message or DM | ~30 |
| Read and summarise a channel | ~40 |
| Summarise a thread | ~50 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Posting and sending DMs ask for confirmation.** You see the text first.
- **GENI does not delete messages or channels.**
- **Private channels are only visible** if the app has been invited (`/invite @dGENIX`).
- **It does not read along continuously.** Messages are fetched when you ask.
- **Files in Slack are recognised but not opened.**
- **On a free Slack workspace** Slack itself limits the retained history.

## Troubleshooting

**A channel is not visible.** It is private. In Slack, type `/invite @dGENIX` in that channel.

**Posting fails.** Your workspace may not allow apps to post. Ask your admin to approve the app.

**A summary lacks context.** Name the period ("since Monday") and GENI fetches more messages.

**Older messages cannot be found.** On a free workspace Slack retains only limited history.

## Frequently asked questions

**Can GENI post to a channel automatically?**
Yes, as a scheduled task, for example a weekly summary in your team channel
every Monday. The confirmation still applies. See
[Scheduled tasks](../handleiding/geplande-taken.md).

**Does it read all my Slack messages?**
No. Only what your request needs, at the moment you ask.

**Can I connect several workspaces?**
One per account. Switching means disconnecting and connecting again.

**Can it put a report from another skill into Slack?**
Yes, and that is a strong combination: a [weekly report](weekly-report.md) or
SEO audit appearing in your team channel by itself.

---

Back to [Skills marketplace](README.md)
See also: [Connecting Slack](../connectors/slack.md) · [Weekly report](weekly-report.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Slack, updated August 2026*
