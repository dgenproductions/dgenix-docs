# CMS Publisher

With the CMS Publisher GENI puts an article straight into your WordPress or Webflow, as a draft by default so you keep the final word.

Available from **Growth**. You need a connected WordPress or Webflow site.

## What can GENI do with it?

- **Publish to WordPress** , title, content, categories and tags, as draft or straight live
- **Publish to Webflow** , an item in your CMS collection, as draft or published

Both default to **draft**. Going live is possible, but you have to ask for it
explicitly.

## Example: what you ask, what you get

```
Put the article on maintenance contracts on my WordPress as a draft
```

> **Draft created , "Why a maintenance contract earns more than it costs"**
>
> - 1,180 words, 6 subheadings
> - Category: Maintenance · Tags: contract, planning, cost
> - Status: **draft**, so not visible to visitors yet
>
> Edit and publish here:
> `yoursite.com/wp-admin/post.php?post=412&action=edit`
>
> I did not set a featured image, that one is yours to pick.

## Requirements

- **Plan:** Growth and up
- **Connection:** WordPress (with an application password) or Webflow. See [Connectors](../connectors/README.md)

## Activating

1. Go to **Dashboard -> Skills** and activate **CMS Publisher**
2. Connect your WordPress or Webflow site through **Dashboard -> Connectors**
3. Ask GENI to place an article as a draft

## What it costs

| Action | Credits |
|---|---|
| Publish to WordPress | 25 |
| Publish to Webflow | 25 |

Writing the article is charged separately; see
[SEO Blog Writer](seo-blog.md) or
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **WordPress and Webflow only.** The [Authority Engine](authority-engine.md) publishes to more systems; this skill does not.
- **Draft is the default, and that is deliberate.** Going straight live is possible but takes an explicit instruction.
- **No images.** Featured images and in-text visuals are yours to set; generating them is possible with [AI Image Generation](ai-beeldgeneratie.md).
- **No updating existing articles.** It creates a new item.
- **Formatting is limited to headings, paragraphs and lists.** Blocks, shortcodes and page builder elements do not carry over.
- **Webflow does not publish your site.** A published item only appears after a site publish in Webflow.

## Troubleshooting

**"No access".** On WordPress the application password has expired or been revoked. Create a new one and reconnect.

**The article has no formatting.** The content arrived as plain text. Ask GENI for markdown formatting with headings.

**Wrong collection in Webflow.** Name the collection explicitly, or set the default on the connection.

**The item is in Webflow but not visible.** Publish your site in Webflow; a CMS item alone is not enough.

## Frequently asked questions

**Does it go live straight away?**
No, not by default. You get a draft and publish yourself, unless you explicitly
ask for live.

**What is the difference with the Authority Engine?**
[That one](authority-engine.md) writes a whole content strategy and publishes to
eight systems. The CMS Publisher is the single step "put this article in".

**Can I schedule this?**
Yes, through [Scheduled tasks](../handleiding/geplande-taken.md), for example a
draft ready every week.

**Does it work with WooCommerce?**
For blog articles yes, that is plain WordPress. Creating products is not
possible.

---

Back to [Skills marketplace](README.md)
See also: [SEO Blog Writer](seo-blog.md) · [Authority Engine](authority-engine.md) · [Connectors](../connectors/README.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, CMS Publisher, updated August 2026*
