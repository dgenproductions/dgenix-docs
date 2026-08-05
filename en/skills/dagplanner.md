# Daily Planner & Life Assistant

With the Daily Planner GENI builds an overview of your day, orders your tasks by priority and sets up recurring tasks for you.

Available from **Starter**. No connection needed, though Google Calendar makes
the overview complete.

## What can GENI do with it?

- **Build a daily overview** for today or another date, including your appointments if Google Calendar is connected
- **Prioritise tasks** by urgency, impact and the time you have
- **List your recurring tasks**
- **Create a recurring task** (daily, weekly or monthly, at a fixed time)
- **Edit a recurring task** or switch it off temporarily
- **Delete a recurring task**

Note the difference: the first two are about your day, the last four manage
**Automations** , tasks GENI runs itself at a set moment. See
[Scheduled tasks](../handleiding/geplande-taken.md).

## Example: what you ask, what you get

```
What does my day look like?
```

> **Wednesday 5 August**
>
> **Fixed in the calendar**
> - 09:30-10:00 , Standup
> - 14:00-15:00 , Client call De Krent
> - 16:30-17:00 , Supplier call
>
> **You have two blocks free:** 10:00-14:00 and 15:00-16:30
>
> **What is outstanding**
> - Finish the De Krent quote , before the 14:00 call, so in the morning block
> - Send invoice 2026-084 , 10 minutes, fits in between
> - Write the quarterly plan , will not fit today, tomorrow morning
>
> Shall I put your morning block on the quote?

And for a recurring task:

```
Send me a summary of my week every Monday at 8
```

> Done. **Week-start summary**, every Monday at 08:00.
> You will find it under Automations, where you can also pause it.

## Requirements

- **Plan:** Starter and up
- **Connection:** none. [Google Calendar](google-calendar.md) is optional but strongly recommended

## Activating

1. Go to **Dashboard -> Skills** and activate **Daily Planner & Life Assistant**
2. Optionally connect Google Calendar through **Dashboard -> Connectors**
3. Ask for a daily overview

## What it costs

| Action | Credits |
|---|---|
| Any daily planner action | 3 |

That is the cheapest skill on the platform. On top of those 3 credits comes the
conversation itself; see [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Without Google Calendar GENI does not know your appointments.** The overview then covers only what you tell it and your tasks.
- **A schedule is a proposal**, not a calendar change. Ask [Google Calendar](google-calendar.md) to actually book it.
- **Recurring tasks count against your slots**: Free 0, Starter 1, Growth 5, Pro 10, Business 20.
- **The shortest interval is daily.** Several times a day is not possible.
- **Prioritising works on what you supply.** GENI does not know your unspoken deadlines unless you mention them or store them in your [memory](../functies/geheugen.md).

## Troubleshooting

**My appointments are missing.** Google Calendar is not connected, or the overview covers a different day. Name the date explicitly.

**The prioritisation makes no sense.** Supply context: hard deadlines, how much time you have, and how demanding the work is.

**My recurring task is not running.** Check under Automations whether it is switched on and whether you have slots left; with too few credits it gets paused.

**It creates a task when I only wanted an overview.** Say "show me" or "give me an overview" instead of "set up".

## Frequently asked questions

**What is the difference with the Workspace?**
The [Workspace](../functies/werkruimte.md) is where you keep notes and to-dos.
The Daily Planner looks at your day and orders what is outstanding.

**Does it remember my working rhythm?**
If you tell it, yes. Say you are sharpest in the morning and GENI stores that in
your memory and takes it into account.

**Can it move my appointments?**
Not from this skill. With [Google Calendar](google-calendar.md) connected it
can, and it asks for confirmation first.

**Does this work through Telegram too?**
Yes, if you use the Telegram add-on. A daily overview at 8 on your phone is a
common automation.

---

Back to [Skills marketplace](README.md)
See also: [Google Calendar](google-calendar.md) · [Scheduled tasks](../handleiding/geplande-taken.md) · [Workspace](../functies/werkruimte.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Daily Planner & Life Assistant, updated August 2026*
