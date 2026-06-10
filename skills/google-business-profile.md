# Google Bedrijfsprofiel

Beheer je Google Business Profile via de AI-assistent. Reviews analyseren, posts plaatsen, openingstijden aanpassen en bedrijfsinfo ophalen zonder het Google-dashboard te openen.

**Vereisten:** Growth+ abonnement, Google-account koppelen via Instellingen

---

## Beschikbare acties

| Actie | Creditkosten | Omschrijving |
|---|---|---|
| `profiel_info` | 15 cr | Bedrijfsinfo ophalen (naam, adres, telefoonnummer, website) |
| `reviews_analyseren` | 50 cr | Reviews ophalen met sentimentscore en samenvattende analyse |
| `post_maken` | 25 cr | Google Business post schrijven en publiceren |
| `review_beantwoorden` | 20 cr | Professionele reactie opstellen op een specifieke review |
| `openingstijden_bijwerken` | 15 cr | Openingstijden aanpassen (ook voor feestdagen) |

---

## Verbinding koppelen

1. Ga naar **Instellingen > Integraties**
2. Klik op **Verbinden** bij Google Bedrijfsprofiel
3. Log in met het Google-account dat toegang heeft tot je Business Profile
4. Geef toestemming voor `business.manage`

De koppeling werkt alleen als je een geverifieerd Google Business Profile hebt.

---

## Voorbeeldgesprekken

**Reviews analyseren:**
> "Analyseer mijn Google-reviews van de afgelopen maand"

**Post aanmaken:**
> "Maak een Google Business post voor onze zomeractie dit weekend"

**Openingstijden bijwerken:**
> "Pas mijn openingstijden aan voor tweede Kerstdag: gesloten"

**Review beantwoorden:**
> "Schrijf een professionele reactie op de negatieve review over de wachttijden"

---

## Tips

- Gebruik `reviews_analyseren` wekelijks voor een snel overzicht van klanttevredenheid
- Google Business posts verlopen na 7 dagen — plan regelmatige updates
- Bij wijziging van openingstijden duurt het enkele minuten voordat Google de update toont
- De skill werkt alleen met geverifieerde bedrijfslocaties

---

## Beperkingen

- Foto's uploaden wordt niet ondersteund (Google API-beperking)
- Antwoorden op reviews zijn definitief en niet verwijderbaar via de API
- Maximaal 1 locatie per Google-account koppeling
