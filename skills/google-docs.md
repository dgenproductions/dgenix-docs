# Google Docs

Google Docs aanmaken, lezen, bewerken en samenvatten via de AI-assistent. Geen browser nodig — de document-link wordt direct teruggegeven.

**Vereisten:** Growth+ abonnement, Google-account koppelen via Instellingen

---

## Beschikbare acties

| Actie | Creditkosten | Omschrijving |
|---|---|---|
| `docs_document_lezen` | 15 cr | Document ophalen op basis van document-ID of URL |
| `docs_document_aanmaken` | 650 cr | Nieuw document aanmaken met volledige AI-gegenereerde inhoud |
| `docs_samenvatten` | 65 cr | Lang document samenvatten in kernpunten |
| `docs_bewerken` | 25 cr | Specifieke sectie aanpassen of herschrijven |

---

## Verbinding koppelen

1. Ga naar **Instellingen > Integraties**
2. Klik op **Verbinden** bij Google Docs
3. Log in met het Google-account dat de doeldocumenten bezit
4. Geef toestemming voor `documents` (lezen en schrijven)

---

## Voorbeeldgesprekken

**Document aanmaken:**
> "Maak een Google Doc aan met een gedetailleerde projectbeschrijving voor onze nieuwe webshop"

**Document samenvatten:**
> "Vat dit document samen in 5 kernpunten: docs.google.com/document/d/1abc123..."

**Document bewerken:**
> "Herschrijf de introductie van mijn offerte-document zodat het zakelijker klinkt"

**Document lezen:**
> "Haal de inhoud op van mijn strategiedocument: [document-URL]"

---

## Tips

- `docs_document_aanmaken` gebruikt Claude Sonnet voor de beste schrijfkwaliteit (650 cr)
- Geef de assistent context mee: doelgroep, toon, gewenste lengte
- Gebruik `docs_samenvatten` voor lange rapporten voordat je ze met anderen deelt
- De teruggekregen document-link is direct klikbaar in de chat

---

## Beperkingen

- Afbeeldingen en tabellen zijn niet beschikbaar via de API (tekst-only)
- Formulieren (Google Forms) worden niet ondersteund
- Gedeelde documenten waar je geen eigenaar van bent vereisen expliciete leesrechten
