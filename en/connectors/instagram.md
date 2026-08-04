# Connecting Instagram Business

The Instagram connection lets GENI read incoming DMs from your Business inbox, sort them by type and prepare replies for you.

The connection activates the [Instagram DM skill](../skills/instagram-dm.md),
available from **Growth**. Setup runs through Meta, just like WhatsApp.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "What is in my Instagram DMs?" | Reads the recent incoming messages |
| "Which messages are real leads?" | Sorts each message as spam, question, lead or appointment |
| "Reply that we are open until 18:00" | Sends a DM to that account |
| "Summarise today's DMs" | Lists the questions, with spam filtered out |

The sorting is the most useful part: with dozens of DMs a day you see at a
glance which ones actually matter.

## Requirements

- An Instagram **Business** account, not a personal account
- Linked to a Facebook page in Meta Business Manager
- A Meta Developer account with an approved app

## Connecting

1. In Meta Business Manager go to *Instagram -> API Setup*
2. Copy your **Access Token** and **Business Account ID**
3. Go to **Dashboard -> Connectors** and click **Connect** on Instagram
4. Enter both values and save; the connection is active right away

## Setting up the webhook

Without a webhook GENI can send, but receives no DMs.

1. Go to your Meta App -> *Instagram -> Webhooks*
2. Set the Webhook URL: `https://app.dgenix.com/api/instagram/webhook`
3. Set the Verify Token to the value from **Dashboard -> Connectors -> Instagram**
4. Subscribe to the `messages` event

## What access you grant

| Value | What dGENIX uses it for |
|---|---|
| Access Token | Fetching and sending DMs on behalf of your Business account |
| Business Account ID | Identifying your Instagram Business account |

The connection touches your **DMs** only. Posts, stories, comments and your
follower list stay out of reach.

## Checking that it works

Send a DM to your Business account from another Instagram account, then ask:

```
What is in my Instagram DMs?
```

If you see the test message, the webhook works.

## Limits

- Sending a DM asks for confirmation
- Meta only allows free-form text within **24 hours** of the customer's last message
- Text only; images, story replies and voice notes are not supported
- No reading or replying to comments under posts
- GENI does not delete messages or block accounts

## Troubleshooting

**No DMs come in.** The webhook is not set up correctly. Check the URL, the Verify Token and the `messages` subscription.

**Your account is rejected.** It is probably a personal or Creator account. Switch it to a Business account in the Instagram app and link it to a Facebook page.

**Sending fails.** The 24-hour window has expired, or the account has blocked you.

**Comments under posts are missing.** Those are deliberately outside this connection; only DMs are fetched.

## Disconnecting

Go to **Dashboard -> Connectors**, click Instagram and choose **Disconnect**.
Also remove the webhook in Meta.

## Frequently asked questions

**Can I connect my personal Instagram?**
No. Meta only grants Business accounts access to the DM API.

**Does GENI reply to DMs automatically?**
Only if you schedule that. By default it reads and sorts, and you decide what
goes back.

**Can I combine this with WhatsApp?**
Yes. With both connected you can ask in one request what came in across both
channels.

---

Back to [Connectors overview](README.md)
See also: [Instagram DM skill](../skills/instagram-dm.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting Instagram Business, updated August 2026*
