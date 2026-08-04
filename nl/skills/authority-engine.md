# Authority Engine

De [Authority Engine](https://dgenix.nl/engines/authority) is de stap van *meten* naar *doen*: GENI schrijft artikelen die op autoriteit zijn gebouwd en zet ze klaar in je CMS, maar nooit zonder jouw goedkeuring.

De andere engines vertellen je wat er mis is. Deze schrijft de content die het
oplost. Beschikbaar vanaf **Pro**.

## Wat de Authority Engine doet

| Onderdeel | Wat het oplevert |
|---|---|
| **Topical map** | Een contentplan: één pillar-artikel plus clusterartikelen rond je hoofdonderwerp |
| **Conceptartikel** | Een origineel, op E-E-A-T gericht artikel, klaar om te beoordelen |
| **Content-score** | Een cijfer voor je concept, afgezet tegen wat er nu bovenaan Google staat |
| **Publiceren** | Naar je CMS als concept, of live, altijd als bewuste keuze |

De volgorde is bewust: eerst een plan, dan de artikelen, dan terugmeten. Losse
artikelen schrijven zonder plan levert stukken op die om dezelfde zoekwoorden
concurreren.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

Je vraagt om een topical map over "warmtepompen". Je krijgt geen artikelen maar
een **plan**:

> **Pillar:** Warmtepompen, de complete gids voor woningeigenaren
>
> **Clusters:**
> - Wat kost een warmtepomp?
> - Warmtepomp of cv-ketel, wat is voordeliger?
> - Welke subsidie krijg je op een warmtepomp?
> - Is mijn huis geschikt voor een warmtepomp?
>
> Per titel: **Schrijf artikel** →

Elke titel staat er met het maandelijkse zoekvolume erbij en is een knop. Klik
erop en GENI schrijft dat ene artikel, met een interne link naar de pillar. Zo
bouw je een samenhangend cluster in plaats van losse stukken.

Bij een conceptartikel krijg je de volledige tekst in de wachtrij, met daarnaast
**Naar CMS als concept**, **Publiceer live**, **Bewerken** en **Verwerp**.

## Hoe het werkt

1. **Koppel je CMS.** WordPress (Application Password) of Webflow (API-sleutel en collection-ID), plus zes andere systemen. Zonder koppeling werkt alles behalve publiceren.
2. **Bouw een topical map** of geef direct een onderwerp op voor één artikel.
3. **Genereer een concept.** Het blijft in dGENIX staan; er gaat niets naar je site.
4. **Beoordeel in de wachtrij.** Lezen, bewerken, of laten scoren tegen de concurrentie.
5. **Jij beslist**: naar je CMS als concept, live publiceren, of verwerpen.
6. **Rollback.** Een gepubliceerd of doorgestuurd stuk zet je met één klik terug naar concept.

## Content-score, terugmeten tegen de SERP

Een concept beoordelen op gevoel is lastig. De **content-score** haalt daarom de
pagina's op die nú bovenaan staan voor jouw zoekwoord en vergelijkt jouw stuk
daarmee:

- een **dekkingsscore** van 0 tot 100
- **gemiste onderwerpen** die de concurrentie wel behandelt
- concrete **toevoegingen** om het stuk completer te maken
- een **lengte-benchmark** tegen de huidige top-pagina's

Daarmee is de cirkel rond: meten, schrijven, terugmeten.

## Via GENI en op de automaat

De Authority Engine is ook gewoon een skill van GENI. Je kunt hem in de chat
vragen ("schrijf een concept over X", "bouw een topical map over Y") en, nuttiger,
**inplannen**. Zet een herhaalde taak op, bijvoorbeeld elke maandag een nieuw
concept, en de stukken landen vanzelf in je wachtrij. Publiceren blijft altijd
jouw handeling.

Zie [Geplande taken](../handleiding/geplande-taken.md).

## Veilig by design

Google treedt op tegen ongecontroleerd gepubliceerde massa-AI-content. Daarom
zit die rem hier ingebouwd:

- **Draft-first.** GENI raakt je site nooit aan zonder dat jij publiceert.
- **Verplichte goedkeuring.** Elke publicatie is een aparte, bewuste handeling.
- **Volume-limiet.** Maximaal 30 concepten per maand, gerekend vanaf je factuurdatum.
- **Activiteitenlog.** Elke schrijf- en publicatieactie wordt vastgelegd.
- **Intrekbare koppeling.** Credentials staan versleuteld en zijn op elk moment in te trekken.

## Wat het kost

| Actie | Credits |
|---|---|
| Topical map | 2.000 |
| Conceptartikel | 3.000 |
| Content-score | 2.500 |
| Naar CMS sturen of publiceren | gratis |

Mislukt een actie, dan krijg je de credits terug. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen

- **Maximaal 30 concepten per maand.** Bewust, om kwaliteit boven volume te houden.
- **GENI publiceert nooit uit zichzelf**, ook niet binnen een herhaalde taak.
- **Alleen tekst.** Afbeeldingen bij een artikel voeg je zelf toe in je CMS.
- **Geen bestaande pagina's herschrijven**; de engine maakt nieuwe stukken.
- **Je blijft verantwoordelijk voor de inhoud.** GENI schrijft goed onderbouwde tekst, maar feiten over jouw bedrijf, prijzen en beloftes controleer je zelf.
- **Framer wordt nog niet ondersteund**, zolang hun schrijf-API niet volwassen is.

## Problemen oplossen

**Publiceren geeft een foutmelding.** Meestal is de CMS-koppeling verlopen of mist er een recht. Controleer de koppeling in het Authority-dashboard.

**Je zit aan de maandlimiet.** De teller loopt vanaf je factuurdatum, niet vanaf de eerste van de maand. In het dashboard zie je hoeveel je nog hebt.

**Het artikel gaat naar de verkeerde plek in je CMS.** Bij WordPress landt het in de standaard-categorie, bij Webflow in de opgegeven collection. Stel dat in bij de koppeling.

**Het concept klopt inhoudelijk niet.** Bewerk het in de wachtrij vóór je goedkeurt. Dat is precies waarvoor die stap er is.

**Je ziet geen zoekvolumes in de topical map.** De cijfers komen uit een externe bron; valt die weg, dan krijg je alsnog een plan, alleen zonder volumes.

## Veelgestelde vragen

**Merkt Google dat dit AI-content is?**
Google straft niet AI-gebruik af, maar ongecontroleerde massaproductie zonder
redactie. Daarom dwingt deze engine goedkeuring per stuk af en zit er een
maandlimiet op. Lees wat je publiceert en vul aan waar je eigen ervaring
toevoegt; dat is precies het verschil dat E-E-A-T beoordeelt.

**Welke CMS'en worden ondersteund?**
WordPress, WooCommerce, Webflow, Shopify, HubSpot, Wix, Storyblok en Magento.

**Kan ik het zonder CMS gebruiken?**
Ja. Zonder koppeling schrijft GENI gewoon concepten die je kopieert; alleen de
publiceerknop is dan niet bruikbaar.

**Wat is het verschil met de SEO Blog Schrijver?**
Die schrijft één artikel op verzoek. De Authority Engine denkt in clusters,
meet terug tegen de SERP en publiceert met goedkeuring.

**Werkt dit ook voor klanten van mijn bureau?**
Ja. Zet per klant een project op, dan blijft de context gescheiden. Zie
[Projecten](../functies/projecten.md).

---

→ Verder: [SEO Engine](seo-engine.md) · [GEO Engine](geo-engine.md) · [Alle Groei Tools](../engines/README.md)
→ Op de site: [Authority Engine](https://dgenix.nl/engines/authority) · [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, Authority Engine, bijgewerkt augustus 2026*
