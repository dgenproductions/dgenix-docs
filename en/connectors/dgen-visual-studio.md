# Connecting dGEN Visual Studio

With this connector GENI works inside your own dGEN Visual Studio: it creates images and video there, and it runs the flows you built on the canvas yourself.

The difference with the image skills dGENIX ships on its own is the word *your*. The work happens in your own studio account, with your own models and your own LoRAs, and the result lands in your own library.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "Create a campaign image in my studio" | Generates the image there and shows it to you |
| "Which flows do I have ready?" | Lists your saved flows and their steps |
| "Run the weekly banner flow" | Starts that flow from beginning to end |
| "Which models can I use?" | Returns the catalogue with what each model accepts |
| "What is in my library?" | Returns your latest files with a link |
| "How many credits do I have left there?" | Reads your studio balance |

The flow is where this gets interesting. Build it once on the canvas, put it in a [scheduled task](../handleiding/geplande-taken.md), and your recurring visual work happens without you opening the studio again.

## Connecting

1. Go to **Dashboard → Connectors**
2. Click **Connect** next to dGEN Visual Studio
3. Sign in to the studio; you get a consent screen there listing the permissions requested
4. Click **Allow**. The [dGEN Visual Studio skill](../skills/dgen-visual-studio.md) is active straight away

The connector is available from **Growth** upwards. If you do not have a studio account yet, create one first at dgenvisual.com.

## What access you give

| Permission | What dGENIX uses it for |
|---|---|
| View flows | Fetching your list of flows and the model catalogue |
| Run a flow | Executing a saved flow from beginning to end |
| View files | Searching your library and getting a temporary download link |
| View LoRAs | Seeing which style models of your own you have |
| Create images | Generating an image (costs studio credits) |
| Create video | Generating a video (costs studio credits) |
| View balance | Reading how many credits you have left there |

Changing and deleting are not included: GENI cannot edit your flows and cannot remove anything from your library.

## What it costs

This is where most of the confusion starts, so plainly: **the generation is billed in the studio, against your balance there.** dGENIX only charges the action, 5 credits to look something up and 25 to have something made. What the image itself costs is listed in the studio next to the model.

Anything that creates something therefore asks for your confirmation first, with the amount shown. See [The credit system](../hoe-het-werkt/credits.md).

## Checking that it works

After connecting, ask it to **read** something rather than make something:

```
How many credits do I have left in my Visual Studio?
```

If you get a balance back, the connection is live. Then feel free to ask which flows are ready.

## Limits

- **Images take seconds, video takes minutes.** For video you first get a confirmation that it is running; the result lands in your library
- **GENI does not build flows.** It runs what you made; the canvas stays your work
- **A model that cannot read your input is refused by the studio** , ask which models exist rather than naming one
- **No studio credits, no images.** dGENIX cannot top up your balance there
- **The studio decides the catalogue.** If the model line-up changes there, it changes here

## Troubleshooting

**GENI says you are not connected.** Check under **Dashboard → Connectors** whether the connector says Connected. If the consent was revoked in the studio, the connector stops without warning.

**"The studio could not run this."** That is a message from the studio itself, usually about a model that does not accept the input you sent. Ask which models are available and what input they expect.

**You get an id back instead of an image.** The generation is still running. Ask about it later with that id, or look in your studio library.

**The image is right but the style is not.** Name your LoRA or use a flow; a one-off request falls back to the studio default model.

## Disconnecting

Go to **Dashboard → Connectors**, find dGEN Visual Studio and click **Disconnect**. Access ends immediately.

Two things worth knowing:

- **The skill stays activated.** To remove it entirely, switch it off in the marketplace too
- **What was made stays.** Disconnecting removes nothing from your studio library

You can also revoke the consent in the studio itself, under **Connected apps**. That is also where the daily spending ceiling per connection lives.

## Frequently asked questions

**Why not just use the dGENIX image skills?**
Those are faster for one-off images. This connector exists for work that belongs in your studio: your own models, your own LoRAs, one library, and flows you built yourself.

**Am I paying twice now?**
No. The studio charges the generation, dGENIX charges the action. The studio amount is the same as when you press Run there yourself.

**Can GENI do this on a schedule?**
Yes, and that is the main reason this connector exists. See [Scheduled tasks](../handleiding/geplande-taken.md).

**Can GENI change my flows?**
No. It may read and run them, nothing more.

---

→ Back to [Connectors](README.md)
→ Next: [dGEN Visual Studio skill](../skills/dgen-visual-studio.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
→ On the site: [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, dGEN Visual Studio, updated August 2026*
