# WhatsApp Business

With the WhatsApp Business skill GENI reads your business inbox and drafts replies, so you do not have to sit behind your phone all day.

Available from **Growth**. You need a number on the WhatsApp Business API; see
[Connecting WhatsApp Business](../connectors/whatsapp-business.md).

## What can GENI do with WhatsApp Business?

- **Read your Business inbox** and fetch the recent incoming messages
- **Send a message** from your business number

In practice that means: have incoming questions summarised, see which ones
actually need action, and have the replies drafted.

## Example: what you ask, what you get

```
What came in on WhatsApp?
```

> **9 messages since yesterday, 4 need action**
>
> - **+31 6 12…** , asks whether you are open on Saturday. *Comes up often.*
> - **+31 6 44…** , still waiting for last week's quote.
> - **+31 6 78…** , reports a fault with the March installation. *Urgent.*
> - **+31 6 21…** , asks about maintenance pricing.
>
> The other 5 are thank-yous and confirmations.
>
> I would take the fault first. Shall I draft a reply?

## Requirements

- **Plan:** Growth and up
- **Connection:** a number on the WhatsApp Business API, through Meta
- A **Meta Developer account** with an approved app

A regular WhatsApp or WhatsApp Business **app** account is not enough.

## Activating

1. Go to **Dashboard -> Skills** and activate **WhatsApp Business**
2. Go to **Dashboard -> Connectors** and enter your Meta credentials
3. Set up the webhook in Meta, otherwise you receive no messages
4. WhatsApp Business is usable

## What it costs

| Action | Credits |
|---|---|
| Read and summarise messages | ~50 |
| Draft and send a message | ~80 |

Meta also charges its own conversation fees; those run through your Meta account
and are separate from your credits. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Sending asks for confirmation.** You read the text before it goes out.
- **Meta only allows free-form text within 24 hours** of the customer's last message. Outside that you need an approved template.
- **Text only.** Sending images, documents and voice notes is not supported.
- **No group conversations.**
- **GENI does not delete messages or block contacts.**
- **No webhook means no incoming messages**, even though sending works.

## Troubleshooting

**No messages come in.** The webhook is not set up correctly. Check the URL, the Verify Token and that you subscribed to `messages`.

**Sending fails outside office hours.** The 24-hour window has probably expired. Use a template approved in Meta instead.

**The token keeps expiring.** Meta issues temporary tokens by default. Create a permanent system user token.

**Meta will not approve your app.** Without an approved app the API does not work. That runs entirely through Meta.

## Frequently asked questions

**Does GENI reply to everything automatically?**
Only if you explicitly schedule that. By default it reads and you decide what
goes back.

**Can I connect my personal WhatsApp?**
No. Only a number on the Business API; that is a Meta requirement.

**Can it handle frequently asked questions itself?**
You can schedule it, with confirmation before sending. For a real answering
script the [AI Receptionist](ai-receptionist.md) is a better fit.

**Can I see WhatsApp and Instagram together?**
Yes. With both connected you can ask in one request what came in across both
channels.

---

Back to [Skills marketplace](README.md)
See also: [Connecting WhatsApp Business](../connectors/whatsapp-business.md) · [Instagram DM](instagram-dm.md) · [AI Receptionist](ai-receptionist.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, WhatsApp Business, updated August 2026*
