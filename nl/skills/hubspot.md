# HubSpot CRM

Met de HubSpot-skill houdt GENI je CRM bij vanuit de chat: contacten opzoeken en aanmaken, deals bijwerken, notities toevoegen en je pipeline samenvatten.

Beschikbaar vanaf **Growth**. Je hebt een gekoppeld HubSpot-account nodig; zie
[HubSpot koppelen](../connectors/hubspot.md).

## Wat kan GENI met HubSpot?

- **Een contact opzoeken** op e-mail, naam of bedrijf
- **Een contact aanmaken**
- **Een deal aanmaken of van fase wisselen**
- **Een notitie toevoegen** aan een contact of deal
- **Je pipeline ophalen**, gegroepeerd per fase

Het meeste rendement zit in de kleine handelingen: na een gesprek meteen een
notitie erbij, in plaats van het later alsnog niet doen.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Hoe staat mijn pipeline ervoor?
```

> **14 open deals, samen € 96.400**
>
> | Fase | Deals | Waarde |
> |---|---|---|
> | Eerste contact | 5 | € 18.200 |
> | Offerte verstuurd | 6 | € 52.900 |
> | Onderhandeling | 3 | € 25.300 |
>
> **Wat opvalt:** vier deals in "Offerte verstuurd" staan er langer dan drie
> weken in, samen goed voor € 31.000. De oudste is De Vries, sinds 12 juli.
>
> Zal ik voor die vier een opvolgnotitie klaarzetten?

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een HubSpot Private App Token via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **HubSpot CRM**
2. Maak in HubSpot een private app aan met de benodigde scopes
3. Plak het token bij **Dashboard → Connectors**

De scopes die je aanzet bepalen wat GENI mag. Laat je de schrijfrechten uit, dan
kan hij alleen lezen. Zie [HubSpot koppelen](../connectors/hubspot.md).

## Wat het kost

| Actie | Credits |
|---|---|
| Notitie toevoegen | ~40 |
| Contact aanmaken of zoeken | ~50 |
| Deal bijwerken | ~50 |
| Pipeline-overzicht | ~70 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Aanmaken en bijwerken vragen om bevestiging.**
- **GENI verwijdert nooit** contacten, deals of notities.
- **Alleen contacten, deals en notities.** Tickets, producten en offertes vallen erbuiten.
- **Aangepaste eigenschappen worden niet automatisch gevuld.**
- **Zonder de juiste scope kan hij het niet**, ook niet als je het vraagt. Dat is opzet.
- **E-mail versturen loopt niet via HubSpot** maar via je e-mailkoppeling.

## Problemen oplossen

**Rechtenfout bij een actie.** De bijbehorende scope staat uit in je private app. Vink hem aan in HubSpot en sla op; het token blijft hetzelfde.

**Een deal komt in de verkeerde pipeline.** Zonder aanduiding gebruikt HubSpot je standaardpipeline. Noem de pipeline in je opdracht.

**Een contact wordt niet gevonden.** Zoek op e-mail; dat is het betrouwbaarste veld. Namen komen vaker dubbel of anders gespeld voor.

**Het token wordt geweigerd.** Je plakte waarschijnlijk de Client secret in plaats van het access token van de private app.

## Veelgestelde vragen

**Kan GENI mijn hele CRM doorzoeken?**
Hij zoekt gericht op e-mail, naam of bedrijf. Er wordt niets gekopieerd of
geïndexeerd; elke zoekopdracht gaat live naar HubSpot.

**Kan ik dit combineren met andere skills?**
Ja, dat is de meerwaarde: een nieuwe lead uit [Lead Research](lead-research.md)
meteen als contact wegschrijven, of een pipeline-overzicht in je
[weekrapport](weekly-report.md).

**Werkt dit met een gratis HubSpot-account?**
Private apps zijn beschikbaar in de gratis CRM-tiers. Sommige velden en
pipelines vragen wel een betaald HubSpot-plan.

**Wat is het verschil met CRM Sync?**
[CRM Sync](crm-sync.md) houdt gegevens tussen systemen gelijk. Deze skill werkt
rechtstreeks in HubSpot.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [HubSpot koppelen](../connectors/hubspot.md) · [Lead Research](lead-research.md) · [CRM Sync](crm-sync.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, HubSpot CRM, bijgewerkt augustus 2026*
