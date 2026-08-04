# Connecting Slack

The Slack connection lets GENI read along and join in inside your workspace: read channels, summarise threads, send messages and search what has already been discussed.

You connect Slack once, in a few clicks. It then activates the
[Slack skill](../skills/slack.md), available from **Growth**.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "What was said in #support today?" | Reads the channel and summarises |
| "Summarise the discussion about the release" | Reads the whole thread including replies |
| "Find where we talked about the new pricing" | Searches messages for a term |
| "Post in #general that the release is live" | Sends a message to a channel |
| "DM Lisa that the quote is ready" | Sends a direct message |
| "Put a thumbs up on Jan's last message" | Adds an emoji reaction |
| "Create a channel #project-dewit" | Creates a new channel |

## Connecting

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to Slack
3. Pick the workspace you want to let GENI into
4. Review the permissions requested and click **Allow**
5. The window closes by itself and Slack shows as **Connected**

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| `channels:read` + `channels:history` | Reading public channels |
| `groups:read` + `groups:history` | Reading private channels the app is in |
| `chat:write` | Posting messages |
| `im:read` + `im:write` | Reading and sending direct messages |
| `search:read` | Searching messages |
| `reactions:write` | Reacting with an emoji |
| `channels:manage` | Creating a channel at your request |
| `users:read` | Reading the member list, to find the right person |
| `files:read` + `files:write` | Fetching and uploading files |

GENI only reaches channels the connection has access to. A private channel the
app is not in stays invisible.

## Checking that it works

Ask this right after connecting:

```
Which Slack channels can you see?
```

You get a list of channel names back. If a channel you expected is missing, it
is a private channel the app has not been invited to yet.

## Limits

- Sending a message asks for confirmation; you see the text first
- GENI never deletes messages, channels or files
- Private channels only become visible once you invite the app
- Messages are only fetched at the moment you ask; nothing is read continuously

## Troubleshooting

**GENI cannot see a channel.** It is a private channel. In Slack, type `/invite @dGENIX` in that channel.

**Posting fails.** Your workspace may not allow apps to post. Ask your Slack admin to approve the app.

**You connected the wrong workspace.** Disconnect, sign out of that workspace in Slack, and connect again.

**Older messages cannot be found.** On a free Slack workspace, Slack itself limits how much history is retained.

## Disconnecting

Go to **Dashboard -> Connectors**, click Slack and choose **Disconnect**. You can
also remove the app via *Slack -> Settings -> Manage apps*.

## Frequently asked questions

**Does GENI read all my Slack messages?**
No. It only fetches what your request needs, at the moment you ask. There is no
background process indexing your workspace.

**Can it post to a channel automatically?**
Yes, through a recurring task, for example a weekly summary in your team channel
every Monday. See [Scheduled tasks](../handleiding/geplande-taken.md).

**Can I connect several workspaces?**
One workspace per account. To switch, disconnect and connect the other one.

---

Back to [Connectors overview](README.md)
See also: [Slack skill](../skills/slack.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting Slack, updated August 2026*
