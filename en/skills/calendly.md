# Calendly

With the Calendly skill GENI fetches your event types, scheduled meetings and free time slots, so you do not have to switch between calendars.

Available from **Growth**. You need a connected Calendly account.

## What can GENI do with Calendly?

- **List your event types**, for example intro call, advisory session, demo
- **Fetch upcoming meetings**
- **Retrieve available time slots** for a specific event type

## Example: what you ask, what you get

```
What calls are scheduled this week?
```

> **5 meetings through Calendly**
>
> | When | Type | With |
> |---|---|---|
> | Mon 09:00 | Intro call (30 min) | Sanne de Wit |
> | Tue 14:00 | Advisory session (60 min) | Bakkerij De Krent |
> | Wed 11:00 | Intro call (30 min) | Mark Jansen |
> | Thu 10:30 | Demo (45 min) | Studio Noord |
> | Fri 15:00 | Advisory session (60 min) | Van Dijk BV |
>
> Thursday is your only day with a free morning block. Shall I prepare for
> Tuesday's advisory session?

## Requirements

- **Plan:** Growth and up
- **Connection:** a Calendly account via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Calendly**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Ask about your meetings, types or availability

## What it costs

These are light read actions; they cost a small number of credits per query. The
amount shows on the button before you start. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Read only.** GENI does not book Calendly meetings and does not move or cancel them.
- **No creating or editing event types.** You do that in Calendly.
- **No sending invitations.** You share your Calendly link yourself.
- **Upcoming meetings**, not full history.
- **To book something yourself**, use [Google Calendar](google-calendar.md); that one can create appointments.

## Troubleshooting

**No meetings come through.** None are scheduled in the fetched period, or the connected account is not the one receiving the bookings.

**An event type is missing.** Check that it is active in Calendly; hidden types are not shown.

**Availability does not match your expectation.** Calendly works from your configured working hours and buffers. Adjust those there.

**You want to move a meeting.** That goes through Calendly itself or through the customer; GENI cannot.

## Frequently asked questions

**Can GENI summarise my day including Calendly?**
Yes, combined with [Google Calendar](google-calendar.md) and [Gmail](gmail.md)
you get one daily overview instead of three screens.

**Can I schedule this?**
Yes, for example an overview of your week every Monday. See
[Scheduled tasks](../handleiding/geplande-taken.md).

**Can it prepare me for a call?**
Yes, combined with [Lead Research](lead-research.md) it finds out who you are
meeting before you sit down.

**What is the difference with Google Calendar?**
Calendly is about meetings others book with you. Google Calendar is your own
calendar, which GENI can also book into.

---

Back to [Skills marketplace](README.md)
See also: [Google Calendar](google-calendar.md) · [Lead Research](lead-research.md) · [Day planner](dagplanner.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Calendly, updated August 2026*
