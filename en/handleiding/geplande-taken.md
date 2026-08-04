# Scheduled tasks & automation

With scheduled tasks you let your assistant run commands on a fixed schedule, with no effort from you. Set it once, it does the rest.

---

## What are scheduled tasks?

A scheduled task is a command you set up once, after which your assistant runs it automatically at the time you want.

**Examples:**
- Every Monday at 08:30, an overview of your calendar for the week
- Every day at 09:00, three priorities based on your inbox
- Every Friday at 17:00, a weekly report from your activities
- On the 1st of each month, a financial overview from Google Sheets

---

## How do you set up a task?

1. Go to **Dashboard -> Tasks**
2. Click **"New task"**
3. Fill in:
   - **Name**, what do you call the task? (internal, for yourself)
   - **Command**, what should the assistant do? Write it like a normal chat message
   - **Frequency**, when should it run?
4. Click **Save**

The task appears in the overview. You can pause, edit or delete it.

---

## Frequencies

| Option | When |
|---|---|
| Once | On a specific date and time |
| Daily | Every day at the same time |
| Weekdays | Monday to Friday at the same time |
| Weekly | Every week on the same day and time |
| Monthly | Every month on the same date and time |

---

## Writing the command

Write the command as you would send a message to your assistant. It runs exactly as if you sent it yourself.

**Good commands are specific:**

Less good: "make a report"
Better: "Make a weekly report of my Google Calendar appointments from last week. Use an overview format with sections per day."

**Your assistant has access to:** your connected Google Calendar, Gmail, Google Sheets, Google Drive; your active skills; your knowledge document and instructions.

**Your assistant does NOT have access to:** information outside your connected services; real-time data (news, weather) unless you have the relevant skill.

---

## Run overview

In the Tasks dashboard you see per task: status (active, paused or disabled), last run, and result (whether the run succeeded). You can also view the run history per task.

---

## Receiving results

When a task runs, your assistant receives the result and saves it. Depending on the command:

- **Text answers** appear as a message in your web chat (a new session)
- **Files** are saved in your Assets overview
- If you have **Telegram** connected, you also receive a Telegram message

---

## Credit cost

Scheduled tasks use credits at run time. The cost is the same as for manual commands:

| Task type | ~Credits |
|---|---|
| Fetch a calendar overview | 50-150 cr |
| Email summary | 100-200 cr |
| Generate a report | 150-500 cr |
| Create a social post | 100-300 cr |

Note: tasks run even if your balance is low. Make sure you have enough credits for critical tasks.

---

## Practical ideas

**Productivity:**
- Daily 08:00, "Give me three priorities for today based on my calendar"
- Monday 09:00, "Overview of all appointments this week with locations and attendees"

**Communication:**
- Friday 16:00, "Check my inbox for unanswered emails older than 3 days and make a list"

**Reporting:**
- Monthly, 1st at 08:00, "Pull last month's revenue from my Google Sheets and summarise it"

**Content:**
- Monday 10:00, "Draft a LinkedIn post based on something I did last week" _(combine with the Social Media skill)_

---

## Tips

**Test your task manually first.** Send the command as a normal chat message and check the result, then set it up as a scheduled task.

**Be specific about the format you want.** A report task is only useful if you also say what the report should look like.

**Use frequency 'once' for deadlines.** For a reminder before a specific deadline, set a one-time task on the day before.

---

## What you see

You schedule a daily overview for every weekday at 08:00. From the next morning
this is waiting without you asking:

> **Good morning. Here is today.**
>
> - **10:00** , call De Vries about the quote
> - **13:30** , supplier, Industrieweg 4
> - **16:00** , team meeting
>
> **From your inbox:** 2 emails need action. The accountant wants the VAT
> figures before the 25th, and Sofie is waiting on the contract.
>
> Your only free block is between 12:00 and 13:30.

Exactly what you would have got by asking, except you did not have to remember
to ask.

## Limits

- **The number of tasks depends on your plan**: Free 0, Starter 1, Growth 5, Pro 10, Business 20.
- **Irreversible actions ask for confirmation here too.** A scheduled task that sends or publishes waits for your approval.
- **Credits are deducted per run.** A heavy daily task adds up; work out what a month costs first.
- **Without credits execution stops** until your balance is topped up. You get a notification.
- **If a skill or connection is missing, the task fails.** So test the request by hand first.
- **The smallest frequency is daily.** Anything more frequent you start yourself.

## Troubleshooting

**The task does not run.** Check whether it is switched on and whether credits remain. A paused task stays but executes nothing.

**It keeps failing.** The run history shows the error. Usually a connection is missing or has expired.

**The result does not reach you.** Without a delivery step it stays in the dashboard. State in the request where it should go, for example "email the result to me".

**It runs at an odd time.** Timing follows your account's time zone; check it in Settings.

**The result varies a lot between runs.** Make the request more specific, especially about the format you want. Vague instructions produce variable output.

## Frequently asked questions

**What is the difference with a Workspace task?**
A scheduled task is executed by GENI at a set time. A Workspace task is a to-do
you tick off. See [Workspace](../functies/werkruimte.md).

**Can I pause a task?**
Yes, with the on/off switch. Your settings are kept.

**Can I see what has run?**
Yes, each task has a run history with status, credits and result.

**Does a scheduled task cost extra?**
No, only the work it performs uses credits, just as when you ask yourself.

---

Next: [Workflow Automations](../functies/workflow-automations.md) · [Workspace](../functies/werkruimte.md) · [The credit system](../hoe-het-werkt/credits.md)
On the site: [pricing](https://dgenix.com/pricing)

*dGENIX Docs, Scheduled tasks, updated August 2026*
