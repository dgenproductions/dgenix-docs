# dGEN Visual Studio

dGEN Visual Studio is an AI studio for images and video, with your own style and with
recurring work built as a flow on a canvas. With this skill GENI does that work for you: creating an image or a video, or running a flow you built yourself.

Available from **Growth** upwards. You need the
[dGEN Visual Studio connector](../connectors/dgen-visual-studio.md) and a studio account of
your own.

## What GENI can do with it

The difference with [AI Image Generation](ai-beeldgeneratie.md) and [FLUX](flux-image.md) is
the word *your*. Those two quickly make a one-off image on our models. This skill works in
your studio, with your models, your LoRAs and your library , and it can do something the
other two cannot: run a flow you built.

| Tool | What it does |
|---|---|
| `visualstudio_beeld_maken` | Creates an image in your studio |
| `visualstudio_video_maken` | Creates a video (takes minutes) |
| `visualstudio_flows` | Lists your saved flows with their id |
| `visualstudio_flow_draaien` | Runs a flow from beginning to end |
| `visualstudio_modellen` | The catalogue, with what each model accepts |
| `visualstudio_bibliotheek` | Your latest files with a link |
| `visualstudio_bestand_ophalen` | Fetches a file so a next step can use it |
| `visualstudio_saldo` | Your credit balance in the studio |

## Example: what you ask, what you get back

```
Run my weekly banner flow and get the result ready
```

> You have three flows ready. I will run **Weekly banner** (4 steps).
>
> This costs credits in your studio, not on your dGENIX balance. Shall I go ahead?
>
> *[after your confirmation]*
>
> The flow is done; everything is in your studio library.

Put that same instruction in a [scheduled task](../handleiding/geplande-taken.md) and your
monthly round of visuals happens on its own, every Monday at eight.

## Combining with other skills

Everything GENI makes in your studio also lands in your dGENIX files. That turns the result
from an endpoint into a link in a chain:

- **Knowledge base → SEO Blog Writer → this skill → CMS Publisher** , an article with a
  matching image, staged as a draft
- **Scheduled task → this skill → Social Media Manager** , fresh visuals every Monday with
  the posts scheduled alongside
- **Google Business Profile → this skill → LinkedIn** , a good review becomes a quote card
- **Google Sheets → this skill → Google Drive** , every row without an image gets one

⚠️ To use an **existing** file, have GENI fetch it first. The link from
`visualstudio_bibliotheek` is temporary; a fetched file keeps working.

## Requirements

- **Plan:** Growth and above
- **Connector:** dGEN Visual Studio, with a studio account of your own
- **Balance in the studio:** the generation is billed there

## Activating

1. Go to **Dashboard → Skills** and activate **dGEN Visual Studio**
2. Connect your account under **Dashboard → Connectors**
3. Ask GENI what is ready in your studio

## What it costs

Two balances, and that is on purpose:

| What | Where it comes off |
|---|---|
| Looking something up (flows, models, library, balance) | **5 credits** at dGENIX |
| Having something made (image, video, flow) | **25 credits** at dGENIX |
| The generation itself | **Your studio credits**, the same amount as pressing Run there |

Anything that creates something asks for your confirmation first, with the amount shown. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI does not build flows.** It reads and runs them; the canvas stays your work
- **Video takes minutes.** You get a confirmation that it is running, the result lands in
  your library
- **Do not invent model names.** Ask for the catalogue first; the studio refuses an unknown id
- **No studio credits, no images.** Topping up only happens in the studio itself
- **Nothing is deleted.** The skill has no permission to remove anything from your library

## Troubleshooting

**"Your dGEN Visual Studio is not connected yet."** Check under **Dashboard → Connectors**
whether the connector says Connected. If you revoke the consent in the studio, the connector
stops without warning.

**You get an id back instead of an image.** The generation is still running. Ask about it
later with that id, or look in your library.

**"The studio could not run this."** That is a message from the studio itself, usually about a
model that does not accept the input you sent. Ask for the catalogue.

**The style is off.** Name your LoRA or use a flow; a one-off request falls back to the studio
default model.

## Frequently asked questions

**What is the difference with AI Image Generation?**
That one quickly makes a single image on our models and charges dGENIX credits. This skill
works in your studio account, with your models, and bills there.

**Can GENI do this on a schedule?**
Yes. That is the main reason this skill exists; see
[Scheduled tasks](../handleiding/geplande-taken.md).

**What happens to what it makes?**
It lands in two places: in your studio library, exactly like work you make on the canvas yourself, and in your dGENIX files. The second is what makes it usable in a next step.

---

→ Back to [Skills marketplace](README.md)
→ See also: [Connecting dGEN Visual Studio](../connectors/dgen-visual-studio.md) · [AI Image Generation](ai-beeldgeneratie.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
→ On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, dGEN Visual Studio, updated August 2026*
