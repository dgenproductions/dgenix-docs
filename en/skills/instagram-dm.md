# Instagram DM

With the Instagram DM skill GENI reads your Business inbox, sorts every message by type and drafts replies.

That sorting is the most useful part: with dozens of DMs a day you see at a
glance which ones actually matter. Available from **Growth**; see
[Connecting Instagram Business](../connectors/instagram.md).

## What can GENI do with Instagram DM?

- **Read your Business inbox** and fetch the recent DMs
- **Classify a message** as spam, FAQ, lead or appointment request
- **Send a DM** to an account

## Example: what you ask, what you get

```
Which DMs today are actually worth it?
```

> **23 DMs, sorted**
>
> | Type | Count |
> |---|---|
> | Lead | 3 |
> | Appointment request | 2 |
> | FAQ | 9 |
> | Spam | 9 |
>
> **The 3 leads:**
> - **@sportschool_veldhoven** , asking for a quote for 40 people
> - **@marieke.k** , wants to know whether you also work in Tilburg
> - **@bouwbedrijf_jansen** , asking about a partnership
>
> The 9 FAQs are almost all about your opening hours. Shall I draft one answer
> you can reuse?

## Requirements

- **Plan:** Growth and up
- An Instagram **Business** account, not a personal one
- Linked to a Facebook page in Meta Business Manager
- A **Meta Developer account** with an approved app

## Activating

1. Go to **Dashboard -> Skills** and activate **Instagram DM**
2. Go to **Dashboard -> Connectors** and enter your Meta credentials
3. Set up the webhook in Meta, otherwise you receive no DMs
4. Instagram DM is usable

## What it costs

| Action | Credits |
|---|---|
| Read and summarise DMs | ~50 |
| Draft and send a reply | ~80 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Sending asks for confirmation.**
- **Meta only allows free-form text within 24 hours** of the customer's last message.
- **Text only.** Images, story replies and voice notes are not supported.
- **DMs only.** Comments under posts are not read or answered.
- **GENI does not delete messages or block accounts.**
- **The classification is an estimate**, not a certainty. Check the leads yourself.

## Troubleshooting

**No DMs come in.** The webhook is not set up correctly. Check the URL, the Verify Token and the `messages` subscription.

**Your account is rejected.** It is probably a personal or Creator account. Switch it to Business and link it to a Facebook page.

**A real lead was marked as spam.** The classification is an estimate. Ask for the full list if you do not want to miss anything.

**Sending fails.** The 24-hour window has expired, or the account has blocked you.

## Frequently asked questions

**Does GENI reply to DMs automatically?**
Only if you schedule it. By default it reads and sorts, and you decide.

**Can I connect my personal Instagram?**
No. Meta only grants Business accounts access to the DM API.

**Can I combine this with WhatsApp?**
Yes, then one request covers what came in across both channels. See
[WhatsApp Business](whatsapp-business.md).

**Can it answer comments under my posts?**
No, those fall outside this connection.

---

Back to [Skills marketplace](README.md)
See also: [Connecting Instagram Business](../connectors/instagram.md) · [WhatsApp Business](whatsapp-business.md) · [Social Media Manager](social-media.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Instagram DM, updated August 2026*
