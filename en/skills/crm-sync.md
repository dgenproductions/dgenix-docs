# CRM Sync

## What does this skill do?

The CRM Sync skill connects your HubSpot CRM data to your AI assistant. Fetch contacts and deal statuses, get pipeline reports and keep your sales pipeline up to date, without opening the HubSpot dashboard.

## Requirements

- **Plan:** Pro or higher
- **Integrations:** HubSpot Private App token

## Connecting HubSpot

1. Log in to HubSpot -> **Settings -> Integrations -> Private Apps**
2. Create a new Private App with scopes: `crm.objects.contacts.read`, `crm.objects.deals.read`, `crm.objects.deals.write`
3. Copy the Access Token
4. In dGENIX go to **Connectors -> HubSpot CRM**
5. Click **Connect** and paste the token
6. Click **Test connection**, done

## What can you do with it?

**Fetch contacts:**
> "Get my 20 newest HubSpot contacts"

**View the deal pipeline:**
> "Show all open deals in the pipeline and their status"

**Generate a CRM report:**
> "Make a summary report of my CRM pipeline for this week"

**Other examples:**
- Identify stalled deals
- Find contacts by company or sector
- Calculate pipeline value

## Credit cost

| Action | Credits |
|---|---|
| Fetch contacts | 15 cr |
| Update deal status | 5 cr |
| Generate CRM report | 15 cr |

---

*dGENIX, Growth skill, requires a HubSpot Private App token*
