# HubSpot CRM

Manage your HubSpot CRM straight from chat. Add contacts, update deals and keep your pipeline current, without opening HubSpot manually.

---

## What can your assistant do?

- Create new contacts after a call or meeting
- Find and look up existing contacts
- Update deal status in the pipeline
- Add notes to contacts or deals
- Get a pipeline overview per stage

---

## Requirements

- **Plan:** Growth or higher
- **Integrations:** HubSpot Private App token (create in HubSpot settings)

---

## How do you activate HubSpot CRM?

1. Go to **Dashboard -> Skills**
2. Click **"Activate"** on HubSpot CRM
3. In HubSpot, create a **Private App**: *Settings -> Integrations -> Private Apps*
4. Grant the scopes: `crm.objects.contacts.read/write`, `crm.objects.deals.read/write`, `crm.objects.notes.write`
5. In dGENIX go to **Dashboard -> Connectors -> HubSpot CRM** and paste the generated token
6. The skill is active right away

---

## Example commands

```
Create a new contact: Jan Jansen, jan@company.com, CEO at CompanyX
```
```
What's the status of the deal with Client Y?
```
```
Add a note to contact jan@company.com: "Had a call on 14 April"
```
```
Give an overview of all open deals in the pipeline
```

---

## Credit cost

| Action | ~Credits |
|---|---|
| Create or find a contact | ~50 cr |
| Update a deal | ~50 cr |
| Add a note | ~40 cr |
| Pipeline overview | ~70 cr |

---

## Pricing

Included from the **Growth** plan. You pay per action in credits.

---

Back to [Skills marketplace](README.md)
