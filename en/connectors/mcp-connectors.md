# MCP connectors

MCP connectors link GENI to tools that have no dedicated dGENIX connection, through the Model Context Protocol: an open standard by which external services expose their capabilities.

The practical consequence: a dGENIX connection no longer has to be built for
every tool separately. If a service offers an MCP server, it can be plugged in
as a connector. For you such a connector works exactly like any other: activate
it, connect your account, done.

## What you can do with it

What an MCP connector can do is decided by the service itself. In practice it
comes down to the same kinds of actions as our own connections: look something
up, create something, update something. Every connector shows in the dashboard
which actions it brings.

The point is not that MCP does something other connections cannot, but that
adding a tool goes **much faster**.

## Activating

1. Go to **Dashboard -> Skills** and find the connector
2. Click **Activate**; it appears as a regular skill toggle
3. Follow the step-by-step instruction that appears right after activation
4. Connect your own account via **Dashboard -> Connectors**, if the connector asks for it
5. Ask GENI to do something with it

Every MCP connector has its own instruction in the dashboard, just like Gmail or
WhatsApp. You do not need to do anything technical or run a server.

## Ways of connecting

| Method | How it goes | Comparable to |
|---|---|---|
| Signing in | You log in to the service and grant permission | Slack, Notion |
| Pasting a key | You paste a key from your own account | Stripe, HubSpot |
| No connection | Activating is enough, no account needed | , |

Which one applies is shown in the connector's own instruction.

## It runs on your account

An MCP connector works on **your own account** at that service by default. That
has three consequences worth knowing:

- You keep control over the account and the data in it
- If the service charges, those costs run through your account and not through dGENIX
- You can disconnect any time via **Connectors -> Disconnect**, after which GENI immediately loses access

## What it costs

MCP connectors use the same credit system as all other skills: a fixed price per
action, visible before it runs. More expensive actions ask for confirmation
first, so there are no surprises. See
[The credit system](../hoe-het-werkt/credits.md).

MCP connectors sit in **Growth** and up.

## Limits

- A connector can only do what the service itself exposes through MCP
- If the service is down, the connector is down; dGENIX cannot work around that
- Actions that change or delete something always ask for confirmation
- We decide which connectors are available; you cannot add your own
- The range grows gradually, so your tool may not be there yet

## Troubleshooting

**The connector is not in the marketplace.** Then it is not available yet. You can request it through the skill marketplace.

**Activating works, but nothing happens.** The connector probably still needs a connection. Check **Dashboard -> Connectors** to see whether it shows as Connected.

**You do not know which actions it supports.** Open the connector in the dashboard; the instruction states exactly what it can do.

## Frequently asked questions

**What is MCP, really?**
An open standard by which a service exposes its capabilities to AI assistants in
a uniform way. Because it is a standard, not every connection has to be
hand-built from scratch.

**Does it feel different from a regular connection?**
No. In the dashboard, in chat and in credit accounting it works identically.

**Can I plug in my own MCP server?**
Not at the moment. The range is curated by us, so every connector comes with a
tested instruction and a fixed credit price.

---

Back to [Connectors](README.md)
Next: [Skills explained](../handleiding/skills-uitgelegd.md) · [The credit system](../hoe-het-werkt/credits.md)
On the site: [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, MCP connectors, updated August 2026*
