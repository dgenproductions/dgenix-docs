# Connecting Microsoft 365

The Microsoft 365 connection lets GENI read and send your Outlook mail, check your calendar and read along in a Teams channel.

> **Coming soon.** The connection is built and waiting on Microsoft's Azure
> OAuth verification. Once that clears, Microsoft 365 appears in your Connectors
> list; there is nothing to prepare.

If you use Google rather than Microsoft, that works today: see
[Gmail](gmail.md) and [Google Calendar](google-calendar.md).

## What you can do with it

| What you ask | What GENI does |
|---|---|
| "What is in my Outlook inbox?" | Reads your recent emails |
| "Email Sofie that the quote is ready" | Sends an email through Outlook |
| "What is in my calendar this week?" | Fetches your upcoming appointments |
| "What was discussed in the project channel?" | Reads recent messages from a Teams channel |

## Connecting (once available)

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to Microsoft 365
3. Log in with your work or school account
4. Review the permissions requested and click **Accept**
5. The [Microsoft 365 skill](https://dgenix.com/skills/microsoft-365) is active right away

The skill sits in **Growth** and up.

## What access you grant

| Scope | What dGENIX uses it for |
|---|---|
| `Mail.ReadWrite` | Reading your Outlook mail and drafting replies |
| `Mail.Send` | Sending an email after your approval |
| `Calendars.ReadWrite` | Checking your calendar and scheduling appointments |
| `Files.ReadWrite.All` | Fetching and saving OneDrive files |
| `User.Read` | Reading your name and email address |

> **Note:** in many organisations an administrator has to approve these
> permissions. If you see "Approval required" when signing in, ask your IT
> administrator to grant consent.

## Checking that it works

After connecting, ask:

```
What is in my Outlook inbox?
```

You get a summary of your recent mail back.

## Limits

- Sending an email or scheduling an appointment asks for confirmation
- GENI does not delete mail, calendar entries or files
- In Teams it only **reads**; posting messages is not supported
- Only channels where you name the team and channel, not an automatic overview of everything
- Shared mailboxes and colleagues' calendars are out of scope

## Troubleshooting

**Microsoft 365 is not in Connectors.** The connection has not been released yet. See the notice at the top of this page.

**"Administrator approval required" when signing in.** Your organisation does not allow apps by default. Your IT administrator has to approve the app in Azure.

**Teams returns nothing.** You have to point at a team and channel; without that GENI does not know where to look.

**You have a personal Microsoft account.** The connection targets work and school accounts; a personal account may work only partially.

## Disconnecting

Go to **Dashboard -> Connectors**, click Microsoft 365 and choose **Disconnect**.
You can also revoke access via *Microsoft account -> Privacy -> Apps and
services*.

## Frequently asked questions

**When will the connection arrive?**
That depends on Microsoft's verification process. Once it clears, the connection
appears in your dashboard by itself.

**Can I connect both Google and Microsoft?**
Yes. They are independent; GENI picks the account based on your request.

**Can my employer see what GENI does?**
Your administrator can see the app was approved and can revoke access. What you
ask inside dGENIX stays within your own account.

---

Back to [Connectors overview](README.md)
See also: [Gmail](gmail.md) · [Google Calendar](google-calendar.md) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Connecting Microsoft 365, updated August 2026*
