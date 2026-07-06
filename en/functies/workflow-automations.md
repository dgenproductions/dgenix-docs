# Workflow Automations

Workflow Automations are recurring commands your assistant runs automatically at set times, with no effort from you.

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
| Starter | 1 slot |
| Growth | 5 slots |
| Pro | 15 slots |

**Extra slots:** available to buy via **Account -> Subscription** (slot add-on packs).

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
