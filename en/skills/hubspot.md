# HubSpot CRM

With the HubSpot skill GENI keeps your CRM current from the chat: looking up and creating contacts, updating deals, adding notes and summarising your pipeline.

Available from **Growth**. You need a connected HubSpot account; see
[Connecting HubSpot](../connectors/hubspot.md).

## What can GENI do with HubSpot?

- **Look up a contact** by email, name or company
- **Create a contact**
- **Create a deal or move its stage**
- **Add a note** to a contact or deal
- **Fetch your pipeline**, grouped by stage

Most of the return is in the small actions: adding a note straight after a call,
instead of never getting round to it.

## Example: what you ask, what you get

```
How is my pipeline looking?
```

> **14 open deals, €96,400 combined**
>
> | Stage | Deals | Value |
> |---|---|---|
> | First contact | 5 | €18,200 |
> | Quote sent | 6 | €52,900 |
> | Negotiation | 3 | €25,300 |
>
> **Worth noting:** four deals in "Quote sent" have been there over three weeks,
> together worth €31,000. The oldest is De Vries, since 12 July.
>
> Shall I stage a follow-up note for those four?

## Requirements

- **Plan:** Growth and up
- **Connection:** a HubSpot Private App token via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **HubSpot CRM**
2. Create a private app in HubSpot with the scopes you need
3. Paste the token at **Dashboard -> Connectors**

The scopes you enable decide what GENI may do. Leave the write scopes off and it
can only read. See [Connecting HubSpot](../connectors/hubspot.md).

## What it costs

| Action | Credits |
|---|---|
| Add a note | ~40 |
| Create or find a contact | ~50 |
| Update a deal | ~50 |
| Pipeline overview | ~70 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Creating and updating ask for confirmation.**
- **GENI never deletes** contacts, deals or notes.
- **Contacts, deals and notes only.** Tickets, products and quotes are out of scope.
- **Custom properties are not filled automatically.**
- **Without the right scope it cannot**, even if you ask. That is by design.
- **Sending email does not run through HubSpot** but through your email connection.

## Troubleshooting

**Permissions error on an action.** The matching scope is off in your private app. Tick it in HubSpot and save; the token stays the same.

**A deal lands in the wrong pipeline.** Without being told, HubSpot uses your default pipeline. Name the pipeline in your request.

**A contact is not found.** Search by email; that is the most reliable field. Names appear duplicated or spelled differently more often.

**The token is rejected.** You probably pasted the Client secret instead of the private app's access token.

## Frequently asked questions

**Can GENI search my whole CRM?**
It searches specifically by email, name or company. Nothing is copied or
indexed; every search goes live to HubSpot.

**Can I combine this with other skills?**
Yes, and that is the value: writing a new lead from
[Lead Research](lead-research.md) straight in as a contact, or a pipeline
overview inside your [weekly report](weekly-report.md).

**Does this work with a free HubSpot account?**
Private apps are available on the free CRM tiers. Some fields and pipelines do
require a paid HubSpot plan.

**What is the difference with CRM Sync?**
[CRM Sync](crm-sync.md) keeps data aligned between systems. This skill works
directly inside HubSpot.

---

Back to [Skills marketplace](README.md)
See also: [Connecting HubSpot](../connectors/hubspot.md) · [Lead Research](lead-research.md) · [CRM Sync](crm-sync.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, HubSpot CRM, updated August 2026*
