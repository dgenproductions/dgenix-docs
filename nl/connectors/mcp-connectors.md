# MCP-connectors

MCP-connectors koppelen GENI aan tools die geen eigen dGENIX-koppeling hebben, via het Model Context Protocol: een open standaard waarmee externe diensten hun mogelijkheden aanbieden.

Het praktische gevolg: er hoeft geen dGENIX-koppeling meer gebouwd te worden
voor elke tool afzonderlijk. Biedt een dienst een MCP-server aan, dan kan die
als connector worden aangesloten. Voor jou werkt zo'n connector precies als elke
andere: activeren, je account koppelen, klaar.

## Wat je hiermee kunt

Wat een MCP-connector kan, bepaalt de dienst zelf. In de praktijk komt het neer
op dezelfde soort acties als bij onze eigen koppelingen: iets opzoeken, iets
aanmaken, iets bijwerken. Elke connector toont in het dashboard welke acties hij
meebrengt.

Het punt is niet dat MCP iets kan wat andere koppelingen niet kunnen, maar dat
het **veel sneller gaat** om een tool toe te voegen.

## Activeren

1. Ga naar **Dashboard → Skills** en zoek de connector
2. Klik op **Activeren**; hij verschijnt als gewone skill-schakelaar
3. Volg de stap-voor-stap-instructie die direct na activatie verschijnt
4. Koppel je eigen account via **Dashboard → Connectors**, als de connector dat vraagt
5. Vraag GENI om er iets mee te doen

Elke MCP-connector heeft zijn eigen instructie in het dashboard, net als Gmail
of WhatsApp. Je hoeft niets technisch te doen en geen server op te zetten.

## Manieren van koppelen

| Manier | Hoe het gaat | Vergelijkbaar met |
|---|---|---|
| Inloggen | Je logt in bij de dienst en geeft toestemming | Slack, Notion |
| Sleutel plakken | Je plakt een sleutel uit je eigen account | Stripe, HubSpot |
| Geen koppeling | Activeren volstaat, er is geen account nodig | , |

Welke manier geldt, staat in de instructie van de connector zelf.

## Welke toegang je geeft

Een MCP-connector werkt standaard op **jouw eigen account** bij die dienst. Dat
heeft drie gevolgen die de moeite waard zijn:

- Je houdt zelf zeggenschap over het account en de gegevens erin
- Rekent de dienst zelf kosten, dan lopen die via jouw account en niet via dGENIX
- Verbreken kan altijd, waarna GENI er direct niet meer bij kan

Wat een connector precies mag, bepaalt de dienst bij het koppelen. Log je in bij
de dienst, dan zie je daar het toestemmingsscherm met de rechten die gevraagd
worden , lees dat, want daar staat het echte antwoord. Plak je een sleutel, dan
geldt wat die sleutel mag; maak er een aan met zo min mogelijk rechten.

Wat er ook gevraagd wordt: acties die iets wijzigen of verwijderen vragen bij
dGENIX altijd eerst om jouw bevestiging.

## Controleren of het werkt

Vraag GENI na het koppelen om iets te **lezen**, niet om iets te maken:

```
Wat kun je met [naam van de connector]?
```

> Ik heb toegang tot **[connector]** en kan daar op dit moment 4 acties in
> uitvoeren: zoeken, een item openen, een item aanmaken en een item bijwerken.
> Zal ik iets voor je opzoeken?

Krijg je die opsomming, dan staat de verbinding en weet je meteen welke acties
je hebt. Zegt GENI dat hij er niet bij kan, kijk dan bij
**Dashboard → Connectors** of de connector op **Verbonden** staat.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, zoek de connector en klik op **Verbreken**.
De toegang vervalt onmiddellijk en GENI kan er daarna niets meer mee.

Twee dingen om te weten:

- **De skill blijft geactiveerd.** Wil je hem helemaal weg, zet hem dan ook uit in de marktplaats.
- **Wat de connector eerder heeft gemaakt, blijft staan.** Verbreken haalt niets terug uit de dienst zelf; dat ruim je daar op.

Je kunt de toestemming ook intrekken bij de dienst zelf. Doe je dat, dan stopt
de connector zonder waarschuwing , verbreken in dGENIX houdt het overzicht
schoner.

## Wat het kost

MCP-connectors gebruiken hetzelfde creditsysteem als alle andere skills: een
vaste prijs per actie, zichtbaar vóór uitvoering. Duurdere acties vragen eerst
om bevestiging, dus je komt niet voor verrassingen te staan. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

MCP-connectors vallen onder **Growth** en hoger.

## Grenzen

- Een connector kan alleen wat de dienst zelf via MCP aanbiedt
- Werkt de dienst niet, dan werkt de connector niet; dGENIX kan dat niet omzeilen
- Acties die iets veranderen of verwijderen vragen altijd om bevestiging
- Wij bepalen welke connectors beschikbaar zijn; je kunt er zelf geen toevoegen
- Het aanbod groeit geleidelijk, dus jouw tool zit er misschien nog niet bij

## Problemen oplossen

**De connector staat niet in de marktplaats.** Dan is hij nog niet beschikbaar. Je kunt hem aanvragen via de skill-marktplaats.

**Activeren lukt, maar er gebeurt niets.** Waarschijnlijk vraagt de connector nog om een koppeling. Kijk bij **Dashboard → Connectors** of hij op Verbonden staat.

**Je weet niet welke acties hij ondersteunt.** Open de connector in het dashboard; de instructie noemt precies wat hij kan.

## Veelgestelde vragen

**Wat is MCP eigenlijk?**
Een open standaard waarmee een dienst zijn mogelijkheden op een eenduidige
manier aanbiedt aan AI-assistenten. Doordat het een standaard is, hoeft niet
elke koppeling opnieuw met de hand gebouwd te worden.

**Merk ik verschil met een gewone koppeling?**
Nee. In het dashboard, in de chat en in de creditafrekening werkt het identiek.

**Kan ik mijn eigen MCP-server aansluiten?**
Op dit moment niet. Het aanbod wordt door ons samengesteld, zodat elke connector
een geteste instructie en een vaste creditprijs heeft.

---

→ Terug naar [Connectors](README.md)
→ Verder: [Skills uitgelegd](../handleiding/skills-uitgelegd.md) · [Het creditsysteem](../hoe-het-werkt/credits.md)
→ Op de site: [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, MCP-connectors, bijgewerkt augustus 2026*
