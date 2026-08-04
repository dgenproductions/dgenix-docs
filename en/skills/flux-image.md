# FLUX Image Generation

With the FLUX skill GENI generates images from a description, with four models that let you trade speed against quality.

Available from **Growth**. No connection needed.

## What can GENI do with FLUX?

- **Generate an image** from a text description, with a choice of four models

The model choice decides almost everything: 20 credits for a quick sketch
against 1,000 for a premium edit is a factor of 50.

| Model | For | Credits |
|---|---|---|
| **Schnell** | Fast iterations, concepts, trying things out | 20 |
| **Dev** | High quality, sharp detail, portraits | 175 |
| **Kontext Pro** | Adjusting an existing image, context-aware | 500 |
| **Kontext Max** | Premium context-aware editing | 1,000 |

## Example: what you ask, what you get

```
Make a hero image for my website: an installer at work in a Dutch living room,
warm daylight
```

> Done with **Dev** (175 credits).
>
> The image is in your Workspace under Files. If you want variations, I can make
> three with **Schnell** for 60 credits total; then you pick the direction and
> have that one redone in Dev.

That is usually the cheapest way to work: explore cheaply first, then render
once at quality.

## Requirements

- **Plan:** Growth and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **FLUX Image Generation**
2. Describe what you want to see and optionally name the model

## What it costs

See the table above: from 20 to 1,000 credits per image. Without a model choice
GENI picks a sensible default and states the cost before starting. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Do not expect literal text in the image.** For text in an image
  [Nano Banana Pro](ai-beeldgeneratie.md) is a better fit.
- **No recognisable people or brand logos.** Descriptions asking for those are refused.
- **You will not always get what was in your head.** Expect a few attempts; that is what Schnell is for.
- **Every attempt costs credits**, including ones you do not like.
- **No editing an existing image** except with the Kontext models.
- **You are responsible for how you use the result.**

## Troubleshooting

**The result does not match your description.** Be more concrete about composition, light and style. "An installer" leaves a lot open; "an installer seen from the side, warm daylight from the left" much less.

**It costs more than expected.** You were probably on Dev or Kontext. Name **Schnell** explicitly when you want to explore quickly.

**Hands or faces come out wrong.** A known weakness of image models. Dev does better than Schnell; otherwise frame the shot differently.

**Your request is refused.** The description touches on recognisable people, brands or other material that may not be generated.

## Frequently asked questions

**What is the difference with AI image generation?**
That runs on Nano Banana and is stronger at text-in-image and business assets.
FLUX gives you more control over style plus a cheap fast option. See
[AI image generation](ai-beeldgeneratie.md).

**Where do the images end up?**
In your Workspace, Files tab. See [Files](../functies/bestanden.md).

**May I use the images commercially?**
Yes, with the caveat that you remain responsible for what you publish.

**Can I have an existing image adjusted?**
Yes, with Kontext Pro or Max. For scaling and cropping,
[AI image editing](image-resizer.md) is far cheaper.

---

Back to [Skills marketplace](README.md)
See also: [AI image generation](ai-beeldgeneratie.md) · [AI image editing](image-resizer.md) · [Files](../functies/bestanden.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, FLUX Image Generation, updated August 2026*
