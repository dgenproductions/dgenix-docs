# Airtable

With the Airtable skill GENI reads your bases, fetches records and creates or updates them, so you can keep things current from the chat.

Available from **Growth**. You need a connected Airtable account.

## What can GENI do with Airtable?

- **List your bases** available to the connection
- **Read records** from a table
- **Create a record**
- **Update an existing record**

Where a spreadsheet stops, Airtable begins: linked tables, status fields and
different views on the same data.

## Example: what you ask, what you get

```
Which leads are on "waiting for quote"?
```

> From base **Sales 2026**, table *Leads*, 4 records:
>
> | Company | Since | Contact |
> |---|---|---|
> | Bakkerij De Krent | 12 July | Sanne |
> | Studio Noord | 24 July | Mark |
> | Van Dijk BV | 30 July | Lisa |
> | De Vries | 2 August | Peter |
>
> The first two have been there over two weeks. Shall I set their status to
> "follow up"?

When creating or updating you see what will be written first:

```
Set Van Dijk to "quote sent"
```

> **Van Dijk BV** , status from *waiting for quote* to *quote sent*.
> Shall I apply that?

## Requirements

- **Plan:** Growth and up
- **Connection:** an Airtable account via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Airtable**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Pick the bases you grant access to

## What it costs

Airtable actions are light operations: reading and writing cost a small number of
credits per action. The exact amount shows on the button before you start. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Creating and updating ask for confirmation.**
- **GENI never deletes records, tables or bases.**
- **Only the bases you granted access to.** What you did not share stays invisible.
- **No creating tables or fields.** You build the structure in Airtable.
- **Formulas, links and views are read as values**, not modified.
- **On large tables part is read.** Name a view or filter if you want a specific set.

## Troubleshooting

**A base is not found.** It was not shared when connecting. Disconnect and grant access to it as well.

**The wrong record is updated.** Name the record as specifically as possible, for example by a unique field rather than the company name.

**A field is not filled.** Check the field type; a select field only accepts existing options, and a linked field points to another record.

**You see fewer records than expected.** On large tables part is fetched. Filter by status or period.

## Frequently asked questions

**What is the difference with Google Sheets?**
[Sheets](google-sheets.md) is a spreadsheet: rows and columns. Airtable is a
light database with field types and relations. For simple lists Sheets is
enough; for a pipeline with statuses Airtable works better.

**Can I schedule this?**
Yes, for example a weekly overview of records stuck on the same status too long.
See [Scheduled tasks](../handleiding/geplande-taken.md).

**Can it read attachments in a record?**
No, it reads the fields. For documents use the
[knowledge base](../functies/kennisbank.md).

**Does this work with a free Airtable account?**
Yes, within the limits Airtable itself sets.

---

Back to [Skills marketplace](README.md)
See also: [Google Sheets](google-sheets.md) · [Typeform](typeform.md) · [HubSpot CRM](hubspot.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Airtable, updated August 2026*
