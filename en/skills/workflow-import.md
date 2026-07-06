# Workflow Builder

## What does this skill do?

With the Workflow Builder you import existing n8n workflow JSON files into dGENIX. Your assistant runs the workflow step by step via a built-in Tool Layer, from HTTP requests to emails and AI generation. Everything is tracked transparently in credits.

## Requirements

- **Plan:** Pro or higher
- **Integrations:** none, the workflow runs server-side
- **Workflow format:** n8n workflow JSON (export via n8n -> Menu -> Download as JSON)

## How do you activate the skill?

1. Go to **Skills** -> enable **Workflow Builder** (Pro required)
2. Go to **Workflow Builder** in the side menu
3. Click **Import** and paste your n8n workflow JSON
4. Give the workflow a name and an optional description

## Workflow slots

The Pro plan includes **3 workflow slots** by default. Extra slots are available as add-ons:

| Add-on | Extra slots | Price |
|---|---|---|
| +1 slot | 1 | €6.99/month |
| +5 slots | 5 | €29.99/month |
| +10 slots | 10 | €59.99/month |

Slots can be bought via **Account -> Subscription -> Workflow Builder slots**.

## What can you do with it?

**Run a workflow:**
> "Run the 'Lead Enrichment' workflow"

**Import a workflow:**
> "I want to import a new workflow"

**View workflows:**
> "Which workflows have I imported?"

## Supported node types

| Node type | Tool | Credits |
|---|---|---|
| HTTP Request | `http.request` | 5 cr/step |
| OpenAI / Anthropic | `ai.generate` | 50 cr/step |
| Send email | `email.send` | 10 cr/step |
| HubSpot CRM | `crm.create_lead` | 15 cr/step |
| Data transform (Set) | `data.transform` | 2 cr/step |
| Webhook call | `webhook.call` | 8 cr/step |

## Security restrictions

The following node types are blocked on import (server safety):

- `n8n-nodes-base.code`, code execution forbidden
- `n8n-nodes-base.executeCommand`, shell commands forbidden
- `n8n-nodes-base.ssh`, SSH connections forbidden
- `n8n-nodes-base.function`, function nodes forbidden

## Credit cost

| Action | Credits |
|---|---|
| Import a workflow | 0 cr |
| Run a workflow (base) | 25 cr + cost per step |
| List workflows | 3 cr |
| Delete a workflow | 0 cr |

Each step processes credits based on the node type (see the table above).

---

*dGENIX, Pro skill, requires a Pro plan + n8n workflow JSON*
