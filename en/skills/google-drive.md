# Google Drive

With the Google Drive skill GENI finds files in your Drive, reads their content and tidies your folders, so you do not have to dig.

Available from **Starter**. You need a connected Google account; see
[Connecting Google Drive](../connectors/google-drive.md).

## What can GENI do with Google Drive?

- **Search files** by name, type or content
- **Read a document's text**, so it can summarise or quote from it
- **Create a folder** in your Drive structure
- **Move or rename a file**
- **Set sharing permissions** per person: view, comment or edit

## Example: what you ask, what you get

```
Find the De Vries quote and summarise it
```

> Found: **Quote De Vries , heat pump.docx**, last modified 2 August.
>
> - Heat pump including installation: **€8,450** excluding VAT
> - Lead time 4 to 6 weeks after approval
> - Quote valid until **1 September**
> - Maintenance contract optional, €240 per year
>
> The quote expires in four weeks. Shall I set a reminder?

## Requirements

- **Plan:** Starter and up
- **Connection:** a Google account via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Google Drive**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Complete the Google consent screen
4. Drive is usable right away

## What it costs

| Action | Credits |
|---|---|
| Search a file | ~20 |
| Read and summarise a document | ~40 |
| Create a folder | ~15 |
| Move or rename a file | ~15 |
| Set sharing permissions | ~20 |

The skill is included in your plan; you pay per action. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI never deletes a file or folder.**
- **It reads text, not layout.** Images, charts and complex formatting inside a document are not interpreted.
- **A scanned PDF without a text layer yields nothing.**
- **Moving, renaming and sharing ask for confirmation**, because they change something for other people.
- **It does not edit a document's content.** For writing in Google Docs use [Google Docs](google-docs.md).
- **Only the connected account.** Other people's shared Drives are visible only if you have access.

## Troubleshooting

**A file is not found.** Search on part of the filename. If it sits in a shared Drive you cannot access, GENI cannot see it either.

**It cannot read the content.** With a scanned PDF or a format without a text layer there is nothing to extract.

**Setting permissions fails.** You do not have rights to share that file, or the organisation restricts external sharing.

**It finds an old version.** Drive keeps versions; GENI reads the current one. Check you are looking for the right copy.

## Frequently asked questions

**Can GENI upload files?**
Files you send in the chat end up in your Workspace. See
[Files](../functies/bestanden.md).

**What is the difference with the knowledge base?**
Drive is your storage, which GENI searches when you ask. The
[knowledge base](../functies/kennisbank.md) is a fixed set of documents it
consults on its own.

**Can it clean up folders?**
It can move and rename, not delete. Clearing out stays your call.

**Does dGENIX see all my files?**
Only what is needed for your question, at the moment you ask it.

---

Back to [Skills marketplace](README.md)
See also: [Connecting Google Drive](../connectors/google-drive.md) · [Google Docs](google-docs.md) · [Knowledge base](../functies/kennisbank.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Google Drive, updated August 2026*
