# SEO Engine

## What does this skill do?

The [SEO Engine](https://dgenix.com/engines/seo) analyses your web pages on all technical SEO factors: on-page elements, content quality, technical health and site structure. You get an overall score, sub-scores per category, a list of issues found and priority actions to rank higher on Google.

## Requirements

- **Plan:** Growth+
- **Integrations:** none, the audit analyses your public web page directly

## How do you activate the skill?

1. Go to **Dashboard -> Skills** and activate the **SEO Engine**
2. Go via the side menu to **Growth Tools -> SEO Engine**
3. Enter your page URL and click the **+** button
4. Choose an audit depth and start

## What can you do with it?

### Website audit

Run an audit on any page you want to improve. Choose from four depths:

| Type | Content | Credits |
|---|---|---|
| Quick Check | Basic scores, on-page elements | 1,500 cr |
| Standard Audit | Full analysis, 4 categories, 5 pages | 4,000 cr |
| Deep Audit | Up to 10 subpages analysed | 10,000 cr |
| **Max Audit** | Deep + JS rendering + real Core Web Vitals + keyword positions & search volume | 22,000 cr |

### What is measured?

**SEO Score**, weighted overall score of the four categories (0-100).

**On-Page**, title tag, meta description, H1-H3 headings, alt texts, internal links.

**Content**, readability, keyword density (if provided), text length, unique-content signals.

**Technical**, HTTPS, canonical tag, viewport meta, **real Core Web Vitals** (LCP/INP/CLS via Google PageSpeed, mobile/desktop selectable), Open Graph, alt texts. Plus the **fundamentals**: robots.txt validation, XML sitemap check, **broken links** (4xx/5xx), **redirect chains** (including HTTP->HTTPS), **mixed content**, **hreflang** and outdated **image format** (WebP/AVIF advice).

**Structure**, URL depth, breadcrumb presence, internal link structure, sitemap references.

### Max Audit, the deepest analysis

The **Max Audit** adds three things on top of a Deep Audit:

- **JavaScript rendering**, the page is fully loaded first (like a real browser), so content that comes in via JavaScript (Wix, Shopify, React) is analysed too.
- **Real Core Web Vitals**, LCP, INP and CLS from Google PageSpeed Insights instead of an estimate.
- **Keyword positions & search volume**, which keywords your site ranks for, at which position, with monthly search volume (via DataForSEO). Selectable **per country and language**, so the data fits your market (NL, BE, DE, UK, US and more).

### Specify a target keyword

You can optionally pass a target keyword with each audit. The SEO Engine then also analyses keyword density, placement in title/H1 and content relevance for that keyword.

### Issues and recommendations

Per audit you get:

- **Issues** sorted by severity (Critical / High / Medium / Low) with type and description
- **Recommendations** sorted by priority (High / Medium) with concrete action steps and expected result

### Export & compare

Export any report as **PDF** (client-ready) or **CSV** (scores, issues, keywords and competitors, handy for agencies). On a second audit the dashboard automatically shows the **change versus the previous audit** (score, sub-scores and number of issues) plus your **progress over time**.

## Site Crawl, a real multi-page crawl

Besides the quick audit, the SEO Engine has a **Site Crawl**: a real crawl of your whole site (not a single page). You get a tabbed panel with **Overview**, **Issues** (with "how to fix" per type), **Crawled pages** and **Statistics**, plus a **Site Health meter**.

| Tier | Pages | Content | Credits |
|---|---|---|---|
| Light | up to 25 | 100+ checks, duplicate titles/descriptions, broken links, redirects | 6,000 cr |
| Standard | up to 50 | + more resources and checks | 12,000 cr |
| Pro | up to 100 | + JavaScript rendering + Lighthouse | 22,000 cr |

The page limit determines the cost, so you always keep the crawl (and the credits) in hand.

## Keyword Research

Give a keyword and you get a worksheet with **long-tail ideas**: monthly **search volume**, **difficulty**, **search intent** (informational/commercial/transactional) and an **AI-Overview opportunity** flag (candidates that score well in AI answers). **500 credits** per query.

## Links & Authority

In the **Links** tab you analyse your backlink profile:

- **Authority Score**, your domain authority (0-100)
- **Domain overview**, backlinks, referring domains, IPs, broken links, keywords
- **New & lost** referring domains over time
- **Toxic / risk domains**, referring domains with a high spam score
- **(Pro) Link gap**, domains that link your competitor but not you, plus a domain-vs-domain comparison

| Tier | Content | Credits |
|---|---|---|
| Links Check | Authority + top referring domains | 8,000 cr |
| Links Audit | + new/lost + toxic links | 15,000 cr |
| Links Audit Pro | + competitor link gap + compare | 25,000 cr |

## Credit cost

| Action | Credits |
|---|---|
| Quick Check | 1,500 |
| Standard Audit | 4,000 |
| Deep Audit (up to 10 pages) | 10,000 |
| Max Audit (+ render + CWV + keywords) | 22,000 |
| Site Crawl (Light / Standard / Pro) | 6,000 / 12,000 / 22,000 |
| Keyword Research (per query) | 500 |
| Links & Authority (Check / Audit / Pro) | 8,000 / 15,000 / 25,000 |

## Example: what you get after an audit

You run a Standard Audit on your services page. The result is not a list of
technical notices but an ordered judgement:

> **SEO score 61 / 100** , was 54 at your previous audit *(+7)*
>
> | Category | Score |
> |---|---|
> | On-page | 72 |
> | Content | 58 |
> | Technical | 49 |
> | Structure | 66 |
>
> **Critical (2)**
> - Meta description missing on this page
> - 3 internal links return a 404
>
> **High (1)**
> - LCP is 4.1 seconds on mobile, aim for under 2.5
>
> **Recommended action:** write a meta description of 150-160 characters around
> your target keyword. Expected effect: a higher click-through rate from Google.

The ordering is the payoff: you know which three things to do on Monday, instead
of picking from a hundred signals yourself.

## Limits

- **The engine changes nothing on your site.** It measures and advises; you make the changes yourself or through the [Authority Engine](authority-engine.md).
- **Your page has to be publicly reachable.** A staging environment behind a login or password cannot be analysed.
- **A score is not a ranking guarantee.** A higher score improves your foundation, but positions also depend on competition, authority and search intent.
- **The page limit per tier is hard.** A crawl covers 25, 50 or 100 pages; larger sites you analyse in parts.
- **No JavaScript rendering below Max.** On a site that loads its content through JavaScript, a lower tier sees less than is actually there.
- **Keyword data is per country and language.** Pick the right market, otherwise the volumes are not your audience.

## Troubleshooting

**The audit stays on "running".** Large crawls take minutes. If it hangs longer than fifteen minutes, start again; failed audits are refunded.

**The score is far lower than expected.** Check whether you used a lower tier on a JavaScript site: without rendering the audit reads a near-empty page. Run a Max Audit or Site Crawl Pro.

**Core Web Vitals are empty.** Google only supplies those when there is enough field data. For a new or rarely visited page that is normal.

**Broken links are reported that work fine.** Some servers block automated requests. Check the link by hand; if it works, you can ignore the notice.

**Your keywords are missing.** Check the country and language setting. Keywords without measurable volume are left out.

## Frequently asked questions

**What is the difference between a page analysis and a site crawl?**
Depth versus breadth. The audit goes deep on one page, with AI recommendations,
keyword positions and Core Web Vitals. The crawl goes wide across your whole
site, with a hundred mechanical checks, duplicate titles and broken links, but
without per-page AI advice.

**How often should I audit?**
After every major change, and monthly beyond that. You can also have it run
automatically, so you see the trend without thinking about it.

**Can I hand the report to a client?**
Yes. Export as PDF; on Pro and up you put your own logo, colour and agency name
on it.

**Does this work for webshops?**
Yes. On large shops watch the page limit and crawl in parts, for example per
category.

**What is the difference with the GEO Engine?**
The SEO Engine measures your position in Google. The
[GEO Engine](geo-engine.md) measures whether AI assistants mention you.
Increasingly you need both.

## Tips

- **Start with a Standard Audit** for a full picture of your most important landing page
- **Provide a target keyword** for pages you want to rank for a specific term
- **Use a Deep Audit** on a new site or after a redesign
- **Compare audits** in the history to see whether your changes had an effect

---

Next: [GEO Engine](geo-engine.md) · [Authority Engine](authority-engine.md) · [All Growth Tools](../engines/README.md)
On the site: [SEO Engine](https://dgenix.com/engines/seo) · [pricing](https://dgenix.com/pricing)

*dGENIX Docs, SEO Engine, updated August 2026*
