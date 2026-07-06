# Google Search Console

Keyword report, page performance and SEO opportunities based on real Google Search Console data. Discover which queries drive traffic and where your rankings can improve.

**Requirements:** Growth+ plan, connect a Google account via Connectors

---

## Available actions

| Action | Credit cost | Description |
|---|---|---|
| `keywords_report` | 50 cr | Top keywords with clicks, impressions, CTR and average position |
| `page_performance` | 35 cr | Performance per URL: clicks, impressions, CTR, position |
| `seo_opportunities` | 450 cr | Strategic SEO analysis with AI recommendations (Sonnet) |

---

## Connecting

1. Go to **Connectors**
2. Click **Connect** on Search Console
3. Log in with the Google account that owns the Search Console property
4. Grant permission for `webmasters.readonly`

On first use the assistant asks for your website URL so the right property is selected.

---

## Example conversations

**Keyword report:**
> "Which keywords bring the most traffic to my site in the past 28 days?"

**Page analysis:**
> "Analyse the performance of my homepage in Search Console"

**SEO opportunities:**
> "Which SEO improvements can I make based on my Search Console data?"

---

## Tips

- `seo_opportunities` uses Claude Sonnet for the best analysis (450 cr), use it monthly for strategic planning
- Filter by page URL to zoom into specific landing pages
- Combine with Google Analytics for a complete view of traffic and behaviour
- Low CTR at high impressions = a strong opportunity for title/meta optimisation

---

## Limitations

- Read only (no changes in Search Console)
- Data has a 2-3 day delay
- URL inspection and sitemaps are not available via this skill
- Maximum 1,000 rows per query (Google API limit)
