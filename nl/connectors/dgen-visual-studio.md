# dGEN Visual Studio koppelen

Met deze koppeling werkt GENI in jouw eigen dGEN Visual Studio: hij maakt daar beeld en video, en hij draait de flows die jij op het canvas hebt gebouwd.

Het verschil met de beeldskills die dGENIX zelf meebrengt zit in het woord *jouw*. Het werk gebeurt in je eigen studio-account, met je eigen modellen en je eigen LoRA-s, en het resultaat komt in je eigen bibliotheek te staan.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Maak een campagnebeeld in mijn studio" | Genereert het beeld daar en laat het zien |
| "Welke flows heb ik klaarstaan?" | Geeft je opgeslagen flows met hun stappen |
| "Draai de flow voor de weekbanner" | Start die flow van begin tot eind |
| "Welke modellen kan ik gebruiken?" | Geeft de catalogus met wat elk model aankan |
| "Wat staat er in mijn bibliotheek?" | Geeft je laatste bestanden met een link |
| "Hoeveel credits heb ik daar nog?" | Leest je studiosaldo |

De flow is waar dit interessant wordt. Bouw hem één keer op het canvas, zet hem daarna in een [geplande taak](../handleiding/geplande-taken.md), en je terugkerende beeldwerk gebeurt zonder dat je de studio nog opent.

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast dGEN Visual Studio
3. Log in bij de studio; je krijgt daar een toestemmingsscherm met de rechten die gevraagd worden
4. Klik op **Allow**. De [dGEN Visual Studio-skill](../skills/dgen-visual-studio.md) is direct actief

De koppeling valt onder **Growth** en hoger. Heb je nog geen studio-account, maak dat dan eerst aan op dgenvisual.com.

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

- **Beeld duurt seconden, video duurt minuten.** Bij video krijg je eerst een bevestiging dat het loopt; het resultaat komt in je bibliotheek te staan
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

---

→ Terug naar [Connectors](README.md)
→ Verder: [dGEN Visual Studio-skill](../skills/dgen-visual-studio.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, dGEN Visual Studio, bijgewerkt augustus 2026*
