# Workflow Automations

Workflow Automations are recurring commands GENI runs automatically at set times, with no effort from you.

The rule of thumb: anything you can ask by hand you can also schedule. If a
request works in chat, it works as an automation.

## What you can do with it

| What you schedule | When it runs |
|---|---|
| Daily overview of your inbox and calendar | Every weekday at 08:00 |
| Weekly report to your mailbox | Every Monday |
| SEO audit of your site | Monthly |
| Review requests to new customers | Every Monday |
| Social post from your latest blog | Weekly |

---

## How does it work?

1. Create a workflow with a name, instruction and frequency
2. The assistant runs the task automatically at the set time
3. You receive the result (in the dashboard, and via Telegram if you use the add-on)

---

## Creating a workflow

1. Go to **Dashboard -> Tasks**
2. Click **+ New workflow**
3. Fill in:
   - **Name:** a short description (for example "Daily news summary")
   - **Instruction:** what exactly should the assistant do?
   - **Frequency:** how often should the task run?
4. Save, the workflow is active right away

**Tip:** write the instruction as if you are addressing the assistant directly. The more specific, the better the result.

---

## Available frequencies

| Frequency | Time |
|------------|----------|
| Daily | 08:00 |
| Weekdays (Mon-Fri) | 08:00 |
| Weekly | Monday 08:00 |
| Monthly | 1st of the month |

---

## Examples

- *Daily:* "Give me a summary of today's news"
- *Weekdays:* "Send me a motivational quote for the day"
- *Weekly:* "Make a weekly plan based on my calendar"
- *Monthly:* "Remind me to check my invoices and send an overview of my fixed costs"

---

## Slots per plan

| Plan | Slots included |
|------|-----------------|
| Free | 0 slots |
| Starter | 1 slot |
| Growth | 5 slots |
| Pro | 10 slots |
| Business | 20 slots |

**Extra slots** (from Pro), via **Account -> Subscription**:

| Pack | Price |
|---|---|
| +1 slot | €6.99/mo |
| +5 slots | €29.99/mo |
| +10 slots | €59.99/mo |

---

## Managing workflows

### Enable / disable
Use the toggle next to a workflow to pause it temporarily. It is not deleted, just skipped at the next run time.

### Run history
Click the clock icon next to a workflow to see the last 10 runs: status (success / error), credits used and a result summary.

### Edit
Click the pencil icon to change the name, instruction or frequency.

### Delete
Click the trash icon. The workflow is permanently removed.

---

## Google Calendar integration

If you connected Google Calendar (via **Connectors**), a **GCal** button appears next to each workflow. Click it to add the workflow as a recurring calendar event, so you also see the tasks in your calendar.

---

## Credits

Each automatic run uses credits based on the complexity of the task and the model used. See the credit cost per run in the run history.

---

## Tabs: Workflows and Templates

The page has two tabs at the top:

- **Workflows**, your active scheduled workflows with a calendar + list + slot packs
- **Templates**, ready-made examples to set up a workflow quickly

You can link directly to a tab via `?tab=workflows` or `?tab=templates` in the URL, handy to share with your team.

---

## Workflow Templates

The Templates tab has ready-made examples for recurring workflows. Each template has a title, a short description and the skills it needs.

### For you

At the top is a **For you** row: templates that best match your plan and active skills. Click **Refresh** for a new selection.

### Category sections

Below that you see templates per category: Marketing, Sales, Content, Research, Communication, Reporting, Operations and Personal.

### Search and filter

- The **search bar** filters by title, description and skill slug
- The **category dropdown** limits the view to one category

### Using a template

Click a template card to open a form with the title and instruction pre-filled, plus frequency and time. In the instruction you see text in brackets like `[my segment name]`, **replace those with your own details**. Anything you leave out, the assistant asks for on the first run.

### Skills not yet active

If a template needs skills you have not activated, you see a warning badge on the card and a banner in the form with a direct link to the Skills marketplace. You can still create the workflow, but it fails on each run until the skills are activated.

### No template found?

If your search returns nothing, two buttons appear: **New workflow** (build one from scratch) and **Request a template** (describe what you are missing; the request goes to dGENIX support).

---

## Limits

- **The number of slots depends on your plan**: Free 0, Starter 1, Growth 5, Pro 10, Business 20. Extra slots can be bought separately from Pro.
- **Irreversible actions ask for confirmation inside an automation too.** No email or publication ever goes out unseen.
- **An automation fails if a required skill or connection is missing.** You see that as a warning on the template beforehand.
- **Credits are deducted per run.** A heavy daily task adds up; check the cost per run first.
- **Without credits execution stops** until your balance is topped up.
- **The smallest frequency is daily.** For anything more frequent, start it by hand.

## Troubleshooting

**Your automation does not run.** Check whether it is switched on and whether you still have credits. A paused task stays but executes nothing.

**It fails every time.** A skill or connection is probably missing. The overview shows the last run with the error.

**You cannot create a new automation.** Your slots are full. Delete an existing one or buy extra slots.

**The result does not reach you.** Check that the task has a delivery step, for example "email the result to me". Without it the result stays in the dashboard.

**The timing is off.** Execution follows your account's time zone; check it in Settings.

## Frequently asked questions

**What is the difference with a Workspace task?**
An automation is executed by GENI at a set time. A Workspace task is a to-do you
tick off. See [Workspace](werkruimte.md).

**Can I pause an automation?**
Yes, with the on/off switch. Your settings are kept.

**Does an automation cost extra?**
The automation itself does not; only the work it performs uses credits, just as
when you ask for it by hand.

**Can I see what has run?**
Yes, each automation shows its last run with the result, and everything also
appears in your Workspace timeline.

---

Next: [Scheduled tasks](../handleiding/geplande-taken.md) · [Workspace](werkruimte.md) · [The credit system](../hoe-het-werkt/credits.md)
On the site: [pricing](https://dgenix.com/pricing)

*dGENIX Docs, Workflow Automations, updated August 2026*
