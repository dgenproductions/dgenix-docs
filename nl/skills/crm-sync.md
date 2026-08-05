# CRM Sync

Met de CRM Sync-skill haalt GENI contacten op uit je CRM, werkt hij dealstatussen bij en maakt hij een overzichtsrapport, zodat je systemen niet uit elkaar lopen.

Beschikbaar vanaf **Pro**.

## Wat kan GENI hiermee?

- **Contacten ophalen** uit je gekoppelde CRM
- **Een dealstatus bijwerken**
- **Een sync-rapport genereren** met wat er niet gelijk staat

Het derde is waar de skill zijn naam aan dankt. Als je met meerdere systemen
werkt, lopen ze uit elkaar zonder dat iemand dat merkt: een deal die in het ene
systeem gewonnen is en in het andere nog openstaat.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Maak een sync-rapport
```

> **12 contacten gecontroleerd, 3 verschillen gevonden**
>
> | Contact | Verschil |
> |---|---|
> | De Vries | Deal staat op "gewonnen" in CRM, op "offerte" in je werkruimte |
> | Studio Noord | Telefoonnummer verschilt tussen beide systemen |
> | Van Dijk BV | Staat alleen in je werkruimte, niet in het CRM |
>
> De eerste is de belangrijkste: die deal is drie weken geleden gewonnen en
> telt nu nog mee in je open pipeline.
>
> Zal ik de status in je werkruimte bijwerken?

## Vereisten

- **Plan:** Pro en hoger
- **Koppeling:** een CRM, bijvoorbeeld [HubSpot](hubspot.md)

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **CRM Sync**
2. Koppel je CRM via **Dashboard → Connectors**
3. Vraag om contacten, een statuswijziging of een rapport

## Wat het kost

| Actie | Credits |
|---|---|
| Contacten ophalen | 15 |
| Sync-rapport genereren | 15 |

Dit is een van de goedkoopste skills, juist omdat je hem regelmatig hoort te
draaien. Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Hij synchroniseert niet automatisch.** Je krijgt de verschillen te zien en beslist zelf wat er gebeurt.
- **Bijwerken vraagt om bevestiging.**
- **GENI verwijdert nooit contacten of deals.**
- **Geen tweerichtingsverkeer in één klik.** Verschillen los je per geval op, niet met een knop "maak alles gelijk".
- **Alleen de velden die het CRM beschikbaar stelt.** Aangepaste eigenschappen vallen er vaak buiten.

## Problemen oplossen

**Er worden geen verschillen gevonden.** Dat kan kloppen. Controleer wel of je CRM gekoppeld is en of er contacten in beide systemen staan.

**Een verschil klopt niet.** Twee systemen kunnen bewust verschillen, bijvoorbeeld een intern werkveld dat de klant niet hoort te zien. Zeg welke velden je wilt vergelijken.

**Bijwerken lukt niet.** De schrijfrechten in je CRM-koppeling staan uit. Zie [HubSpot koppelen](../connectors/hubspot.md).

**Er ontbreken contacten.** Hij haalt op wat de koppeling toont; contacten in een andere pipeline of eigenaar vallen er soms buiten.

## Veelgestelde vragen

**Welk CRM wordt ondersteund?**
HubSpot via de eigen koppeling. Andere systemen kunnen via
[MCP-connectors](../connectors/mcp-connectors.md) beschikbaar komen.

**Wat is het verschil met de HubSpot-skill?**
[Die](hubspot.md) werkt rechtstreeks in HubSpot: contacten aanmaken, deals
bijwerken. CRM Sync kijkt naar verschillen tussen systemen.

**Kan ik dit wekelijks laten draaien?**
Ja, en dat is de beste inzet: 15 credits per rapport, dus wekelijks kost je dat
bijna niets. Zie [Geplande taken](../handleiding/geplande-taken.md).

**Past hij dingen aan zonder dat ik het weet?**
Nee. Elke wijziging vraagt om bevestiging.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [HubSpot CRM](hubspot.md) · [Weekrapport](weekly-report.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, CRM Sync, bijgewerkt augustus 2026*
