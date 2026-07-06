# Connect HubSpot

Connect your HubSpot CRM via a Private App token to manage contacts, deals and notes via your AI assistant.

---

## Steps

1. Log in to your HubSpot account
2. Go to *Settings -> Integrations -> Private Apps*
3. Click **"Create a private app"**
4. Give the app a name (e.g. "dGENIX")
5. Go to the **Scopes** tab and enable:
   - `crm.objects.contacts.read` + `.write`
   - `crm.objects.deals.read` + `.write`
   - `crm.objects.notes.write`
6. Click **"Create app"** and copy the generated token
7. Go to **Dashboard -> Connectors**
8. Click **"Connect"** on HubSpot and enter the token

---

## Removing the connection

Delete the Private App in HubSpot, or go to **Dashboard -> Connectors** -> click HubSpot -> **"Disconnect"**.

---

Back to [Connectors overview](README.md)
See also: [HubSpot CRM skill](../skills/hubspot.md)
