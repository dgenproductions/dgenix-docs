# Weekly Report Generator

With the Weekly Report Generator GENI builds one report from your scattered data , KPIs from a spreadsheet, what came up in your inbox , and emails it to whoever needs to read it.

Available from **Growth**. It works better the more connections you have.

## What can GENI do with it?

- **Generate a weekly report** over a period of your choice, with KPIs from a Google Sheet, signals from your Gmail, and optionally sent straight to an email address

One tool, but it gathers from several sources. It remembers the sheet URL after
the first time.

## Example: what you ask, what you get

```
Build the weekly report and send it to bart@example.com
```

> **Weekly report , 29 July to 4 August**
>
> **Figures**
>
> | KPI | This week | Last week |
> |---|---|---|
> | New leads | 18 | 12 |
> | Quotes sent | 6 | 7 |
> | Revenue | € 8,420 | € 6,100 |
>
> **What stood out**
> - The spike in leads comes from one source: the comparison page that went live
>   last week
> - Six quotes against 18 leads is on the low side. Twelve leads have had no
>   follow-up.
>
> **From your inbox**
> - Two customers asked about the same feature (export to Excel)
> - A supplier announced a price increase from 1 September
>
> **For next week**
> - Follow up the 12 untouched leads
> - Respond to the price increase before the end of August
>
> Sent to bart@example.com.

## Requirements

- **Plan:** Growth and up
- **Connection:** none required. [Google Sheets](google-sheets.md) for KPIs, [Gmail](gmail.md) for inbox signals and sending

## Activating

1. Go to **Dashboard -> Skills** and activate **Weekly Report Generator**
2. Connect Google Sheets and Gmail through **Dashboard -> Connectors**
3. Ask for a weekly report and supply the sheet URL once

## What it costs

| Action | Credits |
|---|---|
| Generate a weekly report | 300 |

That includes fetching and summarising the sources. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Without sources it comes out thin.** With no sheet and no inbox there is little to report on.
- **The KPIs come from your sheet.** If the sheet is wrong the report is wrong; it does not verify your figures.
- **No charts.** You get text and tables.
- **Only the sources you connect.** Figures from your accounting or CRM only appear if you put them in the sheet.
- **Sending requires Gmail.** Without it you get the report in the chat.

## Troubleshooting

**The KPIs are missing.** The sheet URL was not supplied or the tab has no recognisable headers. Put the KPIs in a table with a header row.

**The report covers the wrong week.** Name the period explicitly; by default it takes the last 7 days.

**It was not sent.** Gmail is not connected, or the address was missing. Name the email address in the request.

**The content is too generic.** Say who reads it. A report for yourself looks different from one for a client or investor.

## Frequently asked questions

**Can I get this weekly on a schedule?**
Yes, that is the point. Set it as a
[scheduled task](../handleiding/geplande-taken.md), for example every Friday at
16:00.

**Can I set several recipients?**
Yes, name the addresses. For a client-facing report,
[White Label](white-label.md) may be a better fit.

**What is the difference with an engine report?**
The [engines](../engines/README.md) report on your visibility and reputation.
This report covers your business figures.

**Can it keep the report?**
Yes, ask it to put it as a note in your
[Workspace](../functies/werkruimte.md).

---

Back to [Skills marketplace](README.md)
See also: [Google Sheets](google-sheets.md) · [White Label](white-label.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Weekly Report Generator, updated August 2026*
