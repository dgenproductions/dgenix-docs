# Custom Workflows

## What does this skill do?

With Custom Workflows you connect your own n8n workflows or other webhook-based automations to the AI assistant. Provide the webhook URLs and the assistant triggers them on command, without opening the n8n dashboard.

## Requirements

- **Plan:** Growth or higher
- **Integrations:** your own webhook URLs (e.g. n8n, Make.com, Zapier)

## Setting up workflows

1. Go to **Connectors -> Custom Workflows**
2. Click **Connect**
3. Enter your workflows as a JSON array:
   ```json
   [
     { "name": "Lead follow-up", "url": "https://n8n.mycompany.com/webhook/abc123" },
     { "name": "Create invoice", "url": "https://n8n.mycompany.com/webhook/def456" }
   ]
   ```
4. Click **Test connection**, done

## What can you do with it?

**Trigger a workflow:**
> "Trigger the 'Lead follow-up' workflow"

**Get workflows:**
> "Which workflows have I connected?"

**Other examples:**
- Trigger an n8n workflow after a meeting
- Start an automatic invoice workflow
- Start a data sync via a voice command

## Credit cost

| Action | Credits |
|---|---|
| Trigger a workflow | 10 cr |
| Get workflows | 3 cr |

---

*dGENIX, Growth skill, requires webhook URL(s)*
