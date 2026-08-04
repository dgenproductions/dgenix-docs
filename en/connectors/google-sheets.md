# Connect Google Sheets

The Google Sheets connector gives GENI access to your spreadsheets, so it can pull data, add rows and update cells without you opening the file.

## What you can do with it

| What GENI does | Example |
|---|---|
| Pull and summarise data | "What's in my leads sheet from this week?" |
| Add new rows | "Add this lead to my leads sheet" |
| Update cells | "Set the status of row 12 to called" |

The connection activates the **[Google Sheets skill](../skills/google-sheets.md)**, available from Starter.

## Connecting

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to Google Sheets
3. Sign in with the Google account that has access to the spreadsheets you want to use
4. Grant dGENIX the requested permissions
5. The window closes by itself and the connection is live

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| Read spreadsheets | Pulling and summarising data |
| Edit spreadsheets | Adding rows and updating cells |

dGENIX **cannot** delete spreadsheets and does not manage your Google Drive.

## How to point at a spreadsheet

Include the spreadsheet ID or the full URL in your request. The ID sits in the
URL between `/d/` and `/edit`:

```
https://docs.google.com/spreadsheets/d/1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs/edit
                                       ^--------- this is the ID -------^
```

Both forms work:

```
Read the first 10 rows of spreadsheet 1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs
```

```
Add a row to my leads sheet with name, email and today's date
```

## Checking that it works

Right after connecting, ask GENI:

```
Read the first 5 rows of <your spreadsheet URL>
```

You get the column names and the first rows back. If you see an access error,
the spreadsheet is not shared with the connected account.

## Limits

- GENI never deletes a spreadsheet or a tab
- It only sees spreadsheets the connected account can access
- Formulas are read as their result, not as the formula
- You point at a spreadsheet per request; GENI does not scan your whole Drive

## Troubleshooting

**Connection fails.** Check that you are signed in to the right Google account. Sign out of Google and try again.

**GENI cannot find the spreadsheet.** The spreadsheet is not shared with the connected account. Share it, or connect the account that does have access.

**Insufficient permissions message.** The connection was made without edit rights. Disconnect and reconnect, granting all requested permissions.

## Disconnecting

Go to **Dashboard -> Connectors**, click Google Sheets and choose **Disconnect**.
You can also revoke access at Google itself via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Frequently asked questions

**Do I also need the Google Sheets skill?**
Yes. The connector handles access, the skill gives GENI the capabilities. Activate it via **Dashboard -> Skills**.

**Does this work with spreadsheets shared by colleagues?**
Yes, as long as the connected Google account has access to that file.

**Can GENI create a new spreadsheet?**
No. It works in existing spreadsheets. You create a new file yourself and then point GENI at it.

---

Back to [Connectors overview](README.md)
See also: [Google Sheets skill](../skills/google-sheets.md)

*dGENIX Docs, Connect Google Sheets, updated August 2026*
