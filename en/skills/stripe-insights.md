# Stripe Insights

With Stripe Insights you ask about your revenue, failed payments and customer records in plain language, without opening the Stripe dashboard.

Available from **Growth**. You need a connected Stripe account; the connection is
read-only.

## What can GENI do with it?

- **Fetch a revenue overview** for a period: revenue, number of payments, refunds
- **Fetch failed payments** , which ones, from whom, and why they failed
- **Look up a customer** with their payment history and subscription status

## Example: what you ask, what you get

```
How did July go?
```

> **July 2026**
>
> | | |
> |---|---|
> | Revenue | € 14,280 |
> | Payments | 47 successful |
> | Failed | 6 |
> | Refunded | € 340 (2 items) |
>
> June was € 12,910, so **+10.6 percent**.
>
> Of those 6 failed payments, 4 failed for the same reason: insufficient funds,
> all on the 1st of the month. That is € 592 together which is probably
> collectable with a second attempt later in the month.

And specifically:

```
What is the status of customer De Krent?
```

> **De Krent** , customer since March 2026
> Subscription **active**, € 95 per month, next charge 12 August.
> Total paid: € 475 across 5 invoices, no failed payments.

## Requirements

- **Plan:** Growth and up
- **Connection:** Stripe through **Dashboard -> Connectors**. See [Connecting Stripe](../connectors/stripe.md)

## Activating

1. Go to **Dashboard -> Skills** and activate **Stripe Insights**
2. Connect your Stripe account through **Dashboard -> Connectors**
3. Ask about your revenue

## What it costs

| Action | Credits |
|---|---|
| Revenue overview | 25 |
| Failed payments | 15 |
| Look up a customer | 10 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Read-only.** GENI creates no payments, changes no subscriptions and issues no refunds.
- **No sending invoices.** The [Invoice Automator](invoice-automator.md) covers that.
- **Only what is in Stripe.** Payments outside Stripe (bank, cash, another provider) are unknown to it.
- **Not accounting.** Revenue in Stripe is not the same as revenue in your tax return; costs and VAT are not in there.
- **Customer data is real customer data.** What you request ends up in your conversation, so bear that in mind.

## Troubleshooting

**"No access to Stripe".** The connection expired or the key was revoked. Reconnect through Connectors.

**The figures differ from my dashboard.** Usually a period difference or a different currency. Name the period explicitly.

**It cannot find the customer.** Search on the email address from Stripe; company names often differ from what Stripe holds.

**I see test data.** The connection points at your test environment. Connect the live key.

## Frequently asked questions

**Can it issue refunds?**
No. The connection is deliberately read-only; anything that moves money you do
in Stripe itself.

**Can I get a monthly revenue report?**
Yes, through [Scheduled tasks](../handleiding/geplande-taken.md). An overview in
your inbox on the first of the month is the most common form.

**Does this work with the Financial Overview?**
Yes. [Financial Overview](finance.md) uses your Stripe revenue automatically when
this skill is active.

**Is my payment data safe?**
The connection only reads. See the [privacy policy](https://dgenix.com/privacy) for how data is
stored.

---

Back to [Skills marketplace](README.md)
See also: [Financial Overview](finance.md) · [Invoice Automator](invoice-automator.md) · [Connecting Stripe](../connectors/stripe.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Stripe Insights, updated August 2026*
