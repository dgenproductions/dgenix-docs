# Google Analytics

Website traffic inzichten direct in de chat via Google Analytics 4. Bezoekerscijfers, toppaginas, verkeersbronnen en doelgroepdata — zonder het Analytics dashboard te openen.

**Vereisten:** Growth+ abonnement, Google-account koppelen via Instellingen

---

## Beschikbare acties

| Actie | Creditkosten | Omschrijving |
|---|---|---|
| `analytics_overzicht` | 35 cr | Algemeen bezoekersoverzicht (sessies, gebruikers, bouncepercentage) |
| `beste_paginas` | 30 cr | Toppaginas gerangschikt op weergaven en sessieduur |
| `verkeersbronnen_rapport` | 35 cr | Analyse van traffic sources (organisch, sociaal, direct, betaald) |
| `doelgroep_inzichten` | 40 cr | Demografische en gedragsdata (leeftijd, apparaat, land, retentie) |

---

## Verbinding koppelen

1. Ga naar **Instellingen > Integraties**
2. Klik op **Verbinden** bij Google Analytics
3. Log in met het Google-account dat toegang heeft tot je GA4 property
4. Geef toestemming voor `analytics.readonly`

Bij het eerste gebruik vraagt de assistent om het GA4 property ID (te vinden in GA4 > Beheer > Property-instellingen).

---

## Voorbeeldgesprekken

**Wekelijks rapport:**
> "Geef me het bezoekersoverzicht van de afgelopen 7 dagen"

**Toppaginas:**
> "Welke paginas hebben het meeste verkeer gegenereerd afgelopen maand?"

**Verkeersbronnen:**
> "Hoe verhoudt organisch zoekverkeer zich tot social media verkeer?"

**Doelgroep:**
> "Welk percentage van mijn bezoekers gebruikt een mobiel apparaat?"

---

## Tips

- Sla je GA4 property ID op in je kennisdocument zodat je het niet steeds opnieuw hoeft op te geven
- Gebruik `doelgroep_inzichten` voor campagne-optimalisatie en targeting
- Combineer met Search Console voor een volledig SEO-beeld
- Periodenotatie: "afgelopen 7 dagen", "vorige maand", "dit kwartaal"

---

## Beperkingen

- Alleen lezen (geen data aanpassen of events aanmaken)
- Doelen en conversies zijn niet beschikbaar via de Data API v1
- Realtimedata wordt niet ondersteund in deze skill
