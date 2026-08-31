# dGEN Visual Studio koppelen

dGEN Visual Studio is een AI-studio voor beeld en video. Je werkt er met de bekende beeldmodellen, je legt er je eigen stijl vast, en terugkerend beeldwerk bouw je er als flow op een canvas. Met deze koppeling doet GENI dat werk daar voor je: beeld en video maken, en de flows draaien die jij hebt gebouwd.

Het verschil met de beeldskills die dGENIX zelf meebrengt zit in het woord *jouw*. Het werk gebeurt op je eigen studio-account, met je eigen modellen en je eigen stijlmodellen, en het resultaat komt in je eigen bibliotheek.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Maak een campagnebeeld in mijn studio" | Genereert het beeld daar en laat het zien |
| "Welke flows heb ik klaarstaan?" | Geeft je opgeslagen flows met hun stappen |
| "Draai de flow voor de weekbanner" | Start die flow van begin tot eind |
| "Welke modellen kan ik gebruiken?" | Geeft de catalogus met wat elk model aankan |
| "Wat staat er in mijn bibliotheek?" | Geeft je laatste bestanden met een link |
| "Pak dat beeld en zet het in een post" | Haalt het bestand op en gebruikt het in de volgende stap |
| "Hoeveel credits heb ik daar nog?" | Leest je studiosaldo |

Waar het echt interessant wordt, is dat een resultaat **bruikbaar blijft**. Alles wat GENI in je studio maakt, wordt ook opgeslagen in je dGENIX-bestanden. Daardoor kan een volgende stap ermee verder: een artikel plus het beeld als concept naar je CMS, een social post met het nieuwe beeld eronder, of een mail met de hele set eraan.

De flow is waar dit interessant wordt. Bouw hem één keer op het canvas, zet hem daarna in een [geplande taak](../handleiding/geplande-taken.md), en je terugkerende beeldwerk gebeurt zonder dat je de studio nog opent.

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast dGEN Visual Studio
3. Log in bij de studio; je krijgt daar een toestemmingsscherm met de rechten die gevraagd worden
4. Klik op **Allow**. De [dGEN Visual Studio-skill](../skills/dgen-visual-studio.md) is direct actief

