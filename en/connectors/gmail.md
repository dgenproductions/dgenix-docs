# Connect Gmail

The Gmail connector gives GENI access to your inbox, so it can read, summarise and draft email, preparing messages you only need to confirm.

## What you can do with it

| What GENI does | Example |
|---|---|
| Summarise your inbox | "What's important in my unread mail?" |
| Open a specific email | "Read Sofie's email about the quote" |
| Draft and send an email | "Email Jan that tomorrow's meeting is going ahead" |

The connection activates the **[Gmail skill](../skills/gmail.md)**, available from Starter.

## Connecting

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to Gmail
3. You are taken to Google's consent screen
4. Sign in and grant the requested permissions
5. Once approved, the connector shows as **Connected**

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| Read email | Summarising your inbox, finding and opening messages |
| Send email | Sending a drafted message after your confirmation |
| Manage labels | Recognising and archiving newsletters |

dGENIX **never deletes** email, and sends nothing without your explicit
confirmation. You always see the draft first.

## Checking that it works

Right after connecting, ask GENI:

```
Summarise my 5 most recent unread emails
```

You get the sender, subject and gist per message. If it stays empty while you do
have unread mail, the wrong Google account is connected.

## Limits

- GENI never deletes email
- Sending only happens after your confirmation, including inside a recurring task
- It only reads the mailbox of the connected account, not colleagues' shared mailboxes
- Attachments are recognised but not opened automatically; ask for them explicitly

## Troubleshooting

**Connection fails.** Check that your browser is signed in to the right Google account. Sign out of Google and try again.

**GENI does not see your mail.** You connected a different Google account than the one receiving your mail. Disconnect and connect the right account.

**Sending does not work.** The connection was made without send permissions. Disconnect and reconnect, granting all requested permissions.

## Disconnecting

Go to **Dashboard -> Connectors**, click Gmail and choose **Disconnect**.
You can also revoke access at Google itself via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Frequently asked questions

**Does this also connect Calendar, Drive and Sheets at once?**
No. Each Google service is its own connector with its own permissions, even within the same account. That way you never grant more access than you need.

**Can GENI email on my behalf without me seeing it?**
No. Every send asks for confirmation and you see the text beforehand.

**Does this work with my company's Google Workspace account?**
Yes, provided your administrator allows external apps to be connected.

---

Back to [Connectors overview](README.md)
See also: [Gmail skill](../skills/gmail.md)

*dGENIX Docs, Connect Gmail, updated August 2026*
