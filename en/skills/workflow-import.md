# Workflow Builder

With the Workflow Builder you import an existing n8n workflow as JSON into dGENIX and have GENI run it, without needing an n8n server of your own.

Available from **Pro**. Pro includes **3 import slots**; more slots can be added.

## What can GENI do with it?

- **Import a workflow** from n8n JSON you paste or supply
- **Run a workflow**, with the parameters you give it
- **List your imported workflows**
- **Delete a workflow** (freeing up the slot)

So you build the workflow elsewhere (in n8n, or from a template) and run it here.

## Example: what you ask, what you get

```
Import this workflow
[n8n JSON pasted]
```

> **Imported: Lead enrichment**
>
> 6 steps recognised:
> 1. Webhook , receives company name
> 2. HTTP , fetch registry data
> 3. Filter , active registrations only
> 4. HTTP , fetch website
> 5. AI , summarise the company description
> 6. Google Sheets , append a row
>
> You are now using **2 of your 3 slots**.
> Running it costs around 25 credits, depending on the number of steps.

And when running:

```
Run the lead enrichment for "Example Ltd"
```

> Done in 8 seconds. Registry number found, website fetched, summary written and
> added as row 47 in your sheet.
>
> One step raised a warning: the registry returned two registrations, I used the
> active one.

## Requirements

- **Plan:** Pro and up
- **Connection:** depends on your workflow. If it uses Gmail or Sheets, that connector has to be connected

## Activating

1. Go to **Dashboard -> Skills** and activate **Workflow Builder**
2. Paste your n8n JSON into the chat or import it through the dashboard
3. Run it with "run workflow X"

## What it costs

| Action | Credits |
|---|---|
| Import a workflow | 0 |
| Run a workflow | from 25 |
| List workflows | 3 |
| Delete a workflow | 0 |

The 25 credits are the baseline; a workflow with many steps or AI steps costs
more, because each step does its own work. See
[The credit system](../hoe-het-werkt/credits.md).

**Extra slots:** +1 for € 6.99, +5 for € 29.99, +10 for € 59.99 per month,
cancellable monthly.

## Limits

- **Not every n8n node is supported.** dGENIX runs the steps itself; nodes that require their own n8n environment do not work.
- **No visual editor.** You build and change in n8n and import the JSON again.
- **Slots are per imported workflow**, not per run. Delete an old one to make room.
- **Changing the workflow in n8n changes nothing here.** Import it again.
- **Credentials come from your dGENIX connectors**, not from the JSON. A workflow with a Gmail step only works once Gmail is connected.

## Troubleshooting

**"Import failed".** The JSON is incomplete or exported from only part of the canvas. Export the whole workflow.

**A step is skipped.** That node is not supported. Ask which steps were recognised and you see exactly where it breaks.

**"No slots left".** Delete a workflow you no longer use, or buy extra slots through **Account -> Billing**.

**The workflow runs but does nothing.** Usually a connection a step needs is missing. Check your Connectors.

## Frequently asked questions

**Do I need my own n8n server?**
No. You only use n8n to build; running happens at dGENIX.

**What is the difference with Automations?**
[Automations](../functies/workflow-automations.md) are tasks GENI runs at a set
time. The Workflow Builder runs an imported chain of steps. You can combine
them: an automation that starts your workflow.

**What is the difference with Custom Workflows?**
[Custom Workflows](custom-workflows.md) calls a webhook on your own server. The
Workflow Builder runs the steps here.

**Can GENI build a workflow itself?**
It can think along about the setup, but you build the JSON in n8n.

---

Back to [Skills marketplace](README.md)
See also: [Custom Workflows](custom-workflows.md) · [Automations](../functies/workflow-automations.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
On the site: [all skills](https://dgenix.com/skills) · [pricing](https://dgenix.com/pricing)

*dGENIX Docs, Workflow Builder, updated August 2026*
