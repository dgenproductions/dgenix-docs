# Factuur Automator

Met de Factuur Automator maakt GENI een complete factuur uit een paar regels tekst, rekent hij de btw uit en zet hij het bestand in je Drive.

Beschikbaar vanaf **Pro**. Voor opslaan in Drive heb je
[Google Drive](google-drive.md) nodig.

## Wat kan GENI hiermee?

- **Een factuur aanmaken** met klantgegevens, factuurregels, btw-percentage en een factuurnummer (of automatisch doorgenummerd)
- **De factuur opslaan in Google Drive**

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Factuur voor De Krent: website bouw 1x 1500, kassakoppeling 1x 850,
onderhoud 3 maanden a 95
```

> **Factuur 2026-085 , De Krent**
>
> | Omschrijving | Aantal | Bedrag |
> |---|---|---|
> | Website bouw | 1 | € 1.500,00 |
> | Kassakoppeling | 1 | € 850,00 |
> | Onderhoud (per maand) | 3 | € 285,00 |
>
> Subtotaal € 2.635,00
> Btw 21 procent € 553,35
> **Totaal € 3.188,35**
>
> Betaaltermijn 14 dagen.
>
> Zal ik hem in je Drive zetten? Ik heb geen adres van De Krent, dat wil je er
> waarschijnlijk bij hebben.

## Vereisten

- **Plan:** Pro en hoger
- **Koppeling:** geen om de factuur te maken. [Google Drive](google-drive.md) om hem op te slaan

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Factuur Automator**
2. Koppel eventueel Google Drive via **Dashboard → Connectors**
3. Noem de klant en de regels

## Wat het kost

| Actie | Credits |
|---|---|
| Factuur aanmaken | 20 |
| Opslaan in Drive | 5 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Geen boekhoudkoppeling.** De factuur belandt niet in je boekhoudpakket; dat doe je zelf of via de Facturatie-skill met Moneybird.
- **Hij verstuurt niets.** Mailen doe je zelf of via [Gmail](gmail.md).
- **Btw-berekening is rekenwerk, geen advies.** Verlegde btw, ICP-leveringen en afwijkende tarieven controleer je zelf.
- **Factuurnummers lopen door op wat je hem geeft.** Hij kent je administratie niet, dus de reeks bewaak jij.
- **Geen betaalstatus.** Of er betaald is, weet hij niet , daarvoor is [Stripe Inzichten](stripe-insights.md) of Moneybird.

## Problemen oplossen

**De regels komen verkeerd binnen.** Gebruik één regel per post met omschrijving, aantal en bedrag. "Website bouw 1x 1500" werkt beter dan een lopende zin.

**Verkeerd btw-percentage.** Noem het expliciet; standaard rekent hij met 21 procent.

**Opslaan in Drive mislukt.** Google Drive is niet gekoppeld of de rechten zijn ingetrokken. Verbind opnieuw via Connectors.

**Het factuurnummer springt.** Zeg welk nummer de vorige had, dan telt hij verder.

## Veelgestelde vragen

**Wat is het verschil met de Facturatie-skill?**
Facturatie werkt met Moneybird: de conceptfactuur komt in je
echte boekhouding te staan. De Factuur Automator maakt een los document.

**Kan hij de factuur mailen?**
Niet uit zichzelf. Met [Gmail](gmail.md) gekoppeld wel, en dan vraagt hij eerst
om bevestiging.

**Kan ik mijn eigen huisstijl gebruiken?**
Bedrijfsgegevens en betaaltermijn wel. Voor een echt vormgegeven factuur is een
boekhoudpakket geschikter.

**Herkent hij herhaalfacturen?**
Als je het vraagt. Zet een maandelijkse factuur als
[geplande taak](../handleiding/geplande-taken.md).

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Stripe Inzichten](stripe-insights.md) · [Google Drive](google-drive.md) · [Weekrapport](weekly-report.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Factuur Automator, bijgewerkt augustus 2026*
