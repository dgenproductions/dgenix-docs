# Connect Google Sheets

By connecting Google Sheets, your AI assistant can read your spreadsheets, update them and add new rows.

> Google Sheets is included from the Starter plan.

---

## What can your assistant do with Google Sheets?

- Fetch and summarise spreadsheet data
- Add new rows (e.g. leads, notes, tasks)
- Update existing cells
- Analyse data and report insights

---

## Connecting Google Sheets

1. Go to **Dashboard -> Connectors**
2. Click **"Connect"** next to Google Sheets
3. A window opens, log in with your Google account
4. Grant dGENIX the requested permissions
5. The window closes automatically, the connection is active

> You also need the **Google Sheets skill**. Activate it via **Dashboard -> Skills**.

---

## Which permissions does dGENIX request?

| Permission | For |
|---|---|
| Read spreadsheets | Fetch and summarise data |
| Edit spreadsheets | Add rows and update cells |

dGENIX **cannot** delete spreadsheets or manage your Google Drive.

---

## How do you refer to a spreadsheet?

Pass the spreadsheet ID or the full URL in your command:

```
Read the first 10 rows of spreadsheet 1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgVE2upms
```
```
Add a new row to my leads sheet: https://docs.google.com/spreadsheets/d/1BxiM...
```

The spreadsheet ID is in the URL between `/d/` and `/edit`.

---

## Disconnecting Google Sheets

1. Go to **Dashboard -> Connectors**
2. Click **"Remove"** next to Google Sheets
3. The connection is removed immediately

You can also revoke access via [myaccount.google.com/permissions](https://myaccount.google.com/permissions).

---

## Problems?

**Connection failed:** check that you are logged in to the right Google account and try again.

**Assistant can't find the spreadsheet:** make sure you connected the Google account that has access to that spreadsheet.

**Questions?** Use the contact form at [dgenix.com/contact](https://dgenix.com/contact).
