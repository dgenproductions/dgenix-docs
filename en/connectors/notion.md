# Connecting Notion

The Notion connection gives GENI access to the pages and databases you select, so it can read, write and search there.

Notion works differently from most connections: you do not grant access to your
whole workspace, you **choose which pages you share**. The connection activates
the [Notion skill](../skills/notion.md), available from **Growth**.

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "Put today's meeting notes in Notion" | Creates a new page |
| "Add the conclusions to the project page" | Updates an existing page |
| "Where is our onboarding checklist?" | Searches the shared pages and databases |
| "What is in Monday's meeting notes?" | Reads the content of a page |
| "Create a row in my client database" | Creates a page in that database |

## Connecting

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to Notion
3. Log in with your Notion account
4. **Select the pages and databases** you want to share
5. Click **Allow access**; Notion then shows as **Connected**

Step 4 is the important one. If you select nothing, the connection is active but
GENI cannot reach anything.

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| Reading selected pages | Fetching and searching content |
| Adding content | Creating new pages or database rows |
| Updating content | Adding text to an existing page |

Access covers **only what you ticked in step 4**, including the sub-pages under
it. Everything else in your workspace stays out of reach.

## Checking that it works

Ask this right after connecting:

```
Which Notion pages can you see?
```

If you get an empty list back, you selected no pages while connecting. Redo the
connection and tick something this time.

## Limits

- GENI sees **only** the pages you explicitly shared
- You cannot add pages afterwards from inside dGENIX; you disconnect and re-authorise
- GENI never deletes pages or database rows
- Creating or updating a page asks for confirmation
- Very long pages are read partially; ask about a specific section for a better result

## Troubleshooting

**GENI cannot find a page that exists.** That page is not shared. Disconnect and select it as well.

**A new page appears somewhere unexpected.** Without a named location Notion puts it in the first shared page. Name the target page or database in your request.

**You want to add a database.** Databases have to be ticked separately; sharing the parent page is not enough.

## Disconnecting

Go to **Dashboard -> Connectors**, click Notion and choose **Disconnect**. In
Notion you can also revoke access via *Settings -> Connections*.

## Frequently asked questions

**Can GENI reach my whole Notion workspace?**
No, and that is exactly what sets this apart from most connections. Notion asks
your permission per page; dGENIX gets no more than that.

**Can I add more pages later?**
Yes, but it goes through Notion's authorisation: disconnect in dGENIX and
connect again with a wider selection.

**Does this work with a free Notion account?**
Yes. The connection uses Notion's standard integration capabilities.

---

Back to [Connectors overview](README.md)
See also: [Notion skill](../skills/notion.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting Notion, updated August 2026*
