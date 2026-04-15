# Eigen Workflows

## Wat doet deze skill?

Met Eigen Workflows koppel je je eigen n8n workflows of andere webhook-gebaseerde automatiseringen aan de AI-assistent. Geef de webhook-URL's op, en de assistent triggert ze op commando — zonder dat je het n8n-dashboard hoeft te openen.

## Vereisten

- **Plan:** Growth of hoger
- **Integraties:** Eigen webhook-URLs (bijv. n8n, Make.com, Zapier)

## Workflows instellen

1. Ga naar **Instellingen → Integraties → Eigen Workflows**
2. Klik **Koppelen**
3. Voer je workflows in als JSON-array:
   ```json
   [
     { "naam": "Lead opvolging", "url": "https://n8n.mijnbedrijf.nl/webhook/abc123" },
     { "naam": "Factuur aanmaken", "url": "https://n8n.mijnbedrijf.nl/webhook/def456" }
   ]
   ```
4. Klik **Verbinding testen** — klaar

## Wat kun je ermee?

**Workflow triggeren:**
> "Trigger de workflow 'Lead opvolging'"

**Workflows ophalen:**
> "Welke workflows heb ik gekoppeld?"

**Andere voorbeelden:**
- n8n workflow triggeren na een vergadering
- Automatische factuur workflow starten
- Data-synchronisatie starten via spraakcommando

## Creditkosten

| Actie | Credits |
|---|---|
| Workflow triggeren | 10 cr |
| Workflows ophalen | 3 cr |

---

*dGENIX — Growth skill — Vereist: webhook-URL(s)*
