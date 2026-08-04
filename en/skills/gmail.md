# Gmail

With the Gmail skill GENI reads your inbox, summarises it, and writes and sends email on your behalf, in your tone.

Available from **Starter**. You need a connected Google account; see
[Connecting Gmail](../connectors/gmail.md).

## What can GENI do with Gmail?

- **Read your inbox** and fetch the recent messages
- **Open a specific email in full** to assess its content
- **Send an email** to one or more recipients

In practice that lets you have your inbox summarised, replies drafted,
newsletters recognised and searches run for what a sender wrote earlier.

## Example: what you ask, what you get

```
Summarise my unread mail
```

> **12 unread, 3 need action**
>
> - **Sofie van Dijk** , quote approved, wants to sign this week. *Action: send contract.*
> - **Accountant** , VAT return due before the 25th. *Action: supply figures.*
> - **Jan Bakker** , asks whether Thursday can move.
>
> The other 9 are newsletters and notifications.

Ask it to send something and you see the text first:

```
Reply to Sofie that the contract arrives tomorrow
```

> **To:** sofie@vandijk.nl
> **Subject:** Re: Quote approved
>
> Hi Sofie, glad the quote is approved. I will send the contract tomorrow so you
> can sign it this week.
>
> Shall I send this?

## Requirements

- **Plan:** Starter and up
- **Connection:** a Google account via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Gmail**
2. Go to **Dashboard -> Connectors** and click **Connect** next to Gmail
3. Complete the Google consent screen
4. Gmail is usable right away

## What it costs

| Action | Credits |
|---|---|
| Summarise inbox | ~25 |
| Draft and send an email | ~35 |
| Search messages | ~15 |

The skill itself is included in your plan; you only pay per action performed.
See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Sending always asks for confirmation.** You see the full text before it goes out.
- **GENI does not delete mail.** Not even on request; archiving and clearing out is yours to do.
- **It cannot send attachments.** It does read attachments you send in the chat.
- **It does not read along continuously.** Your inbox is only fetched when you ask.
- **Managing filters, labels and rules is not supported.**
- **Only the connected account.** Several mailboxes at once is not possible.

## Troubleshooting

**GENI says it cannot read your inbox.** The connection is missing or expired. Check under **Connectors** whether Gmail still shows as Connected.

**An email is not found.** Search by sender or subject rather than a stray sentence from the body.

**The reply does not sound like you.** Set your writing style in [Settings](../functies/instellingen.md) or record fixed preferences in your [memory](../functies/geheugen.md).

**Sending fails.** Check the recipient's address for typos; Google rejects an invalid address.

## Frequently asked questions

**Can GENI summarise my inbox automatically?**
Yes, schedule it as a daily task. See
[Scheduled tasks](../handleiding/geplande-taken.md).

**Does dGENIX see my password?**
No. You sign in with Google itself; we only get revocable access to what you
approve.

**Does this work with a Google Workspace account?**
Yes. Some organisations do require an administrator's approval.

**Can it send from a different address?**
No, only from the connected account.

---

Back to [Skills marketplace](README.md)
See also: [Connecting Gmail](../connectors/gmail.md) · [Google Calendar](google-calendar.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Gmail, updated August 2026*
