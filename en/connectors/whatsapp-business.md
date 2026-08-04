# Connecting WhatsApp Business

The WhatsApp Business connection lets GENI read incoming messages from your Business inbox and send replies from your business number.

This is the heaviest connection to set up, because Meta requires a Developer
account and an approved app. Allow half an hour. The connection activates the
[WhatsApp Business skill](../skills/whatsapp-business.md), available from
**Growth**.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "What came in on WhatsApp?" | Reads the recent incoming messages |
| "Reply that we open at 10:00 tomorrow" | Sends a message to that number |
| "Summarise today's conversations" | Reads the inbox and lists the questions |
| "Answer new questions about opening hours automatically" | Runs as a recurring task, with confirmation before sending |

## Requirements

- A Meta Developer account
- An approved WhatsApp Business app in Meta Business Manager
- A phone number linked to the WhatsApp Business API

A regular WhatsApp or WhatsApp Business **app** account is not enough; it has to
run through the API.

## Connecting

1. In Meta Business Manager go to *WhatsApp -> API Setup*
2. Copy your **Access Token**, **Phone Number ID** and **Business Account ID**
3. Go to **Dashboard -> Connectors** and click **Connect** on WhatsApp Business
4. Enter the three values and save; the connection is active right away

## Setting up the webhook

Without a webhook GENI can send, but receives nothing.

1. Go to your Meta App -> *WhatsApp -> Configuration*
2. Set the Webhook URL: `https://app.dgenix.com/api/whatsapp/webhook`
3. Set the Verify Token to the value from **Dashboard -> Connectors -> WhatsApp**
4. Subscribe to the `messages` event

## What access you grant

| Value | What dGENIX uses it for |
|---|---|
| Access Token | Fetching and sending messages on behalf of your Business account |
| Phone Number ID | Determining which number a message goes out from |
| Business Account ID | Identifying your WhatsApp Business account |

## Checking that it works

Send a message from your own phone to your business number, then ask:

```
What came in on WhatsApp?
```

If you see your test message, the webhook works. If it stays empty while sending
does work, the webhook is not set up correctly.

## Limits

- Sending a message asks for confirmation
- Meta only allows free-form text within **24 hours** of the customer's last message; outside that you need an approved template
- Text only; sending images, documents and voice notes is not supported
- GENI does not delete messages or block contacts
- Group conversations are not supported

## Troubleshooting

**No messages come in.** The webhook is not set up correctly. Check the URL, the Verify Token and that you subscribed to `messages`.

**Sending fails outside office hours.** The 24-hour window has probably expired. Use a template approved in Meta instead.

**The token expires.** Meta issues temporary tokens by default. Create a permanent system user token in Meta and update it in Connectors.

**Meta will not approve your app.** Without an approved app the API does not work. That runs entirely through Meta; dGENIX cannot speed it up.

## Disconnecting

Go to **Dashboard -> Connectors**, click WhatsApp Business and choose
**Disconnect**. Also remove the webhook in Meta, otherwise Meta keeps trying to
deliver.

## Frequently asked questions

**Can I connect my personal WhatsApp?**
No. Only a number on the WhatsApp Business API; that is a Meta requirement.

**Does GENI reply to everything automatically?**
Only if you explicitly schedule that. By default it reads and you decide what
goes back, with confirmation before sending.

**Does a message cost credits?**
Yes, sending and reading cost credits inside dGENIX. Meta also charges its own
conversation fees; those run through your Meta account.

---

Back to [Connectors overview](README.md)
See also: [WhatsApp Business skill](../skills/whatsapp-business.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting WhatsApp Business, updated August 2026*
