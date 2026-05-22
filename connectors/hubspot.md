# HubSpot koppelen

Koppel je HubSpot CRM via een Private App Token om contacten, deals en notities te beheren via je AI-assistent.

---

## Stappen

1. Log in op je HubSpot-account
2. Ga naar *Instellingen → Integraties → Private Apps*
3. Klik op **"Een private app aanmaken"**
4. Geef de app een naam (bijv. "dGENIX")
5. Ga naar het tabblad **Scopes** en activeer:
   - `crm.objects.contacts.read` + `.write`
   - `crm.objects.deals.read` + `.write`
   - `crm.objects.notes.write`
6. Klik op **"App aanmaken"** en kopieer het gegenereerde token
7. Ga naar **Dashboard → Connectors**
8. Klik op **"Koppelen"** bij HubSpot en voer het token in

---

## Verbinding verwijderen

Verwijder de Private App in HubSpot of ga naar **Dashboard → Connectors** → klik op HubSpot → **"Verbreken"**.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [HubSpot CRM skill](../skills/hubspot.md)
