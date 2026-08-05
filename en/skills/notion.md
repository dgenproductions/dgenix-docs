# Notion

With the Notion skill GENI searches your workspace, reads pages and writes new ones, so capturing notes does not interrupt what you were doing.

Available from **Growth**. You need a connected Notion workspace; see
[Connecting Notion](../connectors/notion.md).

## What can GENI do with Notion?

- **Search** the shared pages and databases
- **Read a page**
- **Create a page**, standalone or in a database
- **Update an existing page**

## Example: what you ask, what you get

```
Put the outcome of this conversation in Notion, under the De Krent project
```

> **Created: Meeting De Krent , 5 August**
> `notion.so/Meeting-De-Krent-5-August-1a2b3c`
>
> Containing:
> - Decision: website plus POS integration, quote approved
> - Materials delivered by 15 August at the latest
> - Contact is Sanne, decision-maker is the owner
> - Open: who supplies the copy
>
> I placed it as a subpage under *Projects 2026*.

And when searching:

```
Where is our onboarding checklist?
```

> Found in **Internal processes › Client onboarding**, last modified 12 June.
> The checklist has 14 items; the last three cover invoicing.

## Requirements

- **Plan:** Growth and up
- **Connection:** a Notion workspace via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Notion**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. **Select the pages and databases** you want to share

That third step decides everything. Select nothing and the connection is active
but GENI can reach nothing.

## What it costs

| Action | Credits |
|---|---|
| Read or search a page | ~30 |
| Update a page | ~50 |
| Create a page | ~60 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI only sees what you explicitly shared**, including the subpages under it.
- **You cannot add pages from inside dGENIX.** You disconnect and re-authorise with a wider selection.
- **Creating and updating ask for confirmation.**
- **GENI never deletes pages or database rows.**
- **Very long pages are read partially.** Ask about a specific section.
- **Complex blocks stay out of view**: databases-in-databases, synced blocks and embeds are not interpreted.

## Troubleshooting

**A page is not found.** It is not shared. Disconnect and select it as well.

**A new page appears somewhere unexpected.** Without a named location Notion puts it in the first shared page. Name the target page or database.

**A database is not seen.** Databases have to be ticked separately; sharing the parent page is not enough.

**The formatting disappoints.** Headings, paragraphs and lists carry over; complex block structures do not.

## Frequently asked questions

**Can GENI reach my whole workspace?**
No, and that is what sets it apart from most connections. Notion asks permission
per page.

**What is the difference with the Workspace?**
The [Workspace](../functies/werkruimte.md) lives inside dGENIX and connects to
your tasks and timeline. Notion is your own system, where your team also works.

**Can it write a conversation out as a note?**
Yes. That is the most common use: have the meeting, have the outcome recorded.

**Can I schedule this?**
Yes, for example updating a status page weekly. See
[Scheduled tasks](../handleiding/geplande-taken.md).

---

Back to [Skills marketplace](README.md)
See also: [Connecting Notion](../connectors/notion.md) · [Workspace](../functies/werkruimte.md) · [Airtable](airtable.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Notion, updated August 2026*
