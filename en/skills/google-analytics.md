# Google Analytics

Website traffic insights straight in the chat via Google Analytics 4. Visitor numbers, top pages, traffic sources and audience data, without opening the Analytics dashboard.

**Requirements:** Growth+ plan, connect a Google account via Connectors

---

## Available actions

| Action | Credit cost | Description |
|---|---|---|
| `analytics_overview` | 35 cr | General visitor overview (sessions, users, bounce rate) |
| `top_pages` | 30 cr | Top pages ranked by views and session duration |
| `traffic_sources_report` | 35 cr | Analysis of traffic sources (organic, social, direct, paid) |
| `audience_insights` | 40 cr | Demographic and behaviour data (age, device, country, retention) |

---

## Connecting

1. Go to **Connectors**
2. Click **Connect** on Google Analytics
3. Log in with the Google account that has access to your GA4 property
4. Grant permission for `analytics.readonly`

On first use the assistant asks for the GA4 property ID (found in GA4 > Admin > Property settings).

---

## Example conversations

**Weekly report:**
> "Give me the visitor overview for the past 7 days"

**Top pages:**
> "Which pages generated the most traffic last month?"

**Traffic sources:**
> "How does organic search traffic compare to social media traffic?"

**Audience:**
> "What percentage of my visitors use a mobile device?"

---

## Tips

- Save your GA4 property ID in your knowledge document so you do not have to give it each time
- Use `audience_insights` for campaign optimisation and targeting
- Combine with Search Console for a complete SEO picture
- Period notation: "past 7 days", "last month", "this quarter"

---

## Limitations

- Read only (no changing data or creating events)
- Goals and conversions are not available via the Data API v1
- Real-time data is not supported in this skill