De koppeling valt onder **Growth** en hoger. Heb je nog geen studio-account, maak dat dan eerst aan op [dgenvisual.com](https://dgenvisual.com).

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| Flows bekijken | De lijst met jouw flows en de modellencatalogus ophalen |
| Een flow draaien | Een opgeslagen flow van begin tot eind uitvoeren |
| Bestanden bekijken | Je bibliotheek doorzoeken en een tijdelijke link ophalen |
| LoRA-s bekijken | Zien welke eigen stijlmodellen je hebt |
| Beeld maken | Een afbeelding genereren (kost studio-credits) |
| Video maken | Een video genereren (kost studio-credits) |
| Saldo bekijken | Lezen hoeveel credits je daar nog hebt |

Wijzigen of verwijderen zit er niet bij: GENI kan je flows niet aanpassen en niets uit je bibliotheek weghalen.

## Combineren met andere skills

Dit is waar de koppeling voor bedoeld is: niet één plaatje, maar een schakel in werk dat al liep.

| Keten | Wat er gebeurt |
|---|---|
| Kennisbank → SEO Blog Schrijver → dGEN Visual Studio → CMS Publisher | Een artikel uit je eigen kennis, met een beeld in jouw stijl, als concept in je CMS |
| Geplande taak → dGEN Visual Studio → Social Media Manager | Elke maandag verse beelden met de posts er ingepland bij |
| Google Bedrijfsprofiel → dGEN Visual Studio → LinkedIn | Een goede review wordt een beeldcitaat dat klaarstaat om te delen |
| Google Sheets → dGEN Visual Studio → Google Drive | Elke rij zonder beeld krijgt er een, opgeslagen in de juiste map |

Je hoeft daar niets voor in te stellen. Vraag het in één zin, of zet die zin in een [geplande taak](../handleiding/geplande-taken.md).

⚠️ **Wil je een bestaand bestand uit je studio gebruiken, vraag GENI dan het op te halen.** De link die de bibliotheek toont is tijdelijk en werkt na ongeveer een uur niet meer; een opgehaald bestand staat in je dGENIX-bestanden en blijft werken.

## Wat het kost

Dit is het punt waar de meeste verwarring ontstaat, dus expliciet: **de generatie wordt in de studio afgerekend, op je saldo dáár.** dGENIX rekent alleen de handeling, 5 credits voor iets opvragen en 25 voor iets laten maken. Wat het beeld zelf kost, staat in de studio bij het model.

Alles wat iets maakt vraagt daarom eerst om je bevestiging, met het bedrag erbij. Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Controleren of het werkt

Vraag na het koppelen om iets te **lezen**, niet om iets te maken:

```
Hoeveel credits heb ik nog in mijn Visual Studio?
```

Krijg je een saldo terug, dan staat de verbinding. Vraag daarna gerust welke flows er klaarstaan.

## Grenzen

- **Beeld duurt seconden, video duurt minuten.** Bij video krijg je eerst een bevestiging dat het loopt; het resultaat komt daarna in je studiobibliotheek én in je dGENIX-bestanden
- **GENI bouwt geen flows.** Hij draait wat jij hebt gemaakt; het canvas blijft jouw werk
- **Een model dat je aansluiting niet kan lezen, weigert de studio** , vraag eerst welke modellen er zijn in plaats van een naam te noemen
- **Geen studio-credits, geen beeld.** dGENIX kan daar niet bijkopen
- **De studio bepaalt het aanbod.** Verandert de modellencatalogus daar, dan verandert hij hier mee

## Problemen oplossen

**GENI zegt dat je niet gekoppeld bent.** Kijk bij **Dashboard → Connectors** of de connector op Verbonden staat. Is de toestemming in de studio ingetrokken, dan stopt de koppeling zonder waarschuwing.

**"De studio kon dit niet uitvoeren."** Dat is een melding van de studio zelf, meestal over een model dat de meegestuurde invoer niet aanneemt. Vraag welke modellen beschikbaar zijn en welke invoer ze verwachten.

**Er komt een id terug in plaats van een beeld.** Dan loopt de generatie nog. Vraag er later naar met dat id, of kijk in je studiobibliotheek.

**Het beeld klopt, maar de stijl niet.** Noem je LoRA of gebruik een flow; los gevraagd beeld valt terug op het standaardmodel van de studio.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, zoek dGEN Visual Studio en klik op **Verbreken**. De toegang vervalt onmiddellijk.

Twee dingen om te weten:

- **De skill blijft geactiveerd.** Wil je hem helemaal weg, zet hem dan ook uit in de marktplaats
- **Wat er gemaakt is, blijft staan.** Verbreken haalt niets uit je studiobibliotheek

Je kunt de toestemming ook in de studio zelf intrekken, onder **Connected apps**. Daar staat ook het dagplafond per koppeling.

## Veelgestelde vragen

**Waarom niet gewoon de beeldskills van dGENIX?**
Die zijn sneller voor los beeld. Deze koppeling is er voor werk dat in jouw studio hoort: eigen modellen, eigen LoRA-s, één bibliotheek, en flows die je zelf hebt gebouwd.

**Betaal ik nu twee keer?**
Nee. De studio rekent de generatie, dGENIX rekent de handeling. Het bedrag van de studio is hetzelfde als wanneer je daar zelf op Run drukt.

**Kan GENI dit ook op een schema doen?**
Ja, dat is de belangrijkste reden dat deze koppeling bestaat. Zie [Geplande taken](../handleiding/geplande-taken.md).

**Kan GENI mijn flows aanpassen?**
Nee. Hij mag ze lezen en draaien, meer niet.

**Waar komt het resultaat terecht?**
Op twee plekken: in je studiobibliotheek, net als werk dat je zelf op het canvas maakt, én in je dGENIX-bestanden. Dat tweede is nodig om het in een volgende stap te kunnen gebruiken.

---

→ Terug naar [Connectors](README.md)
→ Verder: [dGEN Visual Studio-skill](../skills/dgen-visual-studio.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle koppelingen](https://dgenix.nl/integrations)
→ Over het product zelf: [dGEN Visual Studio](https://dgenvisual.com)

*dGENIX Docs, dGEN Visual Studio, bijgewerkt augustus 2026*
