# Google Drive

Met de Google Drive-skill zoekt GENI bestanden in je Drive, leest hun inhoud en ordent je mappen, zodat je niet zelf hoeft te graven.

Beschikbaar vanaf **Starter**. Je hebt een gekoppeld Google-account nodig; zie
[Google Drive koppelen](../connectors/google-drive.md).

## Wat kan GENI met Google Drive?

- **Bestanden zoeken** op naam, type of inhoud
- **De tekst van een document lezen**, zodat hij het kan samenvatten of eruit citeren
- **Een map aanmaken** in je Drive-structuur
- **Een bestand verplaatsen of hernoemen**
- **Deelrechten instellen** per persoon: lezen, reageren of bewerken

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Zoek de offerte voor De Vries en vat hem samen
```

> Gevonden: **Offerte De Vries , warmtepomp.docx**, laatst gewijzigd 2 augustus.
>
> - Warmtepomp inclusief installatie: **€ 8.450** exclusief btw
> - Levertijd 4 tot 6 weken na akkoord
> - Offerte geldig tot **1 september**
> - Onderhoudscontract optioneel, € 240 per jaar
>
> De offerte verloopt over vier weken. Zal ik een herinnering zetten?

## Vereisten

- **Plan:** Starter en hoger
- **Koppeling:** een Google-account via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Google Drive**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Doorloop het Google-toestemmingsscherm
4. Drive is direct bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| Bestand zoeken | ~20 |
| Document lezen en samenvatten | ~40 |
| Map aanmaken | ~15 |
| Bestand verplaatsen of hernoemen | ~15 |
| Deelrechten instellen | ~20 |

De skill zit in je plan; je betaalt per actie. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **GENI verwijdert nooit een bestand of map.**
- **Hij leest tekst, geen opmaak.** Afbeeldingen, grafieken en complexe opmaak in een document worden niet geïnterpreteerd.
- **Een gescande PDF zonder tekstlaag levert niets op.**
- **Verplaatsen, hernoemen en delen vragen om bevestiging**, want ze veranderen iets voor anderen.
- **Hij bewerkt de inhoud van een document niet.** Voor schrijven in Google Docs gebruik je [Google Docs](google-docs.md).
- **Alleen het gekoppelde account.** Gedeelde Drives van anderen zijn alleen zichtbaar als jij er toegang toe hebt.

## Problemen oplossen

**Een bestand wordt niet gevonden.** Zoek op een deel van de bestandsnaam. Staat het in een gedeelde Drive waar je geen toegang toe hebt, dan ziet GENI het ook niet.

**Hij kan de inhoud niet lezen.** Bij een gescande PDF of een bestand in een formaat dat geen tekstlaag heeft, valt er niets uit te halen.

**Deelrechten instellen mislukt.** Je hebt zelf geen rechten om dat bestand te delen, of de organisatie beperkt extern delen.

**Hij vindt een oude versie.** Drive bewaart versies; GENI leest de huidige. Controleer of je de juiste kopie zoekt.

## Veelgestelde vragen

**Kan GENI bestanden uploaden?**
Bestanden die jij in de chat meestuurt komen in je Werkruimte terecht. Zie
[Bestanden](../functies/bestanden.md).

**Wat is het verschil met de kennisbank?**
Drive is jouw opslag, waarin GENI zoekt als je erom vraagt. De
[kennisbank](../functies/kennisbank.md) is een vaste set documenten die hij uit
zichzelf raadpleegt.

**Kan hij mappen opruimen?**
Hij kan verplaatsen en hernoemen, niet verwijderen. Opruimen blijft jouw keuze.

**Ziet dGENIX al mijn bestanden?**
Alleen wat nodig is voor je vraag, op het moment dat je hem stelt.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Drive koppelen](../connectors/google-drive.md) · [Google Docs](google-docs.md) · [Kennisbank](../functies/kennisbank.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Google Drive, bijgewerkt augustus 2026*
