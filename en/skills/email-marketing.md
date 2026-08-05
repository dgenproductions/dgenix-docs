# Email Marketing

With the Email Marketing skill GENI writes a campaign email and sends it to the recipients you supply.

Available from **Pro**.

## What can GENI do with it?

- **Write a campaign email**, with a subject line and structure
- **Send the email** to the addresses you provide

## Example: what you ask, what you get

```
Write an email to our customers about the new maintenance service
```

> **Subject:** Maintenance from now on, without you having to think about it
>
> *(alternative: "New: maintenance at fixed intervals")*
>
> Hi [name],
>
> From September we offer maintenance at fixed intervals, so you no longer have
> to keep track of it yourself. […]
>
> **Length:** 180 words, one clear action at the end.
>
> How many recipients is this going to? At 40 addresses sending costs 600
> credits, plus 10 for the copy.

## Requirements

- **Plan:** Pro and up
- **Connection:** an email connection such as [Gmail](gmail.md) for sending

## Activating

1. Go to **Dashboard -> Skills** and activate **Email Marketing**
2. Describe the message and the audience
3. Supply the recipients

## What it costs

| Action | Credits |
|---|---|
| Write a campaign email | 10 |
| Sending, per email | 15 |

Writing is cheap, sending scales with the number of recipients. Work out the cost
first: 200 recipients is 3,000 credits. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Sending always asks for confirmation**, with the recipient count stated.
- **Your own contacts only.** Bought or scraped lists do not belong here, and breach the GDPR.
- **You have to provide an opt-out yourself.** For commercial email that is a legal requirement; GENI does not add one automatically.
- **No open and click statistics.** This skill sends; it does not measure.
- **No automated email flows.** For a sequence over time, use a real email marketing tool.
- **No layout or templates.** You get text.

## Troubleshooting

**The email reads like an advert.** Ask for one message and one action. Campaign emails that want three things at once rarely work.

**Sending fails.** No email connection is active, or an address contains a typo.

**The cost is higher than expected.** The rate is per recipient. For large lists a dedicated email tool is cheaper; this skill is meant for smaller, targeted sends.

**Emails land in spam.** That depends on your sending domain and reputation, not on the copy. Make sure your domain is configured correctly for email.

## Frequently asked questions

**Am I allowed to email customers?**
Approaching existing customers about a related service is allowed, provided you
offer an opt-out. Cold lists carry stricter rules.

**What is the difference with the Reputation Engine?**
[That one](reputation-engine.md) sends review requests with a built-in
unsubscribe link and suppression list. This skill is more general and leaves that
responsibility with you.

**Can I schedule it?**
Yes, but with confirmation before sending. A campaign going out unseen is exactly
what you do not want.

**Can it pull the list from my CRM?**
With [HubSpot](hubspot.md) connected you can have contacts fetched; the selection
is yours to make.

---

Back to [Skills marketplace](README.md)
See also: [Gmail](gmail.md) · [Reputation Engine](reputation-engine.md) · [HubSpot CRM](hubspot.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Email Marketing, updated August 2026*
