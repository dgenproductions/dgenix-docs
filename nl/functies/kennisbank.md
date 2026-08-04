# Kennisbank

De kennisbank is de plek waar je hele bestanden neerlegt die GENI als achtergrondkennis gebruikt: je productcatalogus, je voorwaarden, je handleiding.

Zo hoef je nooit meer uit te leggen wat je verkoopt of hoe jullie werken. Vraag
je iets dat in een geüpload document staat, dan zoekt GENI het antwoord daar op
en citeert eruit. Beschikbaar vanaf **Growth**.

## Wat je hiermee kunt

| Wat je uploadt | Wat GENI ermee doet |
|---|---|
| Productcatalogus of prijslijst | Offertes en antwoorden met de juiste prijzen |
| Algemene voorwaarden | Vragen over levertijd, garantie en betaling beantwoorden |
| Handleiding of FAQ | Support-antwoorden onderbouwen met je eigen tekst |
| Bedrijfsprofiel | Teksten schrijven die kloppen met wat jullie doen |
| Klantbriefing | Werken binnen de afspraken van dat project |

## Kennisbank, geheugen of kennisdocument?

Deze drie lijken op elkaar en dat is de meest voorkomende verwarring:

- **Geheugen** bewaart één zin ("mijn btw-nummer is NL0012345B01")
- **Kennisdocument** beschrijft wie je bent en hoe GENI schrijft
- **Kennisbank** bewaart twintig pagina's, en GENI zoekt erin wanneer nodig

Zie [Contextopslag vergeleken](../concepten/context-opslag-vergeleken.md) voor
de volledige vergelijking.

## Hoe het werkt

1. Ga naar **Dashboard → Assistent → Kennisbank**
2. Klik op **Bestand uploaden**
3. Kies een PDF, Word-bestand, tekstbestand of markdown-bestand
4. Het bestand wordt verwerkt, meestal binnen een minuut
5. GENI raadpleegt het vanaf dat moment bij relevante vragen

| Type | Extensie |
|---|---|
| PDF | `.pdf` |
| Word | `.docx` |
| Tekst | `.txt` |
| Markdown | `.md` |

## Wat je ziet

Je uploadt je prijslijst en vraagt daarna:

```
Wat is onze levertijd op maatwerk?
```

> Op maatwerk staat een levertijd van **4 tot 6 weken**, gerekend vanaf
> akkoord op de offerte. Bij spoed geldt een toeslag van 15 procent en gaat de
> levertijd naar 2 weken.
>
> *Bron: Algemene voorwaarden 2026.pdf*

Zonder kennisbank had GENI hier moeten vragen wat jullie levertijd is. Nu
haalt hij het antwoord uit je eigen document en zegt hij erbij waar het vandaan
komt.

## Per project of voor je hele account

Je kunt bestanden op twee niveaus uploaden:

- **Op accountniveau**, dan geldt het voor al je gesprekken
- **Binnen een project**, dan gebruikt GENI het alleen daar

Dat tweede is waarom bureaus hiermee werken: de catalogus van klant A komt nooit
in het werk voor klant B terecht. Zie [Projecten](projecten.md).

## Grenzen

- **GENI verzint niets bij.** Staat het antwoord niet in je bestanden, dan zegt hij dat in plaats van te gokken.
- **Alleen tekst wordt gelezen.** Afbeeldingen en diagrammen in een PDF worden niet geïnterpreteerd.
- **Een gescande PDF zonder tekstlaag levert niets op**, want er valt geen tekst uit te halen.
- **Bijwerken gaat via opnieuw uploaden.** Een gewijzigd bestand vervang je; GENI merkt een wijziging niet zelf op.
- **Bestanden worden niet gedeeld.** Je kennisbank is van jou, ook binnen hetzelfde bedrijf.
- **Kennisbank zit vanaf Growth.** Op Free en Starter gebruik je geheugen en het kennisdocument.

## Problemen oplossen

**GENI gebruikt het bestand niet.** Stel je vraag concreter. Hij zoekt op inhoud, dus "wat is onze levertijd" werkt beter dan "vertel eens over ons bedrijf".

**Het antwoord komt uit het verkeerde bestand.** Staat dezelfde informatie in twee documenten, verwijder dan de verouderde versie.

**De verwerking lukt niet.** Waarschijnlijk een gescande PDF zonder tekstlaag. Haal het bestand door een OCR-tool of upload de brontekst.

**Je ziet de kennisbank niet.** Die zit vanaf Growth; op een lager plan is de sectie niet zichtbaar.

**Een oud antwoord blijft terugkomen.** Verwijder het oude bestand echt; alleen een nieuwe versie uploaden laat de oude staan.

## Bestanden verwijderen

Ga naar **Dashboard → Assistent → Kennisbank**, klik het bestand aan en kies
**Verwijderen**. Het is direct weg en GENI kan er daarna niet meer bij.

## Veelgestelde vragen

**Hoeveel bestanden kan ik uploaden?**
Genoeg voor normaal gebruik. Kwaliteit telt zwaarder dan aantal: vijf goede,
actuele documenten werken beter dan dertig overlappende versies.

**Wordt mijn data gebruikt om AI te trainen?**
Nee. Je bestanden blijven van jou en worden niet gebruikt om modellen te
trainen.

**Kost het credits?**
Uploaden en doorzoeken zitten in je plan. Alleen het gesprek zelf verbruikt
credits, zoals elk bericht.

**Kan ik zien welk bestand een antwoord opleverde?**
Ja, GENI noemt de bron waaruit hij citeert.

**Wat is het verschil met een bestand meesturen in de chat?**
Een bijlage geldt voor dat ene gesprek. De kennisbank is blijvend, en GENI
doorzoekt hem uit zichzelf. Zie [Bestanden](bestanden.md).

---

→ Verder: [Contextopslag vergeleken](../concepten/context-opslag-vergeleken.md) · [Projecten](projecten.md) · [Geheugen](geheugen.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, Kennisbank, bijgewerkt augustus 2026*
