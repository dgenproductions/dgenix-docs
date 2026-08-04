# Google Analytics

With the Google Analytics skill you ask for your visitor figures in plain language, instead of clicking your way through the Analytics dashboard.

Available from **Growth**. You need a connected Google account with access to
the GA4 property.

## What can GENI do with Google Analytics?

- **A traffic overview**: sessions, users and bounce rate
- **Your best-visited pages**, with sessions and average time on page
- **Traffic source analysis**: organic, social, direct and paid
- **Audience insights**: devices, countries and returning visitors

## Example: what you ask, what you get

```
How did my website do last month?
```

> **July 2026** , 3,480 sessions from 2,910 users *(+12% vs June)*
>
> | Source | Sessions | Share |
> |---|---|---|
> | Organic search | 1,910 | 55% |
> | Direct | 780 | 22% |
> | Social | 560 | 16% |
> | Other | 230 | 7% |
>
> Your bounce rate went from 61% to 54%, mostly thanks to the services page.
> That drew 340 sessions with an average time of 2:40, well above your site
> average.
>
> Worth noting: social grew 40%, but those visitors stay 22 seconds on average.
> There is gain to be had there.

## Requirements

- **Plan:** Growth and up
- **Connection:** a Google account with access to the GA4 property

## Activating

1. Go to **Dashboard -> Skills** and activate **Google Analytics**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Complete the Google consent screen
4. Analytics is usable right away

## What it costs

| Action | Credits |
|---|---|
| Best-visited pages | 30 |
| Traffic overview | 35 |
| Traffic sources | 35 |
| Audience insights | 40 |

The skill is included in your plan; you pay per action. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GA4 only.** The old Universal Analytics is not supported; Google switched it off.
- **You only see properties your account can reach.**
- **The skill reads, it changes nothing.** Goals, filters and events you configure in Analytics itself.
- **No realtime data.** Expect figures up to yesterday.
- **Custom dimensions and events are not read**, only the standard reports.

## Troubleshooting

**No data comes through.** Your account has no access to the property, or GA4 has not been set up. Check that in Analytics itself.

**The figures differ from Search Console.** That is expected. [Search Console](google-search-console.md) counts impressions and clicks in Google; Analytics counts what happens on your site. Differences are normal.

**You see fewer visitors than expected.** Cookie banners and ad blockers mean part of your traffic is never measured. That applies to everyone.

**You have several properties.** Name the site and GENI picks the right one.

## Frequently asked questions

**Can I have a monthly report sent?**
Yes, as a scheduled task with the outcome by email. See
[Scheduled tasks](../handleiding/geplande-taken.md).

**Can GENI combine this with other data?**
Yes, and that is the value: together with
[Search Console](google-search-console.md) you see not just how many visitors
arrive, but what they found you on.

**Does this work for client sites?**
Yes, provided your account has access. Work per client in a
[project](../functies/projecten.md).

**Is this the same as the SEO Engine?**
No. Analytics tells you what happened; the [SEO Engine](seo-engine.md) tells you
what to improve.

---

Back to [Skills marketplace](README.md)
See also: [Google Search Console](google-search-console.md) · [SEO Engine](seo-engine.md) · [Weekly report](weekly-report.md)
On the site: [the five Growth Engines](https://dgenix.com/engines) · [free scan](https://dgenix.com/demo)

*dGENIX Docs, Google Analytics, updated August 2026*
