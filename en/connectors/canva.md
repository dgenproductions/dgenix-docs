# Connecting Canva

The Canva connection lets GENI search designs, create them from your brand templates and export them as PNG, PDF or MP4.

> **Coming soon.** The connection is built, but waiting on approval from Canva's
> Developer API programme. Once it lands, Canva appears in your Connectors list;
> there is nothing to prepare.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "Which designs do I already have for the summer promo?" | Searches your existing designs |
| "Which brand templates do we have?" | Lists the available brand templates |
| "Create a blank Instagram format" | Creates a new design in the requested size |
| "Fill the promo template with this text and price" | Auto-fills a brand template |
| "Export that design as a PDF" | Delivers a downloadable file |

Filling **brand templates** is where this gets interesting: one template plus
varying text produces a series of visuals that all look the same.

## Connecting (once available)

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to Canva
3. Log in with your Canva account and grant access
4. The [Canva skill](../skills/canva.md) is active right away

The skill sits in **Starter** and up.

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| Reading designs | Searching your existing designs |
| Reading brand templates | Fetching available templates |
| Creating designs | Making a new or filled design |
| Exporting | Retrieving a design as a file |

## Checking that it works

After connecting, ask:

```
Which Canva designs can you see?
```

You get a list of your design titles back.

## Limits

- GENI does not edit an existing design; it creates a **new** one or fills a template
- Free-form design is not possible, only what a brand template supports
- Exporting a large or complex design takes longer; GENI waits and reports the result
- Designs are never deleted
- Brand templates may require a paid Canva plan

## Troubleshooting

**Canva is not in Connectors.** The connection has not been released yet. See the notice at the top of this page.

**There are no brand templates.** Those sit in Canva's paid plans. Without templates you can still create and export blank designs.

**An export seems to hang.** Canva processes exports in the background; a heavy design takes longer. GENI reports back once the file is ready.

## Disconnecting

Go to **Dashboard -> Connectors**, click Canva and choose **Disconnect**. In
Canva you can also revoke access through your account settings.

## Frequently asked questions

**When will the connection be available?**
That depends on Canva's approval. We have no influence on it; once it is
through, the connection appears in your dashboard by itself.

**Is this the same as AI image generation?**
No. Image generation creates a new picture from a description; Canva works with
your own templates and brand style. See
[AI image generation](../skills/ai-beeldgeneratie.md).

**Can GENI design a campaign itself?**
It can fill a series of designs from a template. The design of that template you
make in Canva.

---

Back to [Connectors overview](README.md)
See also: [Canva skill](../skills/canva.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting Canva, updated August 2026*
