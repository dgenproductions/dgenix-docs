# Custom Workflows

With Custom Workflows GENI triggers a webhook on your own server or in your own n8n, so you can drive existing automations from a conversation.

Available from **Pro**. You configure which webhooks are reachable.

## What can GENI do with it?

- **Trigger a workflow** by name, with optional parameters as JSON
- **List your configured workflows**

This is the bridge to what you already run. dGENIX does not execute your
workflow, it starts it and hands back the response.

## Example: what you ask, what you get

```
Which workflows do I have?
```

> You have three configured:
>
> | Name | What it does |
> |---|---|
> | quote-pdf | Generates a quote PDF from your template |
> | stock-sync | Syncs stock with your web shop |
> | client-export | Exports a client file as a zip |

And when triggering:

```
Start quote-pdf for De Krent, amount 4,800
```

> Started. The workflow returned:
>
> > `{ "status": "ok", "url": "https://yourserver.com/quotes/2026-084.pdf" }`
>
> The quote is ready: [2026-084.pdf](https://yourserver.com/quotes/2026-084.pdf)

## Requirements

- **Plan:** Pro and up
- **Connection:** a reachable webhook URL, configured in your account

## Activating

1. Go to **Dashboard -> Skills** and activate **Custom Workflows**
2. Configure your webhooks (name + URL) through **Dashboard -> Connectors**
3. Ask GENI which workflows are available

## What it costs

| Action | Credits |
|---|---|
| Trigger a workflow | 10 |
| List workflows | 3 |

Whatever your own server does afterwards costs nothing at dGENIX , that bill
runs at your end. See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **The webhook has to be publicly reachable.** Internal and private addresses are blocked, which is a deliberate safety measure.
- **GENI waits for a response.** If your workflow takes minutes, have it acknowledge immediately and return the result later.
- **dGENIX does not check what your workflow does.** A wrong parameter can genuinely change something on your side.
- **Only workflows you configured yourself.** GENI cannot call an arbitrary URL.
- **The response comes back as your server gives it.** Send readable JSON and GENI can do something sensible with it.

## Troubleshooting

**"Workflow not found".** The name differs from what is configured. Ask for the list first.

**The webhook is refused.** The address is not publicly reachable, or it is an internal network address. Use a public endpoint with authentication.

**Timeout.** Your workflow takes too long. Have it respond immediately and do the real work in the background.

**The parameters arrive wrong.** Say which fields your workflow expects and GENI sends them in that shape.

## Frequently asked questions

**What is the difference with the Workflow Builder?**
The [Workflow Builder](workflow-import.md) imports n8n JSON and runs the steps
at dGENIX. Custom Workflows calls your server and leaves execution there.

**Can I schedule this?**
Yes. Set it as a [scheduled task](../handleiding/geplande-taken.md), for example
a nightly sync.

**How do I secure the webhook?**
Put a token or a secret URL on it. dGENIX sends what you configure; the
authentication is yours to arrange.

**Does this work with tools other than n8n?**
Yes. Any service that accepts an HTTP webhook works, from Make to a script of
your own.

---

Back to [Skills marketplace](README.md)
See also: [Workflow Builder](workflow-import.md) · [Automations](../functies/workflow-automations.md) · [Connectors](../connectors/README.md)
On the site: [all integrations](https://dgenix.com/integrations) · [all skills](https://dgenix.com/skills)

*dGENIX Docs, Custom Workflows, updated August 2026*
