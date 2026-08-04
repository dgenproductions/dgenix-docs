# Connect YouTube

The YouTube connector gives GENI read access to your channel, so it can pull statistics, analyse comments and turn that into video ideas and upload checklists.

## What you can do with it

| What GENI does | Example |
|---|---|
| Pull channel statistics | "How did my channel do this month?" |
| Per-video statistics | "How much watch time did my last video get?" |
| Analyse comments | "Which questions keep coming up under my last 3 videos?" |
| Analytics report | "Build a report on watch time, CTR and traffic sources" |
| Audience insights | "When is the best time for me to upload?" |
| Generate video ideas | "Give me 10 ideas that fit my best performing content" |
| Build an upload checklist | "Write an SEO title, description and tags for this video" |

The connection activates the **[YouTube Manager skill](../skills/youtube.md)**, available from Growth.

## Connecting

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to YouTube Manager
3. Sign in with the Google account linked to your YouTube channel
4. Grant dGENIX the requested permissions (YouTube and Analytics)
5. The window closes by itself and the connection is live

> Connected YouTube before? Disconnect and reconnect. The Analytics permissions
> were added later, so older connections lack the analytics report and the
> audience insights.

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| Read YouTube channel data | Statistics, videos and channel info |
| Read YouTube Analytics | Watch time, CTR, traffic sources and upload timing |

The connection is **read-only**. dGENIX does not upload videos, does not change
titles or descriptions, and does not post comments.

## Checking that it works

Right after connecting, ask GENI:

```
How did my YouTube channel perform over the last 30 days?
```

You get subscribers, views and your recent videos. If the analytics report
reports missing permissions, the connection predates the Analytics scopes:
reconnecting fixes it.

## Limits

- Read-only: GENI does not upload, edit or reply
- One channel per connected Google account
- Analytics data lags a few days at YouTube itself
- Comments are analysed for themes, not answered

## Troubleshooting

**Connection fails.** Check that you are signed in to the Google account that owns the channel. A brand account requires its managing account.

**Analytics report returns a permission error.** The connection predates the Analytics scopes. Disconnect and reconnect.

**GENI sees the wrong channel.** Your Google account manages several channels. Disconnect and explicitly pick the right channel when reconnecting.

## Disconnecting

Go to **Dashboard -> Connectors**, click YouTube Manager and choose **Disconnect**.
You can also revoke access at Google itself via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Frequently asked questions

**Can GENI upload videos for me?**
No. The connection is deliberately read-only; you stay in control of what appears on your channel.

**Does this work for a brand account?**
Yes, as long as you connect with the Google account that manages that brand account.

**Do I also need the YouTube skill?**
Yes. The connector handles access, the skill gives GENI the capabilities. Activate it via **Dashboard -> Skills**.

**Can GENI turn my videos into shorts too?**
That is a different skill. The [AI Content Engine](https://dgenix.com/engines/ai-content) cuts a
long video into clips with a virality score; this connector is about your
channel statistics.

---

Back to [Connectors overview](README.md)
See also: [YouTube Manager skill](../skills/youtube.md)

*dGENIX Docs, Connect YouTube, updated August 2026*
