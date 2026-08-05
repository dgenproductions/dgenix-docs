# Invoice Automator

With the Invoice Automator GENI builds a complete invoice from a few lines of text, works out the VAT and puts the file in your Drive.

Available from **Pro**. Saving to Drive needs
[Google Drive](google-drive.md).

## What can GENI do with it?

- **Create an invoice** with client details, line items, VAT percentage and an invoice number (or auto-numbered)
- **Save the invoice to Google Drive**

## Example: what you ask, what you get

```
Invoice for De Krent: website build 1x 1500, POS integration 1x 850,
maintenance 3 months at 95
```

> **Invoice 2026-085 , De Krent**
>
> | Description | Qty | Amount |
> |---|---|---|
> | Website build | 1 | € 1,500.00 |
> | POS integration | 1 | € 850.00 |
> | Maintenance (per month) | 3 | € 285.00 |
>
> Subtotal € 2,635.00
> VAT 21 percent € 553.35
> **Total € 3,188.35**
>
> Payment term 14 days.
>
> Shall I put it in your Drive? I have no address for De Krent, which you
> probably want on there.

## Requirements

- **Plan:** Pro and up
- **Connection:** none to create the invoice. [Google Drive](google-drive.md) to save it

## Activating

1. Go to **Dashboard -> Skills** and activate **Invoice Automator**
2. Optionally connect Google Drive through **Dashboard -> Connectors**
3. Name the client and the line items

## What it costs

| Action | Credits |
|---|---|
| Create an invoice | 20 |
| Save to Drive | 5 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **No accounting integration.** The invoice does not land in your accounting package; that is yours to do, or through the Invoicing skill with Moneybird.
- **It sends nothing.** Emailing is yours or through [Gmail](gmail.md).
- **VAT calculation is arithmetic, not advice.** Reverse charge, intra-EU supplies and non-standard rates are yours to check.
- **Invoice numbers continue from what you give it.** It does not know your books, so the sequence is yours to guard.
- **No payment status.** Whether you were paid is not something it knows , [Stripe Insights](stripe-insights.md) or Moneybird covers that.

## Troubleshooting

**The line items come out wrong.** Use one line per item with description, quantity and amount. "Website build 1x 1500" works better than a running sentence.

**Wrong VAT percentage.** State it explicitly; by default it uses 21 percent.

**Saving to Drive fails.** Google Drive is not connected or the permissions were revoked. Reconnect through Connectors.

**The invoice number jumps.** Say what the previous one was and it counts on.

## Frequently asked questions

**What is the difference with the Invoicing skill?**
Invoicing works with Moneybird: the draft invoice appears in your actual books.
The Invoice Automator produces a standalone document.

**Can it email the invoice?**
Not by itself. With [Gmail](gmail.md) connected it can, and it asks for
confirmation first.

**Can I use my own house style?**
Company details and payment terms, yes. For a properly designed invoice an
accounting package is a better fit.

**Does it handle recurring invoices?**
If you ask. Set a monthly invoice as a
[scheduled task](../handleiding/geplande-taken.md).

---

Back to [Skills marketplace](README.md)
See also: [Stripe Insights](stripe-insights.md) · [Google Drive](google-drive.md) · [Weekly Report](weekly-report.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Invoice Automator, updated August 2026*
