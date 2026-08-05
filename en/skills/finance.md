# Financial Overview

With the Financial Overview GENI puts your income, fixed costs and variable spending side by side, and builds a concrete savings plan from it.

Available from **Growth**. No connection needed, though with
[Stripe Insights](stripe-insights.md) it pulls your revenue automatically.

## What can GENI do with it?

- **Analyse your financial picture** , income, fixed costs, variable spending, debts and savings goal in one overview, with a verdict attached
- **Build a savings plan** with a concrete monthly target, and where that has to come from

If you have [Stripe Insights](stripe-insights.md) active, GENI uses your actual
revenue figures. If not, it asks you to state the amounts or paste an overview.

## Example: what you ask, what you get

```
I earn 3,200 net. Rent 1,150, insurance 210, subscriptions 95,
groceries 450, eating out about 200. I want to save 500 a month.
```

> **Financial overview , per month**
>
> | Item | Amount |
> |---|---|
> | Net income | € 3,200 |
> | Fixed costs | € 1,455 |
> | Variable spending | € 650 |
> | **Left over** | **€ 1,095** |
>
> Your € 500 savings goal is comfortably within reach; you still have € 595
> after it.
>
> **What stands out**
> - Your fixed costs are **45 percent** of income. Under 50 is healthy, but the
>   rent weighs heavily.
> - € 95 in subscriptions is a lot for one household. That is usually the item
>   with the quickest win.
> - There is nothing set aside for the unexpected. Reckon on € 100 to € 150 a
>   month, otherwise it eats into your savings.
>
> Shall I build a savings plan towards € 700 a month?

## Requirements

- **Plan:** Growth and up
- **Connection:** none. [Stripe Insights](stripe-insights.md) is optional for automatic revenue figures

## Activating

1. Go to **Dashboard -> Skills** and activate **Financial Overview**
2. State your income and main costs, or paste an overview
3. Ask for an analysis

## What it costs

| Action | Credits |
|---|---|
| Financial analysis | 10 |
| Savings plan | 8 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **This is not financial advice.** No tax advice, no investment advice, no mortgage calculations. For those, see an adviser.
- **There is no bank connection.** GENI does not read your account; you supply the figures yourself or through Stripe.
- **It calculates with what you state.** Forget an item and the overview is wrong, and it cannot tell.
- **No automatic transaction categorisation.** If you paste a long list of debits, group them roughly yourself.
- **Amounts are monthly** unless you say otherwise. Annual costs (insurance, subscriptions) you divide by twelve or flag explicitly.

## Troubleshooting

**The overview is wrong.** Usually an item is missing or an annual amount sits among the monthly ones. State both explicitly.

**The advice is too generic.** Give it a goal: an amount to save, a debt to clear, or a purchase you are saving for.

**It asks for figures I already gave.** Put your fixed data in your [memory](../functies/geheugen.md), then you only mention changes.

**I want my business revenue included.** Activate [Stripe Insights](stripe-insights.md) and it pulls that in itself.

## Frequently asked questions

**Can it read my bank account?**
No. There is no bank connection and there will not be one lightly; you supply
the figures yourself.

**Is this for personal or business use?**
Both work. Personally you supply the amounts; for business the revenue side can
come through [Stripe Insights](stripe-insights.md).

**Does this stay between us?**
Yes. Your data is not used to train AI. See the [privacy policy](https://dgenix.com/privacy).

**Can I get an overview monthly?**
Yes, through [Scheduled tasks](../handleiding/geplande-taken.md), for example on
the first of the month.

---

Back to [Skills marketplace](README.md)
See also: [Stripe Insights](stripe-insights.md) · [Invoice Automator](invoice-automator.md) · [Memory](../functies/geheugen.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Financial Overview, updated August 2026*
