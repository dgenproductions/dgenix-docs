# CRM Sync

With the CRM Sync skill GENI fetches contacts from your CRM, updates deal statuses and produces an overview report, so your systems do not drift apart.

Available from **Pro**.

## What can GENI do with it?

- **Fetch contacts** from your connected CRM
- **Update a deal status**
- **Generate a sync report** with what does not line up

The third is where the skill gets its name. If you work with several systems
they drift without anyone noticing: a deal won in one system and still open in
the other.

## Example: what you ask, what you get

```
Make a sync report
```

> **12 contacts checked, 3 differences found**
>
> | Contact | Difference |
> |---|---|
> | De Vries | Deal is "won" in the CRM, "quote" in your workspace |
> | Studio Noord | Phone number differs between the two systems |
> | Van Dijk BV | Exists only in your workspace, not in the CRM |
>
> The first matters most: that deal was won three weeks ago and still counts
> towards your open pipeline.
>
> Shall I update the status in your workspace?

## Requirements

- **Plan:** Pro and up
- **Connection:** a CRM, for example [HubSpot](hubspot.md)

## Activating

1. Go to **Dashboard -> Skills** and activate **CRM Sync**
2. Connect your CRM via **Dashboard -> Connectors**
3. Ask for contacts, a status change or a report

## What it costs

| Action | Credits |
|---|---|
| Fetch contacts | 15 |
| Generate a sync report | 15 |

This is one of the cheapest skills, precisely because you are meant to run it
regularly. See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **It does not sync automatically.** You see the differences and decide what happens.
- **Updating asks for confirmation.**
- **GENI never deletes contacts or deals.**
- **No two-way sync in one click.** You resolve differences case by case, not with a "make everything match" button.
- **Only the fields the CRM exposes.** Custom properties often fall outside.

## Troubleshooting

**No differences are found.** That may be correct. Do check that your CRM is connected and that contacts exist in both systems.

**A difference is not real.** Two systems can differ deliberately, for example an internal field the client should not see. Say which fields you want compared.

**Updating fails.** The write scopes in your CRM connection are off. See [Connecting HubSpot](../connectors/hubspot.md).

**Contacts are missing.** It fetches what the connection exposes; contacts in another pipeline or with another owner sometimes fall outside.

## Frequently asked questions

**Which CRM is supported?**
HubSpot through its own connection. Other systems may become available through
[MCP connectors](../connectors/mcp-connectors.md).

**What is the difference with the HubSpot skill?**
[That one](hubspot.md) works directly inside HubSpot: creating contacts,
updating deals. CRM Sync looks at differences between systems.

**Can I run this weekly?**
Yes, and that is the best use: 15 credits per report, so weekly costs you almost
nothing. See [Scheduled tasks](../handleiding/geplande-taken.md).

**Does it change things without me knowing?**
No. Every change asks for confirmation.

---

Back to [Skills marketplace](README.md)
See also: [HubSpot CRM](hubspot.md) · [Weekly report](weekly-report.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, CRM Sync, updated August 2026*
