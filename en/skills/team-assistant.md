# Team Assistant

With the Team Assistant GENI condenses long team conversations into what was decided and who has to do what, so a Slack channel that ran on is no longer a backlog.

Available from **Pro**. Works with pasted text; with [Slack](slack.md) connected
it fetches the messages itself.

## What can GENI do with it?

- **Summarise a team update** , a Slack thread, meeting note or long email chain reduced to the essentials
- **Extract action items** , who does what, with a deadline where one was given
- **Fetch Slack messages** from a channel (requires a connected Slack workspace)

The first two work without a connection too: paste the text and you get the same
result.

## Example: what you ask, what you get

```
Summarise #project-dekrent from this week and pull out the action items
```

> **#project-dekrent , 4 to 8 August, 63 messages**
>
> **What it was about**
> Delivery moved from week 38 to week 40 because the POS integration needs an
> extra test round. The client agreed, the planning has been updated.
>
> **Decided**
> - Delivery in week 40
> - Extra test round on the POS integration, run by the client themselves
>
> **Action items**
>
> | Who | What | When |
> |---|---|---|
> | Sanne | Update the planning and confirm with the client | Friday |
> | You | Supply the test script | Wednesday |
> | Unassigned | Who does the final check? | , |
>
> That last one was raised in the channel but never assigned.

## Requirements

- **Plan:** Pro and up
- **Connection:** none, unless you want messages fetched from Slack. See [Connecting Slack](../connectors/slack.md)

## Activating

1. Go to **Dashboard -> Skills** and activate **Team Assistant**
2. Optionally connect Slack through **Dashboard -> Connectors**
3. Paste a conversation, or name the channel you want summarised

## What it costs

| Action | Credits |
|---|---|
| Summarise a team update | 5 |
| Extract action items | 5 |
| Fetch Slack messages | 3 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI does not reply on your behalf.** It reads and summarises; posting is yours or through the [Slack skill](slack.md).
- **Only channels the connection can reach.** Direct messages and private channels without access stay out of view.
- **Action items are a proposal.** An assignment not stated explicitly in the conversation is inferred , check it before passing it on.
- **Very long periods are read partially.** Ask per week or per thread rather than per month.
- **It schedules nothing.** Ask [Google Calendar](google-calendar.md) or your [Workspace](../functies/werkruimte.md) to turn it into actual tasks.

## Troubleshooting

**The channel is not found.** The Slack connection has no access to it. Invite the app into the channel, or paste the messages.

**The summary misses the point.** Say what you are watching for: decisions, blockers, or only what touches you.

**Action items sit with the wrong person.** In a busy channel the assignment is often implicit. Correct it before you share.

**I want this every Monday.** Set it as a [scheduled task](../handleiding/geplande-taken.md); a weekly summary on Monday morning is the most common form.

## Frequently asked questions

**Does this work without Slack?**
Yes. Paste the text from any source , Teams, email, minutes , and you get the
same result.

**What is the difference with the Meeting Assistant?**
[That one](meeting-assistant.md) works from a recording or transcript of a
single meeting. The Team Assistant works on ongoing team communication.

**Can it stage the action items as tasks?**
Yes, ask it to put them in your [Workspace](../functies/werkruimte.md).

**Does it read along in my Slack?**
Only when you ask, and only in channels the connection has access to. Nothing
runs in the background.

---

Back to [Skills marketplace](README.md)
See also: [Slack](slack.md) · [Meeting Assistant](meeting-assistant.md) · [Workspace](../functies/werkruimte.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Team Assistant, updated August 2026*
