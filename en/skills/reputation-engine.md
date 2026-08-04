# Reputation Engine

The [Reputation Engine](https://dgenix.com/engines/reputation) asks your own customers for a Google review, through a branded email with a direct review link, and tracks who responds.

Reviews rarely arrive on their own. Most happy customers never leave one because
nobody asked, or because they could not find the link. This engine removes
exactly those two barriers. Available from **Pro**.

## What the Reputation Engine does

| Part | What it produces |
|---|---|
| **Review link lookup** | The direct "write a review" link for your Google Business Profile |
| **Campaign** | A list of customers you approach in one go |
| **Branded email** | A request with your business name, the link and an unsubscribe option |
| **Status overview** | Per recipient: sent, pending or unsubscribed |

## Example: what you ask, what you get

You ask GENI how your campaigns stand:

> **Campaign "July customers"** , 48 contacts
>
> - Sent: 44
> - Pending: 3
> - Unsubscribed: 1
>
> There are **3 requests ready** to send. Shall I do that? It costs 150 credits.

Say yes and those three go out. Above 25 recipients GENI always asks for
confirmation first, even inside a scheduled task.

## How to set it up

1. Go to **Growth Tools -> Reputation** and create a campaign
2. Enter your business name and click **Find link**; add the town if your business has a common name. You can also paste the link yourself.
3. Add a personal message, optional
4. **Paste your customers' email addresses**, or click **Import from Sheets** and give a Google Sheets link (connect [Google Sheets](../connectors/google-sheets.md) first)
5. Click **Send**

Unsubscribed addresses are skipped automatically; you do not have to watch for
them yourself.

## With GENI

You can ask GENI to look up your review link, report a campaign's status or send
an existing campaign. Creating campaigns and adding contacts happens in the
dashboard, because that is where control over a send list belongs.

Sending can also be [scheduled](../handleiding/geplande-taken.md), for example
every Monday for that week's new customers.

## Safety and GDPR

Review requests are email to real people, so there are deliberate brakes here:

- **Unsubscribe link in every email.** Anyone who unsubscribes goes on a suppression list and never receives another request, not even from a different campaign.
- **Your own customers only.** Bought or scraped lists do not belong here, and they breach the GDPR.
- **Monthly cap per plan**: Pro 500, Business 2,000 requests per month.
- **Confirmation** above 25 recipients.
- **Never writing a review.** GENI asks for one, it does not invent them.

## What it costs

| Action | Credits |
|---|---|
| Review request, per email sent | 50 |
| Review link lookup | 300 |

A failed send is refunded. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Google reviews only.** Trustpilot and other platforms follow later.
- **Email only.** SMS requests are planned as an optional add-on.
- **No replying to reviews.** The engine asks for them; you reply yourself in your Google profile.
- **No filtering out negative reviews.** You cannot pre-select who is likely to be positive; Google does not allow it and it is not fair to readers.
- **No guarantee of a response.** A well-timed ask helps, but whether someone writes stays up to the customer.
- **Reviews cannot be deleted.** Only Google can, and only if their policy is breached.

## Troubleshooting

**The review link is not found.** Add the town name. If your business has no claimed Google Business Profile there is no review link; claim the profile first.

**Emails do not arrive.** Check the addresses for typos and ask the customer to look in their spam folder. Unsubscribed addresses are skipped on purpose.

**The Sheets import reads nothing.** Google Sheets has to be connected and the sheet must contain a column of email addresses. A shared link without a connection does not work.

**You have hit the monthly cap.** The cap runs from your billing date. Wait for the new period or move to Business.

**A customer received two requests.** The same address appears in two campaigns. The suppression list covers unsubscribers, not duplicates within your own lists.

## Frequently asked questions

**Am I allowed to ask customers for a review?**
Approaching your own customers about a service you delivered is allowed, as long
as you offer a way to opt out. That is in every email by default. What is not
allowed is using bought lists.

**Can I write the text myself?**
You add a personal message that goes into the email. The layout and the
unsubscribe link are fixed, so the email stays GDPR-proof.

**Does this work for multiple locations?**
Yes, set up a campaign per location with its own review link.

**What if someone leaves a bad review?**
Then you have valuable feedback and a chance to respond publicly. You reply in
your Google Business Profile.

**I run an agency, can I do this for clients?**
Yes. Work in a separate project per client and lists and context stay apart. See
[Projects](../functies/projecten.md).

---

Next: [GEO Engine](geo-engine.md) · [Authority Engine](authority-engine.md) · [All Growth Tools](../engines/README.md)
On the site: [Reputation Engine](https://dgenix.com/engines/reputation) · [pricing](https://dgenix.com/pricing)

*dGENIX Docs, Reputation Engine, updated August 2026*
