# Weekrapport Generator

Met de Weekrapport Generator maakt GENI één rapport uit je verspreide gegevens , KPI's uit een spreadsheet, wat er in je inbox speelde , en mailt hij het naar wie het moet lezen.

Beschikbaar vanaf **Growth**. Werkt beter naarmate je meer koppelingen hebt.

## Wat kan GENI hiermee?

- **Een weekrapport genereren** over een periode naar keuze, met KPI's uit een Google Sheet, signalen uit je Gmail, en optioneel direct verstuurd naar een e-mailadres

Eén tool, maar hij verzamelt uit meerdere bronnen. De sheet-URL onthoudt hij na
de eerste keer.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Maak het weekrapport en stuur het naar bart@voorbeeld.nl
```

> **Weekrapport , 29 juli t/m 4 augustus**
>
> **Cijfers**
>
> | KPI | Deze week | Vorige week |
> |---|---|---|
> | Nieuwe leads | 18 | 12 |
> | Offertes verstuurd | 6 | 7 |
> | Omzet | € 8.420 | € 6.100 |
>
> **Wat opviel**
> - De piek in leads komt uit één bron: de vergelijkingspagina die vorige week
>   live ging
> - Zes offertes tegenover 18 leads is aan de lage kant. Twaalf leads hebben nog
>   geen opvolging gehad.
>
> **Uit je inbox**
> - Twee klanten vroegen naar dezelfde functie (exporteren naar Excel)
> - Een leverancier kondigt een prijsverhoging aan per 1 september
>
> **Voor volgende week**
> - De 12 onopgevolgde leads nabellen
> - Reageren op de prijsverhoging vóór eind augustus
>
> Verstuurd naar bart@voorbeeld.nl.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** geen verplicht. [Google Sheets](google-sheets.md) voor KPI's, [Gmail](gmail.md) voor inbox-signalen en verzending

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Weekrapport Generator**
2. Koppel Google Sheets en Gmail via **Dashboard → Connectors**
3. Vraag om een weekrapport en geef eenmalig de sheet-URL

## Wat het kost

| Actie | Credits |
|---|---|
| Weekrapport genereren | 300 |

Dat is inclusief het ophalen en samenvatten van de bronnen. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Zonder bronnen wordt het dun.** Zonder sheet en zonder inbox heeft hij weinig om over te rapporteren.
- **De KPI's komen uit jouw sheet.** Klopt de sheet niet, dan klopt het rapport niet; hij controleert je cijfers niet.
- **Geen grafieken.** Je krijgt tekst en tabellen.
- **Alleen de bronnen die je koppelt.** Cijfers uit je boekhouding of CRM komen er alleen in als je ze in de sheet zet.
- **Verzenden vraagt Gmail.** Zonder koppeling krijg je het rapport in de chat.

## Problemen oplossen

**De KPI's ontbreken.** De sheet-URL is niet doorgegeven of het tabblad heeft geen herkenbare koppen. Zet de KPI's in een tabel met kopregel.

**Het rapport gaat over de verkeerde week.** Noem de periode expliciet; standaard neemt hij de afgelopen 7 dagen.

**Het is niet verstuurd.** Gmail is niet gekoppeld, of het adres ontbrak. Noem het e-mailadres in de opdracht.

**De inhoud is te algemeen.** Zeg wie het leest. Een rapport voor jezelf ziet er anders uit dan een rapport voor een klant of investeerder.

## Veelgestelde vragen

**Kan ik dit wekelijks automatisch krijgen?**
Ja, dat is de bedoeling. Zet het als [geplande taak](../handleiding/geplande-taken.md),
bijvoorbeeld elke vrijdag om 16:00.

**Kan ik meerdere ontvangers instellen?**
Ja, noem de adressen. Voor een klantrapport is
[White Label](white-label.md) mogelijk geschikter.

**Wat is het verschil met een engine-rapport?**
De [engines](../engines/README.md) rapporteren over je vindbaarheid en reputatie.
Dit rapport gaat over jouw bedrijfscijfers.

**Kan hij het rapport bewaren?**
Ja, vraag hem het als notitie in je [Werkruimte](../functies/werkruimte.md) te
zetten.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Sheets](google-sheets.md) · [White Label](white-label.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Weekrapport Generator, bijgewerkt augustus 2026*
