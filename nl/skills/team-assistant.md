# Team Assistent

Met de Team Assistent vat GENI lange teamgesprekken samen tot wat er besloten is en wie wat moet doen, zodat een doorgelopen Slack-kanaal geen achterstand meer is.

Beschikbaar vanaf **Pro**. Werkt met geplakte tekst; met een gekoppelde
[Slack](slack.md) haalt hij de berichten zelf op.

## Wat kan GENI hiermee?

- **Een team-update samenvatten** , een Slack-thread, vergadernotitie of lange mailwisseling terugbrengen tot de kern
- **Actie-items extraheren** , wie doet wat, met deadline waar die genoemd is
- **Slack-berichten ophalen** uit een kanaal (vereist een gekoppelde Slack-werkruimte)

De eerste twee werken ook zonder koppeling: plak de tekst en je krijgt hetzelfde
resultaat.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Vat #project-dekrent van deze week samen en haal de actiepunten eruit
```

> **#project-dekrent , 4 t/m 8 augustus, 63 berichten**
>
> **Waar het over ging**
> De oplevering schoof van week 38 naar week 40 omdat de kassakoppeling
> een extra testronde nodig heeft. De klant is akkoord, de planning is bijgewerkt.
>
> **Besloten**
> - Oplevering week 40
> - Extra testronde op de kassakoppeling, uitgevoerd door de klant zelf
>
> **Actiepunten**
>
> | Wie | Wat | Wanneer |
> |---|---|---|
> | Sanne | Planning bijwerken en klant bevestigen | vrijdag |
> | Jij | Testscript aanleveren | woensdag |
> | Onbekend | Wie doet de eindcontrole? | , |
>
> Die laatste is in het kanaal genoemd maar nooit toegewezen.

## Vereisten

- **Plan:** Pro en hoger
- **Koppeling:** geen, tenzij je berichten uit Slack wilt laten ophalen. Zie [Slack koppelen](../connectors/slack.md)

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Team Assistent**
2. Koppel eventueel Slack via **Dashboard → Connectors**
3. Plak een gesprek, of noem het kanaal dat je wilt laten samenvatten

## Wat het kost

| Actie | Credits |
|---|---|
| Team-update samenvatten | 5 |
| Actie-items extraheren | 5 |
| Slack-berichten ophalen | 3 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **GENI reageert niet namens jou.** Hij leest en vat samen; posten doe je zelf of via de [Slack-skill](slack.md).
- **Alleen kanalen waar de koppeling bij kan.** Privéberichten en besloten kanalen zonder toegang blijven buiten beeld.
- **Actie-items zijn een voorstel.** Een toewijzing die niet expliciet in het gesprek staat, leidt hij af , controleer die voor je hem doorgeeft.
- **Zeer lange periodes worden gedeeltelijk gelezen.** Vraag per week of per thread in plaats van per maand.
- **Hij plant niets in.** Vraag [Google Calendar](google-calendar.md) of je [Werkruimte](../functies/werkruimte.md) om er echt taken van te maken.

## Problemen oplossen

**Het kanaal wordt niet gevonden.** De Slack-koppeling heeft geen toegang tot dat kanaal. Nodig de app uit in het kanaal, of plak de berichten.

**De samenvatting mist de kern.** Zeg waar je op let: besluiten, blokkades, of alleen wat jou raakt.

**Actiepunten staan bij de verkeerde persoon.** In een druk kanaal is de toewijzing vaak impliciet. Corrigeer voor je het deelt.

**Ik wil dit elke maandag.** Zet het als [geplande taak](../handleiding/geplande-taken.md); een weeksamenvatting op maandagochtend is de meest gebruikte vorm.

## Veelgestelde vragen

**Werkt dit ook zonder Slack?**
Ja. Plak de tekst uit welke bron dan ook , Teams, mail, notulen , en je krijgt
hetzelfde resultaat.

**Wat is het verschil met de Vergadering Assistent?**
[Die](meeting-assistant.md) werkt vanaf een opname of transcript van één
vergadering. De Team Assistent werkt op doorlopende teamcommunicatie.

**Kan hij de actiepunten als taken klaarzetten?**
Ja, vraag hem ze in je [Werkruimte](../functies/werkruimte.md) te zetten.

**Leest hij mee in mijn Slack?**
Alleen wanneer je erom vraagt, en alleen in kanalen waar de koppeling toegang
toe heeft. Er draait niets op de achtergrond.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Slack](slack.md) · [Vergadering Assistent](meeting-assistant.md) · [Werkruimte](../functies/werkruimte.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Team Assistent, bijgewerkt augustus 2026*
