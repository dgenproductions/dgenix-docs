# Google Sheets

With the Google Sheets skill GENI reads your spreadsheets, works with the numbers and writes new rows, so keeping track is not a manual job.

Available from **Starter**. You need a connected Google account; see
[Connecting Google Sheets](../connectors/google-sheets.md).

## What can GENI do with Google Sheets?

- **Read data** from a spreadsheet, a whole sheet or a range
- **Write or update data** in existing cells
- **Append a row** at the bottom of a sheet

That lets you have figures summarised, a list topped up, or a spreadsheet used
as a simple database.

## Example: what you ask, what you get

```
What were my monthly revenue figures in my revenue sheet?
```

> From **Revenue 2026**, sheet *Monthly overview*:
>
> | Month | Revenue | Change |
> |---|---|---|
> | May | €18,400 | , |
> | June | €21,900 | +19% |
> | July | €17,200 | -21% |
>
> July stands out: it is your lowest month since March. The drop is mostly in
> maintenance contracts.

And when writing you see what is about to be added:

```
Add a row: 3 August, De Vries, 8450, quote sent
```

> To be appended to **Quotes 2026**:
> `03-08-2026 | De Vries | €8,450 | quote sent`
>
> Shall I do that?

## Requirements

- **Plan:** Starter and up
- **Connection:** a Google account via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Google Sheets**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Complete the Google consent screen
4. Sheets is usable right away

## What it costs

| Action | Credits |
|---|---|
| Fetch and summarise data | ~25 |
| Append a row | ~20 |
| Analyse data | ~35 |

The skill is included in your plan; you pay per action. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Writing asks for confirmation.** You see what will be written before it happens.
- **GENI does not delete rows, sheets or spreadsheets.**
- **Formulas are read as values, not rewritten.** It does not set up formulas for you.
- **Formatting, colours and conditional formatting stay out of view.**
- **On very large sheets part is read.** Name a range if you want a specific section.
- **Pivot tables and charts are not interpreted.**

## Troubleshooting

**It cannot find the spreadsheet.** Give the exact name, or the document URL. With several files sharing a name, the URL helps.

**The wrong columns are read.** Name the sheet and the range, for example "sheet Monthly overview, columns A to D".

**An appended row lands in the wrong place.** Rows are added at the bottom. If you want it elsewhere, move it yourself.

**The numbers look wrong.** Check whether the cells are formatted as text; then GENI reads them as text too.

## Frequently asked questions

**Can I use a spreadsheet as a database?**
For simple lists that works fine: leads, quotes, stock. For anything more
complex, the Airtable skill is a better fit.

**Can GENI keep this updated automatically?**
Yes, as a scheduled task, for example a weekly line with your figures. See
[Scheduled tasks](../handleiding/geplande-taken.md).

**Does this work with shared spreadsheets?**
Yes, as long as your account has access.

**Can it create a new spreadsheet?**
No, it works in existing sheets. Create the file yourself and let GENI fill it.

---

Back to [Skills marketplace](README.md)
See also: [Connecting Google Sheets](../connectors/google-sheets.md) · [Google Drive](google-drive.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Google Sheets, updated August 2026*
