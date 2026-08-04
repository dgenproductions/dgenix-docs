# Google Calendar

With the Google Calendar skill GENI looks into your calendar and schedules appointments, so you do not have to puzzle over time slots yourself.

Available from **Starter**. You need a connected Google account; see
[Connecting Google Calendar](../connectors/google-calendar.md).

## What can GENI do with Google Calendar?

- **View your calendar** for a day, a week or a period you choose
- **Schedule an appointment** with date, time, title and location

That lets you ask for your day, have free blocks found and get appointments
created without opening the calendar app.

## Example: what you ask, what you get

```
What is on my calendar tomorrow?
```

> **Thursday 7 August**
>
> - **10:00-11:00** , Client call De Vries
> - **13:30-14:30** , Supplier, Industrieweg 4
> - **16:00-17:00** , Team meeting
>
> You have one free block from 11:00 to 13:30.

When scheduling you see what is about to be created:

```
Book an hour on Friday at 14:00 with ABC about the quote
```

> **Client call ABC , quote**
> Friday 8 August, 14:00-15:00
>
> This does not clash with your other appointments. Shall I create it?

## Requirements

- **Plan:** Starter and up
- **Connection:** a Google account via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Google Calendar**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Complete the Google consent screen
4. The calendar is usable right away

## What it costs

| Action | Credits |
|---|---|
| View calendar | ~20 |
| Create an appointment | ~28 |
| Find free time | ~20 |

The skill is included in your plan; you pay per action. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Creating an appointment asks for confirmation.** You see date, time and title first.
- **GENI does not delete or move existing appointments.**
- **It cannot invite guests.** It creates the appointment; you add attendees yourself.
- **Recurring appointments are read, not created.**
- **Only the connected account's calendars.** Colleagues' calendars stay out of view.
- **It works in your account's time zone.** Check that if times look off.

## Troubleshooting

**Your calendar comes back empty.** The connection is missing or expired, or your appointments sit in a calendar other than the connected account's main one.

**The appointment lands at the wrong time.** Probably a time zone difference. Check the time zone in [Settings](../functies/instellingen.md).

**A double booking is not flagged.** Ask explicitly whether it clashes; then GENI checks your existing appointments.

**You want to invite someone.** That does not go through GENI. Create the appointment and add the guests yourself in Google Calendar.

## Frequently asked questions

**Can GENI walk me through my day every morning?**
Yes, as a scheduled task. Often combined with [Gmail](gmail.md), so you get your
calendar and action items in one message. See
[Scheduled tasks](../handleiding/geplande-taken.md).

**Does this work with several calendars?**
It reads the connected account's calendars. It creates appointments in your main
calendar.

**Can I use the skill without connecting Gmail?**
Yes. You grant permission per Google service separately.

**Does dGENIX see the content of my appointments?**
Only what is needed to answer your question, at the moment you ask it.

---

Back to [Skills marketplace](README.md)
See also: [Connecting Google Calendar](../connectors/google-calendar.md) · [Gmail](gmail.md) · [Google Tasks](google-tasks.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Google Calendar, updated August 2026*
