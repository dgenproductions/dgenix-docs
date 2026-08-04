# Google Search Console

With the Search Console skill GENI pulls your real Google data: which keywords you are found on, how many clicks that brings and where you sit just outside the top.

This is not an estimate but your own measured data. Available from **Growth**.
You need a connected Google account with access to the property.

## What can GENI do with Search Console?

- **A keyword report** with clicks, impressions, CTR and average position
- **Page performance**: which pages bring the most organic clicks
- **SEO opportunities**: keywords sitting just outside the top, with AI recommendations

That last one is where it gets interesting: position 11 to 20 means you already
register but are not quite found, and that is usually the cheapest gain.

## Example: what you ask, what you get

```
Where are my SEO opportunities?
```

> **3 keywords just off the first page**
>
> | Keyword | Position | Impressions | Clicks |
> |---|---|---|---|
> | heat pump installer eindhoven | 11 | 1,240 | 18 |
> | apply for heat pump subsidy | 13 | 890 | 7 |
> | heat pump cost house | 14 | 2,100 | 11 |
>
> The third keyword has the most impressions and the lowest CTR. Your page on it
> is thin and does not answer the question in the first paragraph. Two positions
> gained here is worth more than ten on the rest.

## Requirements

- **Plan:** Growth and up
- **Connection:** a Google account with access to the Search Console property

## Activating

1. Go to **Dashboard -> Skills** and activate **Search Console**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Complete the Google consent screen
4. Search Console is usable right away

## What it costs

| Action | Credits |
|---|---|
| Page performance | 35 |
| Keyword report | 50 |
| SEO opportunities with recommendations | 450 |

The last one costs more because it involves a full analysis. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **You only see properties your account has access to.**
- **Search Console data lags two to three days.** That is Google's delay, not ours.
- **Low-traffic keywords are withheld by Google** for privacy reasons; nobody can see those.
- **The skill changes nothing on your site.** It reads and advises.
- **No historical data from before your connection.** Google keeps 16 months by default.

## Troubleshooting

**No data comes through.** The property is not verified in Search Console, or your account has no rights to it. Check that in Search Console itself first.

**The figures differ from your analytics.** That is expected: Search Console counts impressions and clicks in Google, [Analytics](google-analytics.md) counts visits on your site. Differences of tens of percent are normal.

**A new page is missing.** Google has to index it first and there has to be traffic. Expect several weeks.

**You see fewer keywords than expected.** Google filters out rare queries.

## Frequently asked questions

**What is the difference with the SEO Engine?**
This skill shows your own Google data: what you are found on right now. The
[SEO Engine](seo-engine.md) analyses your pages and says what to improve.
Together they are stronger: measure where the opportunity is, then improve.

**Can I have this reported monthly?**
Yes, as a scheduled task with the outcome by email. See
[Scheduled tasks](../handleiding/geplande-taken.md).

**Does this work for client sites?**
Yes, provided your account has access to their property. Work per client in a
[project](../functies/projecten.md).

**Do I still need the SEO Engine for this?**
Not necessarily. This skill is free data from your own Google account; the
engine adds analysis and competitor comparison.

---

Back to [Skills marketplace](README.md)
See also: [Google Analytics](google-analytics.md) · [SEO Engine](seo-engine.md) · [Authority Engine](authority-engine.md)
On the site: [the five Growth Engines](https://dgenix.com/engines) · [free scan](https://dgenix.com/demo)

*dGENIX Docs, Google Search Console, updated August 2026*
