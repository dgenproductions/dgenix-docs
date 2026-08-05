# Connect Google Calendar

The Google Calendar connector lets GENI check your agenda, schedule appointments and confirm availability, without you opening your calendar.

## What you can do with it

| What GENI does | Example |
|---|---|
| Check your agenda | "What's on my calendar today?" |
| Confirm availability | "Am I free Tuesday at 10:00?" |
| Schedule an appointment | "Book a meeting with Jan Friday at 14:00 and send an invite" |

The connection activates the **[Google Calendar skill](../skills/google-calendar.md)**, available from Starter.

## Connecting

1. Go to **Dashboard -> Connectors**
2. Click **Connect** next to Google Calendar
3. Sign in with the Google account whose calendar you want to use
4. Grant dGENIX the requested permissions
5. The window closes by itself and the connection is live

## What access you grant

| Permission | What dGENIX uses it for |
|---|---|
| Read calendar | Checking appointments and availability |
| Edit calendar | Creating, moving and cancelling appointments |

dGENIX changes your calendar **only** on your explicit request.

## Checking that it works

Right after connecting, ask GENI:

```
What's on my calendar this week?
```

You get your appointments per day. If it stays empty while you do have
appointments, the wrong Google account is probably connected.

## Limits

- GENI never moves or cancels an appointment unless you ask
- It only sees calendars on the connected account, not colleagues' calendars that are not shared with you
- Recurring appointments are read, but the series itself is not edited
- Sending an invite asks for confirmation before the email goes out

## Troubleshooting

**Connection fails.** Check that your browser is signed in to the right Google account and try again.

**GENI does not see your appointments.** You connected a different Google account than the one holding your calendar. Disconnect and connect the right account.

**Appointment lands in the wrong time zone.** GENI follows the time zone of your Google Calendar. Check it in your Google Calendar settings.

## Disconnecting

Go to **Dashboard -> Connectors**, click Google Calendar and choose **Disconnect**.
You can also revoke access at Google itself via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Frequently asked questions

**Is this the same connection as Gmail?**
No, they are separate connectors. You connect both individually, even for the same Google account.

**Can GENI remind me about an appointment?**
Yes, through a recurring task in **Dashboard -> Tasks**. For example a daily overview every weekday at 08:00.

**Does this work with multiple calendars?**
GENI reads the calendars on the connected account. Say which one you mean in your request if you have several.

---

Back to [Connectors overview](README.md)
See also: [Google Calendar skill](../skills/google-calendar.md)
On the site: [all integrations](https://dgenix.com/integrations) · [all skills](https://dgenix.com/skills)

*dGENIX Docs, Connect Google Calendar, updated August 2026*
