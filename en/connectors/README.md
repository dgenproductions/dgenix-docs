# Connectors

A connector is the link between dGENIX and an account that belongs to you: your mailbox, your calendar, your CRM. Without a connector GENI can reach nothing.

You connect a tool once via **Dashboard -> Connectors**. After that GENI uses it
by itself as soon as a request calls for it; you never have to say *which*
connection to reach for.

## Connector or skill?

This is the question people hit most while setting up, so, briefly:

| | Connector | Skill |
|---|---|---|
| **What it governs** | Whether GENI is **allowed** somewhere | What it can **do** there |
| **Where you set it** | Dashboard -> Connectors | Dashboard -> Skills |
| **Example** | Access to your Google account | Reading mail, scheduling |

You need both. Switch on the Gmail skill without connecting Google and GENI
knows how to read mail but there is no mailbox. The other way round it has
access but no actions. See
[How it all fits together](../concepten/hoe-alles-samenwerkt.md).

## How to connect a tool

1. Go to **Dashboard -> Connectors**
2. Pick the connector you want to link
3. Complete the authorisation: sign in to the service, or paste a key
4. The connector shows as **Connected** and all related skills work right away

It rarely takes more than a minute, except for the Meta connections (WhatsApp
and Instagram), which require a Developer account.

## Available connectors

### Google Workspace

| Connector | Skill | Plan |
|---|---|---|
| [Gmail](gmail.md) | Gmail | Starter+ |
| [Google Calendar](google-calendar.md) | Google Calendar | Starter+ |
| [Google Drive](google-drive.md) | Google Drive | Starter+ |
| [Google Sheets](google-sheets.md) | Google Sheets | Starter+ |
| [YouTube](youtube.md) | YouTube Manager | Growth+ |

One Google connection does not cover everything: you grant permission per
service, so you decide whether GENI sees only your calendar or your mail too.

### Communication and collaboration

| Connector | Skill | Plan |
|---|---|---|
| [Slack](slack.md) | Slack | Growth+ |
| [Notion](notion.md) | Notion | Growth+ |
| [LinkedIn](linkedin.md) | LinkedIn | Growth+ |
| [Microsoft 365](microsoft-365.md) | Microsoft 365 | Growth+ (coming soon) |
| [Canva](canva.md) | Canva | Starter+ (coming soon) |

### Social media and messaging

| Connector | Skill | Plan |
|---|---|---|
| [WhatsApp Business](whatsapp-business.md) | WhatsApp Business | Growth+ |
| [Instagram Business](instagram.md) | Instagram DM | Growth+ |

### Finance and CRM

| Connector | Skill | Plan |
|---|---|---|
| [Stripe](stripe.md) | Stripe Insights | Growth+ |
| [HubSpot](hubspot.md) | HubSpot CRM | Growth+ |

### Extendable

| Connector | What for | Plan |
|---|---|---|
| [MCP connectors](mcp-connectors.md) | Growing ecosystem via an open standard | Growth+ |

## Two ways of connecting

**Signing in to the service.** You click Connect, log in and grant permission.
This applies to Gmail, Google Calendar, Google Drive, Google Sheets, YouTube,
Slack, Notion, LinkedIn, Microsoft 365 and Canva. The connection refreshes
itself; you never have to check on it.

**Pasting a key.** You create a key or token in the other service and paste it
into dGENIX. This applies to WhatsApp Business, Instagram Business, Stripe and
HubSpot. The upside: while creating it you decide exactly which permissions that
key carries.

## What a connector does not do

- **Copy nothing.** Your data stays with the service itself; nothing is pulled in or indexed.
- **Delete nothing.** GENI does not erase mail, files, channels or contacts.
- **Change nothing unasked.** Anything that changes or sends asks for confirmation first.
- **Reach no further than you granted.** Every connector page shows exactly which permissions you give.

## Disconnecting

Go to **Dashboard -> Connectors**, click the connector and choose
**Disconnect**. From that moment GENI cannot reach it and every skill depending
on it stops. Most services also let you revoke access on their side; that is
described per connector.

## Frequently asked questions

**Do I have to connect everything?**
No. Connect what you use. Most people start with mail and calendar and expand
later.

**Can someone else reach my connections?**
No. A connector belongs to your account. Even within the same company nobody
shares your connections.

**A skill does not work while it is switched on?**
Almost always because the matching connector is missing or expired. Check
**Dashboard -> Connectors** to see whether the service still shows as Connected.

**My tool is not listed.**
Check whether it is available through [MCP connectors](mcp-connectors.md), or
submit a request through the skill marketplace.

---

Next: [How it all fits together](../concepten/hoe-alles-samenwerkt.md) · [Skills explained](../handleiding/skills-uitgelegd.md)
On the site: [all integrations](https://dgenix.com/integrations) · [all skills](https://dgenix.com/skills)

*dGENIX Docs, Connectors, updated August 2026*
