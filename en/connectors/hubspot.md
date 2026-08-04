# Connecting HubSpot

The HubSpot connection lets GENI look up and create contacts, update deals, add notes and summarise your sales pipeline.

This connection works with a **Private App token** you create in HubSpot
yourself, not with the usual sign-in button. That way you decide exactly which
permissions dGENIX gets. The connection activates the
[HubSpot skill](../skills/hubspot.md), available from **Growth**.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "Is jan@company.com already in our CRM?" | Searches by email, name or company |
| "Add this lead as a contact" | Creates a new contact |
| "Move the De Vries deal to 'quote sent'" | Creates or updates a deal |
| "Note on this contact that they call back in March" | Adds a note |
| "How is my pipeline looking?" | Returns all deals grouped by stage |

## Connecting

1. Log in to HubSpot and go to *Settings -> Integrations -> Private Apps*
2. Click **Create a private app** and give it a name, for example "dGENIX"
3. Open the **Scopes** tab and enable:
   - `crm.objects.contacts.read` + `.write`
   - `crm.objects.deals.read` + `.write`
   - `crm.objects.notes.write`
4. Click **Create app** and copy the token you receive
5. Go to **Dashboard -> Connectors**, click **Connect** on HubSpot and paste the token

Store the token carefully: HubSpot shows it in full only once.

## What access you grant

| Scope | What dGENIX uses it for |
|---|---|
| `crm.objects.contacts.read` | Looking up contacts |
| `crm.objects.contacts.write` | Creating new contacts |
| `crm.objects.deals.read` | Reading the pipeline and individual deals |
| `crm.objects.deals.write` | Creating a deal or changing its stage |
| `crm.objects.notes.write` | Adding notes to a contact or deal |

If you leave a scope off, GENI simply cannot do it. To make it read-only, for
instance, leave the `.write` scopes disabled.

## Checking that it works

Ask this right after connecting:

```
How is my HubSpot pipeline looking?
```

You get your deals grouped by stage. If you get a permissions error, a scope is
missing from your private app.

## Limits

- GENI never **deletes** contacts, deals or notes
- Creating a contact or updating a deal asks for confirmation
- Contacts, deals and notes only; not tickets, products or quotes
- Custom properties are not filled in automatically
- Sending email does not run through HubSpot but through your email connection

## Troubleshooting

**Permissions error on an action.** The matching scope is disabled. Open your private app in HubSpot, tick it and save; the token stays the same.

**The token is rejected.** You probably pasted the Client secret or an old API key. It has to be the private app's **access token**.

**A deal lands in the wrong pipeline.** Without being told, HubSpot uses your default pipeline. Name the pipeline in your request.

## Disconnecting

Delete the private app in HubSpot, or go to **Dashboard -> Connectors**, click
HubSpot and choose **Disconnect**. Deleting the app in HubSpot invalidates the
token immediately.

## Frequently asked questions

**Why no ordinary sign-in button like Slack?**
With a private app you decide, scope by scope, what dGENIX may do. That is more
precise than a standard authorisation where you approve everything at once.

**Does this work with a free HubSpot account?**
Private apps are available on the free CRM tiers. Some fields and pipelines do
require a paid HubSpot plan.

**Can GENI search my entire CRM?**
It searches specifically, by email, name or company. Nothing is copied or
indexed; every search goes live to HubSpot.

---

Back to [Connectors overview](README.md)
See also: [HubSpot CRM skill](../skills/hubspot.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting HubSpot, updated August 2026*
