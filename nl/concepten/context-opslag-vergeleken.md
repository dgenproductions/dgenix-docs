# Geheugen, kennisbank, kennisdocument en projecten vergeleken

dGENIX kent vier plekken waar GENI informatie over jou bewaart, en ze lijken op elkaar. Deze pagina zet ze naast elkaar zodat je weet wat waar hoort.

De korte versie: het **kennisdocument** vertelt wie je bent, het **geheugen**
onthoudt wat GENI onderweg leert, de **kennisbank** bevat je documenten, en een
**project** houdt dat allemaal gescheiden per klant of merk.

## De vier in één tabel

| | Kennisdocument | Geheugen | Kennisbank | Projecten |
|---|---|---|---|---|
| **Wat het bevat** | Wie je bent en hoe GENI moet schrijven | Losse feiten, voorkeuren en doelen | Hele bestanden als achtergrondkennis | Een aparte werkruimte met eigen context |
| **Wie vult het** | Jij, tijdens de intake | GENI zelf, plus jij | Jij, door te uploaden | Jij, per klant of merk |
| **Vorm** | Eén tekst | Losse regels, 8 types | PDF's, Word, tekst | Map met eigen instructies |
| **Wanneer gebruikt** | Bij elk gesprek | Wanneer relevant | Wanneer je een vraag stelt die erin staat | Alleen binnen dat project |
| **Waar** | Intake / Instellingen | Dashboard → Geheugen | Dashboard → Kennisbank | Dashboard → Assistent |
| **Beschikbaar vanaf** | Elk plan | Elk plan | Growth | Growth |

## Kennisdocument

Het kennisdocument maak je één keer, tijdens de intake. Het is de basis: je
bedrijf, je rol, je toon, wat je verkoopt en aan wie. GENI leest het bij élk
gesprek, in elk kanaal.

Gebruik het voor dingen die zelden veranderen. "Wij zijn een installatiebedrijf
in Tilburg met acht monteurs" hoort hier. "Bel Jan terug over de offerte" niet.

Je past het aan via **Dashboard → Instellingen**. Doe je de intake opnieuw, dan
wordt het herschreven.

## Geheugen

Het geheugen is de enige van de vier die zichzelf vult. GENI slaat op wat hij
onderweg leert en gebruikt dat later, ook in een ander kanaal. Er zijn acht
soorten:

| Type | Voorbeeld |
|---|---|
| Feit | "Ik werk bij een marketingbureau in Amsterdam" |
| Voorkeur | "Ik wil antwoorden altijd in bullet points" |
| Doel | "Ik wil mijn e-mailresponstijd halveren" |
| Instructie | "Houd antwoorden onder 150 woorden" |
| Contact | "Mijn vaste ontwerper is Lisa" |
| Patroon | "Ik plan altijd op maandag" |
| Situatie | "We zitten in een groeifase, team van 3" |
| Vaardigheden | "Ik ben expert in copywriting, geen developer" |

Je kunt er zelf ook iets in zetten door het simpelweg te zeggen: *"Onthoud dat
mijn btw-nummer NL0012345B01 is."* Alles is in te zien, aan te passen en te
wissen via **Dashboard → Geheugen**.

Zie [Geheugen (Memory AI)](../functies/geheugen.md) voor het volledige verhaal.

## Kennisbank

De kennisbank is voor **bestanden**, niet voor losse feiten. Je uploadt een
productcatalogus, een handleiding, je algemene voorwaarden of een FAQ, en GENI
zoekt daar zelf in wanneer je iets vraagt dat erin staat.

Het verschil met geheugen: geheugen bewaart één zin, de kennisbank bewaart
twintig pagina's. Vraag je "wat is onze levertijd op maatwerk?", dan zoekt GENI
het antwoord op in je geüploade documenten en citeert daaruit.

Zie [Kennisbank](../functies/kennisbank.md).

## Projecten

Een project is een **afgeschermde werkruimte**. Werk je voor meerdere klanten of
merken, dan houdt een project de context per klant apart: eigen instructies,
eigen gesprekken, eigen herinneringen.

Dat is precies waarom bureaus dit gebruiken. In het project van klant A weet
GENI niets van klant B, dus hij haalt nooit per ongeluk de tone of voice of de
cijfers van de één door de ander.

Zie [Projecten](../functies/projecten.md).

## Wat je ziet

Stel, je bent installateur en je hebt alle vier gevuld. Je vraagt:

```
Schrijf een offerte voor mevrouw De Vries voor een warmtepomp
```

GENI combineert dan:

- uit het **kennisdocument**: dat je een installatiebedrijf bent en formeel schrijft
- uit het **geheugen**: dat je offertes altijd 30 dagen geldig laat zijn
- uit de **kennisbank**: de prijzen en specificaties uit je productcatalogus
- uit het **project**: dat dit klant "De Vries" is, met de eerdere correspondentie

Je krijgt één offerte terug, niet vier losse antwoorden. Zo horen ze samen te werken.

## Welke gebruik je waarvoor?

- Verandert het bijna nooit en geldt het altijd? → **kennisdocument**
- Is het één feit of voorkeur? → **geheugen**
- Staat het in een bestand? → **kennisbank**
- Moet het gescheiden blijven van ander werk? → **project**

## Grenzen

- Het geheugen is **strikt per gebruiker**. Niemand anders kan erbij, ook niet
  binnen hetzelfde bedrijf.
- Kennisbank en projecten zitten in **Growth** en hoger; kennisdocument en
  geheugen zitten in elk plan.
- GENI verzint niets bij. Staat het antwoord niet in je kennisbank, dan zegt hij
  dat, in plaats van te gokken.
- Een project deelt géén herinneringen met je algemene chat. Dat is opzet, maar
  betekent wel dat je iets soms twee keer vertelt.

## Veelgestelde vragen

**Moet ik alle vier gebruiken?**
Nee. Kennisdocument en geheugen krijg je automatisch. Kennisbank en projecten
zet je pas in als je documenten hebt of voor meerdere klanten werkt.

**Wat als geheugen en kennisdocument elkaar tegenspreken?**
Het geheugen is specifieker en recenter, dus dat weegt zwaarder. Klopt iets
structureel niet, pas dan je kennisdocument aan in plaats van het geheugen te
blijven corrigeren.

**Wordt mijn data gebruikt om AI te trainen?**
Nee. Je gegevens blijven van jou en worden niet gebruikt om modellen te trainen.

**Kan ik alles wissen?**
Ja. Het geheugen leeg je per regel of in één keer via **Dashboard → Geheugen**;
kennisbank-bestanden verwijder je stuk voor stuk.

---

→ Verder: [Wat is dGENIX](wat-is-dgenix.md) · [Hoe alles samenwerkt](hoe-alles-samenwerkt.md)
→ Diepgang: [Geheugen](../functies/geheugen.md) · [Kennisbank](../functies/kennisbank.md) · [Projecten](../functies/projecten.md)
→ Op de site: [hoe dGENIX werkt](https://dgenix.nl/hoe-het-werkt) · [voor bureaus](https://dgenix.nl/agencies)

*dGENIX Docs, Contextopslag vergeleken, bijgewerkt augustus 2026*
