# Authority Engine

The [Authority Engine](https://dgenix.com/engines/authority) is the step from *measuring* to *doing*: GENI writes articles built for authority and stages them in your CMS, but never without your approval.

The other engines tell you what is wrong. This one writes the content that fixes
it. Available from **Pro**.

## What the Authority Engine does

| Part | What it produces |
|---|---|
| **Topical map** | A content plan: one pillar article plus cluster articles around your main topic |
| **Draft article** | An original, E-E-A-T-focused article, ready for review |
| **Content score** | A grade for your draft, measured against what currently ranks on Google |
| **Publishing** | To your CMS as a draft, or live, always as a deliberate choice |

The order is deliberate: first a plan, then the articles, then measure back.
Writing individual articles without a plan produces pieces that compete for the
same keywords.

## Example: what you ask, what you get

You ask for a topical map about "heat pumps". You do not get articles but a
**plan**:

> **Pillar:** Heat pumps, the complete guide for homeowners
>
> **Clusters:**
> - What does a heat pump cost?
> - Heat pump or gas boiler, which is cheaper?
> - What subsidy can you get on a heat pump?
> - Is my home suitable for a heat pump?
>
> Per title: **Write article** →

Each title comes with its monthly search volume and is a button. Click it and
GENI writes that one article, with an internal link to the pillar. That is how
you build a coherent cluster instead of scattered pieces.

For a draft article you get the full text in the queue, alongside **To CMS as
draft**, **Publish live**, **Edit** and **Reject**.

## How it works

1. **Connect your CMS.** WordPress (Application Password) or Webflow (API key and collection ID), plus six other systems. Without a connection everything works except publishing.
2. **Build a topical map**, or give a topic directly for a single article.
3. **Generate a draft.** It stays inside dGENIX; nothing goes to your site.
4. **Review it in the queue.** Read, edit, or have it scored against the competition.
5. **You decide**: to your CMS as a draft, publish live, or reject.
6. **Rollback.** A published or forwarded piece reverts to draft with one click.

## Content score, measuring back against the SERP

Judging a draft on instinct is hard. The **content score** therefore fetches the
pages currently ranking for your keyword and compares your piece against them:

- a **coverage score** from 0 to 100
- **missing topics** the competition does cover
- concrete **additions** to make the piece more complete
- a **length benchmark** against the current top pages

That closes the loop: measure, write, measure back.

## Via GENI and on autopilot

The Authority Engine is also just a GENI skill. You can ask it in chat ("write a
draft about X", "build a topical map about Y") and, more usefully, **schedule
it**. Set up a recurring task, for example a new draft every Monday, and the
pieces land in your queue by themselves. Publishing always stays your action.

See [Scheduled tasks](../handleiding/geplande-taken.md).

## Safe by design

Google acts against mass AI content published without oversight. That brake is
built in here:

- **Draft-first.** GENI never touches your site unless you publish.
- **Mandatory approval.** Every publication is a separate, deliberate action.
- **Volume limit.** Up to 30 drafts per month, counted from your billing date.
- **Activity log.** Every writing and publishing action is recorded.
- **Revocable connection.** Credentials are stored encrypted and can be revoked at any time.

## What it costs

| Action | Credits |
|---|---|
| Topical map | 2,000 |
| Draft article | 3,000 |
| Content score | 2,500 |
| Sending to CMS or publishing | free |

If an action fails, you get the credits back. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Up to 30 drafts per month.** Deliberate, to keep quality above volume.
- **GENI never publishes on its own**, not even inside a recurring task.
- **Text only.** You add images to an article yourself in your CMS.
- **No rewriting of existing pages**; the engine creates new pieces.
- **You stay responsible for the content.** GENI writes well-grounded text, but facts about your company, prices and promises are yours to check.
- **Framer is not supported yet**, while their write API is not mature.

## Troubleshooting

**Publishing returns an error.** Usually the CMS connection has expired or a permission is missing. Check the connection in the Authority dashboard.

**You have hit the monthly limit.** The counter runs from your billing date, not from the first of the month. The dashboard shows how many you have left.

**The article lands in the wrong place in your CMS.** On WordPress it goes to the default category, on Webflow to the collection you specified. Set that in the connection.

**The draft is factually off.** Edit it in the queue before you approve. That is exactly what the step is there for.

**You see no search volumes in the topical map.** The figures come from an external source; if that is unavailable you still get a plan, just without volumes.

## Frequently asked questions

**Will Google notice this is AI content?**
Google does not penalise AI use, but unchecked mass production without editing.
That is why this engine enforces approval per piece and caps the month. Read
what you publish and add where your own experience contributes; that is exactly
the difference E-E-A-T judges.

**Which CMS platforms are supported?**
WordPress, WooCommerce, Webflow, Shopify, HubSpot, Wix, Storyblok and Magento.

**Can I use it without a CMS?**
Yes. Without a connection GENI simply writes drafts you copy; only the publish
button is unusable.

**What is the difference with the SEO Blog Writer?**
That writes one article on request. The Authority Engine thinks in clusters,
measures back against the SERP and publishes with approval.

**Does this work for my agency's clients?**
Yes. Set up a project per client and the context stays separate. See
[Projects](../functies/projecten.md).

---

Next: [SEO Engine](seo-engine.md) · [GEO Engine](geo-engine.md) · [All Growth Tools](../engines/README.md)
On the site: [Authority Engine](https://dgenix.com/engines/authority) · [pricing](https://dgenix.com/pricing)

*dGENIX Docs, Authority Engine, updated August 2026*
