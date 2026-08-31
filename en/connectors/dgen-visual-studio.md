# Connecting dGEN Visual Studio

dGEN Visual Studio is an AI studio for images and video. You work there with the well-known image models, you set down your own style, and you build recurring visual work as a flow on a canvas. With this connector GENI does that work for you: creating images and video, and running the flows you built yourself.

The difference with the image skills dGENIX ships on its own is the word *your*. The work happens on your own studio account, with your own models and your own style models, and the result lands in your own library.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "Create a campaign image in my studio" | Generates the image there and shows it to you |
| "Which flows do I have ready?" | Lists your saved flows and their steps |
| "Run the weekly banner flow" | Starts that flow from beginning to end |
| "Which models can I use?" | Returns the catalogue with what each model accepts |
| "What is in my library?" | Returns your latest files with a link |
| "Take that image and put it in a post" | Fetches the file and uses it in the next step |
| "How many credits do I have left there?" | Reads your studio balance |

Where it gets genuinely interesting is that a result **stays usable**. Everything GENI makes in your studio is also stored in your dGENIX files. That lets a next step carry on with it: an article plus the image staged as a draft in your CMS, a social post with the new visual under it, or an email with the whole set attached.

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

## Combining with other skills

This is what the connector is for: not one picture, but a link in work that was already running.

| Chain | What happens |
|---|---|
| Knowledge base → SEO Blog Writer → dGEN Visual Studio → CMS Publisher | An article from your own knowledge, with an image in your style, staged in your CMS |
| Scheduled task → dGEN Visual Studio → Social Media Manager | Fresh visuals every Monday with the posts scheduled alongside |
| Google Business Profile → dGEN Visual Studio → LinkedIn | A good review becomes a quote card ready to share |
| Google Sheets → dGEN Visual Studio → Google Drive | Every row without an image gets one, saved in the right folder |

You do not set any of that up. Ask it in one sentence, or put that sentence in a [scheduled task](../handleiding/geplande-taken.md).

⚠️ **To use an existing file from your studio, ask GENI to fetch it.** The link the library shows is temporary and stops working after about an hour; a fetched file lands in your dGENIX files and keeps working.

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

- **Images take seconds, video takes minutes.** For video you first get a confirmation that it is running; the result then lands in your studio library and in your dGENIX files
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

**Where does the result end up?**
In two places: in your studio library, exactly like work you make on the canvas yourself, and in your dGENIX files. That second one is what makes it usable in a next step.

---

→ Back to [Connectors](README.md)
→ Next: [dGEN Visual Studio skill](../skills/dgen-visual-studio.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
→ On the site: [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, dGEN Visual Studio, updated August 2026*
