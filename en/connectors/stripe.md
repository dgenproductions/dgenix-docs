# Connecting Stripe

The Stripe connection lets GENI fetch your revenue figures, subscriptions and failed payments, so you can ask about them in plain language.

You connect with a **Restricted API Key** you create yourself and set to read
access only. The connection activates the
[Stripe Insights skill](../skills/stripe-insights.md), available from **Growth**.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "How is my revenue doing?" | Returns MRR, ARR, customer count and active subscriptions |
| "Have any payments failed?" | Fetches recent failed payments |
| "What has customer X bought from us?" | Looks up by email address or Stripe customer ID |
| "Send me a revenue summary every Monday" | Combines this with your email connection in a recurring task |

## Connecting

1. Log in to your Stripe Dashboard
2. Go to *Developers -> API Keys -> Restricted Keys*
3. Click **+ Create restricted key** and give it a name, for example "dGENIX read-only"
4. Set these permissions to **Read**:
   - `Balance`, for the balance overview
   - `Charges`, for payments
   - `Customers`, for customer data
   - `Subscriptions`, for subscriptions
   - `Payment Intents`, for transactions
5. Copy the key you receive
6. Go to **Dashboard -> Connectors**, click **Connect** on Stripe and paste the key

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| `Balance` (read) | Balance overview |
| `Charges` (read) | Payments and failed collections |
| `Customers` (read) | Looking up a customer |
| `Subscriptions` (read) | Active subscriptions and MRR |
| `Payment Intents` (read) | Transaction details |

**You do not need write access.** Do not enable it either: that makes it
technically impossible for this connection to ever create or refund a payment.

## Checking that it works

Ask this right after connecting:

```
How is my Stripe revenue doing?
```

You get MRR, ARR and the customer count back. If you get a permissions error, a
`read` permission is missing from your restricted key.

## Limits

- **Read only.** GENI cannot create, refund or cancel a payment
- No changing or cancelling subscriptions
- No editing customer data in Stripe
- Figures come straight from Stripe; they are not stored or tracked
- On very large accounts part of the history is fetched, not all of it

## Troubleshooting

**Permissions error when asking.** A `read` permission is missing. Open the restricted key in Stripe and set the missing resource to Read.

**The key is rejected.** You probably used your publishable key (`pk_...`) or a standard secret key. It has to be a **restricted key** (`rk_...`).

**You see test data.** You created the key in test mode. Switch Stripe to live and create a new restricted key.

## Disconnecting

Revoke the restricted key in Stripe (*Developers -> API Keys*), or go to
**Dashboard -> Connectors**, click Stripe and choose **Disconnect**. A revoked
key stops working immediately.

## Frequently asked questions

**Could GENI move money by accident?**
No. The key has read access only, so the capability does not technically exist,
whatever you ask.

**Can I combine this with other skills?**
Yes, and that is where the value is: a monthly revenue summary that GENI fetches,
condenses and emails you. See [Scheduled tasks](../handleiding/geplande-taken.md).

**Is this the same Stripe account I pay dGENIX with?**
No. This connection is about **your** Stripe account and your customers. Your own
subscription is separate and managed through Billing in the dashboard.

---

Back to [Connectors overview](README.md)
See also: [Stripe Insights skill](../skills/stripe-insights.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting Stripe, updated August 2026*
