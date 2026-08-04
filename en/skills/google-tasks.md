# Google Tasks

With the Google Tasks skill GENI keeps your task list: adding tasks, ticking them off and putting them in order of urgency.

Available from **Starter**. You need a connected Google account.

## What can GENI do with Google Tasks?

- **Fetch open tasks**, with title, deadline and note
- **Create a task**, with an optional deadline and note
- **Complete a task**
- **Plan your tasks**: order them by priority and turn them into an action plan

That last one is the difference with an ordinary to-do app: GENI looks at
deadlines and urgency and tells you where to start today.

## Example: what you ask, what you get

```
What should I do today?
```

> You have **7 open tasks**. This is what I would do today:
>
> 1. **File VAT return** , due tomorrow. Statutory deadline, start here.
> 2. **Send De Vries contract** , they have been waiting since Tuesday.
> 3. **Finish the bakery quote** , due Friday, about an hour left.
>
> The other 4 have no deadline and can wait. Shall I tick off the first when
> you are done?

## Requirements

- **Plan:** Starter and up
- **Connection:** a Google account via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Google Tasks**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Complete the Google consent screen
4. Google Tasks is usable right away

## What it costs

| Action | Credits |
|---|---|
| Fetch tasks | 15 |
| Create a task | 15 |
| Complete a task | 15 |
| Prioritise and plan tasks | 25 |

The skill is included in your plan; you pay per action. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI does not delete tasks.** It can complete them; discarding is yours to do.
- **Subtasks are not created.** It works with tasks at one level.
- **Recurring tasks are read, not configured.**
- **Creating or completing a task asks for confirmation.**
- **Only the connected account's lists.**

## Troubleshooting

**Your tasks do not come through.** The connection is missing or expired, or your tasks sit in a list other than the default one.

**The deadline arrives wrong.** Google Tasks only knows a date, not a time. If you want a time, put it in the title or use your [calendar](google-calendar.md).

**The prioritisation does not match your instinct.** GENI weighs deadlines most. Say what matters to you and it takes that into account.

**A completed task is still showing.** Google Tasks only hides completed tasks after a refresh. Reload the app.

## Frequently asked questions

**What is the difference with Workspace tasks?**
Google Tasks syncs with your Google account, so you see them on your phone too.
[Workspace tasks](../functies/werkruimte.md) stay inside dGENIX and connect to
your notes and timeline.

**Can GENI run through my task list every morning?**
Yes, as a scheduled task, often together with your calendar and inbox. See
[Scheduled tasks](../handleiding/geplande-taken.md).

**Does this work with several task lists?**
It reads your lists; new tasks go into your default list.

**Can it pull tasks out of a conversation?**
Yes, ask it to stage the action items from a conversation as tasks.

---

Back to [Skills marketplace](README.md)
See also: [Google Calendar](google-calendar.md) · [Workspace](../functies/werkruimte.md) · [Day planner](dagplanner.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Google Tasks, updated August 2026*
