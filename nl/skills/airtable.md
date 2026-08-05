# Airtable

Met de Airtable-skill leest GENI je bases uit, haalt hij records op en maakt of werkt hij ze bij, zodat je bijhouden vanuit de chat kunt doen.

Beschikbaar vanaf **Growth**. Je hebt een gekoppeld Airtable-account nodig.

## Wat kan GENI met Airtable?

- **Je bases opsommen** die aan de koppeling beschikbaar zijn
- **Records lezen** uit een tabel
- **Een record aanmaken**
- **Een bestaand record bijwerken**

Waar een spreadsheet ophoudt, begint Airtable: gekoppelde tabellen, statusvelden
en verschillende weergaves op dezelfde data.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Welke leads staan er op "wacht op offerte"?
```

> Uit base **Sales 2026**, tabel *Leads*, 4 records:
>
> | Bedrijf | Sinds | Contactpersoon |
> |---|---|---|
> | Bakkerij De Krent | 12 juli | Sanne |
> | Studio Noord | 24 juli | Mark |
> | Van Dijk BV | 30 juli | Lisa |
> | De Vries | 2 augustus | Peter |
>
> De eerste twee staan er langer dan twee weken in. Zal ik hun status op
> "opvolgen" zetten?

Bij het aanmaken of bijwerken zie je eerst wat er komt te staan:

```
Zet Van Dijk op "offerte verstuurd"
```

> **Van Dijk BV** , status van *wacht op offerte* naar *offerte verstuurd*.
> Zal ik dat doorvoeren?

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een Airtable-account via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Airtable**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Kies de bases waartoe je toegang geeft

## Wat het kost

Airtable-acties zijn lichte handelingen: lezen en schrijven kosten een klein
aantal credits per actie. Het exacte bedrag staat op de knop voordat je start.
Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Aanmaken en bijwerken vragen om bevestiging.**
- **GENI verwijdert nooit records, tabellen of bases.**
- **Alleen de bases waartoe je toegang gaf.** Wat je niet deelde, blijft onzichtbaar.
- **Geen tabellen of velden aanmaken.** De structuur maak je in Airtable.
- **Formules, koppelingen en weergaves worden gelezen als waarde**, niet aangepast.
- **Bij grote tabellen wordt een deel gelezen.** Noem een weergave of filter als je een specifieke set wilt.

## Problemen oplossen

**Een base wordt niet gevonden.** Die is niet gedeeld bij het koppelen. Verbreek de koppeling en geef er alsnog toegang toe.

**Het verkeerde record wordt bijgewerkt.** Noem het record zo specifiek mogelijk, bijvoorbeeld met een uniek veld in plaats van de bedrijfsnaam.

**Een veld wordt niet gevuld.** Controleer het veldtype; een keuzeveld accepteert alleen bestaande opties, en een gekoppeld veld verwijst naar een ander record.

**Je ziet minder records dan verwacht.** Bij grote tabellen wordt een deel opgehaald. Filter op status of periode.

## Veelgestelde vragen

**Wat is het verschil met Google Sheets?**
[Sheets](google-sheets.md) is een spreadsheet: rijen en kolommen. Airtable is een
lichte database met veldtypes en relaties. Voor eenvoudige lijsten volstaat
Sheets; voor een pipeline met statussen werkt Airtable prettiger.

**Kan ik dit inplannen?**
Ja, bijvoorbeeld wekelijks een overzicht van records die te lang op dezelfde
status staan. Zie [Geplande taken](../handleiding/geplande-taken.md).

**Kan hij bijlagen in een record lezen?**
Nee, hij leest de velden. Voor documenten gebruik je de
[kennisbank](../functies/kennisbank.md).

**Werkt dit met een gratis Airtable-account?**
Ja, binnen de limieten die Airtable zelf stelt.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Sheets](google-sheets.md) · [Typeform](typeform.md) · [HubSpot CRM](hubspot.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Airtable, bijgewerkt augustus 2026*
