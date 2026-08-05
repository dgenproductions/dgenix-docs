# Notion

Met de Notion-skill zoekt GENI in je workspace, leest pagina's en schrijft er nieuwe bij, zodat je notities vastleggen niet onderbreekt waar je mee bezig was.

Beschikbaar vanaf **Growth**. Je hebt een gekoppelde Notion-workspace nodig; zie
[Notion koppelen](../connectors/notion.md).

## Wat kan GENI met Notion?

- **Zoeken** in de gedeelde pagina's en databases
- **Een pagina lezen**
- **Een pagina aanmaken**, los of in een database
- **Een bestaande pagina bijwerken**

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Zet de uitkomst van dit gesprek in Notion, bij het project De Krent
```

> **Aangemaakt: Overleg De Krent , 5 augustus**
> `notion.so/Overleg-De-Krent-5-augustus-1a2b3c`
>
> Met daarin:
> - Besluit: website plus kassakoppeling, akkoord op de offerte
> - Levering materiaal uiterlijk 15 augustus
> - Contactpersoon Sanne, beslisser is de eigenaar
> - Openstaand: wie levert de teksten aan
>
> Ik heb hem als subpagina onder *Projecten 2026* gezet.

En bij zoeken:

```
Waar staat onze onboarding-checklist?
```

> Gevonden in **Interne processen › Onboarding klanten**, laatst gewijzigd
> 12 juni. De checklist heeft 14 punten; de laatste drie gaan over facturatie.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een Notion-workspace via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Notion**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. **Selecteer de pagina's en databases** die je wilt delen

Die derde stap bepaalt alles. Selecteer je niets, dan is de koppeling actief maar
kan GENI nergens bij.

## Wat het kost

| Actie | Credits |
|---|---|
| Pagina lezen of zoeken | ~30 |
| Pagina bijwerken | ~50 |
| Pagina aanmaken | ~60 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **GENI ziet alleen wat je expliciet deelde**, inclusief de subpagina's daaronder.
- **Pagina's toevoegen kan niet vanuit dGENIX.** Je verbreekt de koppeling en autoriseert opnieuw met een ruimere selectie.
- **Aanmaken en bijwerken vragen om bevestiging.**
- **GENI verwijdert nooit pagina's of database-rijen.**
- **Zeer lange pagina's worden gedeeltelijk gelezen.** Vraag gericht naar een sectie.
- **Complexe blokken blijven buiten beeld**: databases-in-databases, synced blocks en embeds worden niet geïnterpreteerd.

## Problemen oplossen

**Een pagina wordt niet gevonden.** Die is niet gedeeld. Verbreek de koppeling en selecteer hem alsnog.

**Een nieuwe pagina verschijnt op een onverwachte plek.** Zonder aangewezen locatie plaatst Notion hem in de eerste gedeelde pagina. Noem de doelpagina of database.

**Een database wordt niet gezien.** Databases moet je apart aanvinken; de bovenliggende pagina delen is niet genoeg.

**De opmaak valt tegen.** Koppen, alinea's en lijsten komen mee; complexe blokstructuren niet.

## Veelgestelde vragen

**Kan GENI bij mijn hele workspace?**
Nee, en dat is het verschil met de meeste koppelingen. Notion vraagt per pagina
om toestemming.

**Wat is het verschil met de Werkruimte?**
De [Werkruimte](../functies/werkruimte.md) zit in dGENIX en hangt samen met je
taken en tijdlijn. Notion is je eigen systeem, waar je team ook in werkt.

**Kan hij een gesprek als notitie wegschrijven?**
Ja. Dat is de meest gebruikte toepassing: overleg voeren, uitkomst laten
vastleggen.

**Kan ik dit inplannen?**
Ja, bijvoorbeeld wekelijks een statuspagina laten bijwerken. Zie
[Geplande taken](../handleiding/geplande-taken.md).

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Notion koppelen](../connectors/notion.md) · [Werkruimte](../functies/werkruimte.md) · [Airtable](airtable.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Notion, bijgewerkt augustus 2026*
