# Workflow Builder

## Wat doet deze skill?

Met de Workflow Builder importeer je bestaande n8n workflow JSON bestanden in dGENIX. Je assistent voert de workflow stap-voor-stap uit via een ingebouwde Tool Layer — van HTTP requests tot e-mails en AI-generatie. Alles wordt transparant in credits bijgehouden.

## Vereisten

- **Plan:** Pro of hoger
- **Integraties:** Geen — workflow draait server-side
- **Workflow formaat:** n8n workflow JSON (exporteer via n8n → Menu → Download als JSON)

## Hoe activeer je de skill?

1. Ga naar **Skills** → zet **Workflow Builder** aan (Pro vereist)
2. Ga naar **Workflow Builder** in het zijmenu
3. Klik **Importeren** en plak je n8n workflow JSON
4. Geef de workflow een naam en optionele beschrijving

## Workflow slots

Pro-plan bevat **3 workflow slots** standaard. Extra slots zijn beschikbaar via add-ons:

| Add-on | Extra slots | Prijs |
|---|---|---|
| +1 slot | 1 | €6,99/mnd |
| +5 slots | 5 | €29,99/mnd |
| +10 slots | 10 | €59,99/mnd |

Slots zijn te kopen via **Billing → Workflow Builder slots uitbreiden**.

## Wat kun je ermee?

**Workflow uitvoeren:**
> "Voer de workflow 'Lead Enrichment' uit"

**Workflow importeren:**
> "Ik wil een nieuwe workflow importeren"

**Workflows bekijken:**
> "Welke workflows heb ik geïmporteerd?"

**Andere voorbeelden:**
- Bestaande n8n automatisering via chat triggeren
- HTTP API calls en e-mailverzending combineren
- Data transformeren en opslaan via workflow

## Ondersteunde node-types

| Node type | Tool | Credits |
|---|---|---|
| HTTP Request | `http.request` | 5 cr/stap |
| OpenAI / Anthropic | `ai.generate` | 50 cr/stap |
| E-mail versturen | `email.send` | 10 cr/stap |
| HubSpot CRM | `crm.create_lead` | 15 cr/stap |
| Data transformatie (Set) | `data.transform` | 2 cr/stap |
| Webhook call | `webhook.call` | 8 cr/stap |

## Beveiligingsbeperkingen

De volgende node-types zijn geblokkeerd bij importeren (server-veiligheid):

- `n8n-nodes-base.code` — code uitvoering verboden
- `n8n-nodes-base.executeCommand` — shell commando's verboden
- `n8n-nodes-base.ssh` — SSH verbindingen verboden
- `n8n-nodes-base.function` — functie nodes verboden

## Creditkosten

| Actie | Credits |
|---|---|
| Workflow importeren | 0 cr |
| Workflow uitvoeren (base) | 25 cr + kosten per stap |
| Workflows oplijsten | 3 cr |
| Workflow verwijderen | 0 cr |

Elke stap in de workflow verwerkt credits op basis van het node-type (zie tabel hierboven).

---

*dGENIX — Pro skill — Vereist: Pro-plan + n8n workflow JSON*
