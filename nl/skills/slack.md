# Slack

Met de Slack-skill leest GENI mee in je werkruimte, vat threads samen en post namens jou, zodat je niet alles zelf hoeft te volgen.

Beschikbaar vanaf **Growth**. Je hebt een gekoppelde Slack-werkruimte nodig; zie
[Slack koppelen](../connectors/slack.md).

## Wat kan GENI met Slack?

- **Een kanaal lezen** en de recente berichten ophalen
- **Een thread samenvatten**, inclusief alle reacties
- **Zoeken in berichten** op een zoekterm
- **Je kanalen opsommen** waar de koppeling bij kan
- **Een bericht posten** in een kanaal
- **Een DM sturen** naar een specifieke collega
- **Reageren met een emoji** op een bericht
- **Een kanaal aanmaken**

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Vat de discussie in #release samen, ik was er twee dagen niet
```

> **#release , 34 berichten sinds dinsdag**
>
> **Besloten**
> - De release schuift naar donderdag, vanwege de bug in de betaalflow
> - Sanne pakt de release notes op
>
> **Nog open**
> - Wie doet de communicatie naar klanten? Jan opperde jou, niemand bevestigde.
> - Of de oude API-versie nog een maand blijft draaien; drie meningen, geen besluit.
>
> Je bent twee keer genoemd, beide keren over die klantcommunicatie.

Dat laatste is meestal de reden om dit te vragen: je wilt weten of er iets op je
ligt te wachten.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een Slack-werkruimte via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Slack**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Kies je werkruimte en geef toestemming
4. Slack is direct bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| Reageren met een emoji | ~15 |
| Berichten doorzoeken | ~25 |
| Bericht of DM versturen | ~30 |
| Kanaal lezen en samenvatten | ~40 |
| Thread samenvatten | ~50 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Posten en DM's versturen vragen om bevestiging.** Je ziet de tekst eerst.
- **GENI verwijdert geen berichten of kanalen.**
- **Privékanalen zijn alleen zichtbaar** als de app erin is uitgenodigd (`/invite @dGENIX`).
- **Hij leest niet doorlopend mee.** Berichten worden opgehaald op het moment dat je erom vraagt.
- **Bestanden in Slack worden herkend maar niet geopend.**
- **Op een gratis Slack-werkruimte** beperkt Slack zelf de bewaarde geschiedenis.

## Problemen oplossen

**Een kanaal is niet zichtbaar.** Het is privé. Typ in Slack `/invite @dGENIX` in dat kanaal.

**Posten lukt niet.** Je werkruimte staat posten door apps mogelijk niet toe. Vraag je beheerder om de app goed te keuren.

**Een samenvatting mist context.** Noem de periode erbij ("sinds maandag"), dan haalt GENI meer berichten op.

**Oudere berichten zijn onvindbaar.** Op een gratis werkruimte bewaart Slack maar beperkt geschiedenis.

## Veelgestelde vragen

**Kan GENI automatisch in een kanaal posten?**
Ja, als geplande taak, bijvoorbeeld elke maandag een weekoverzicht in je
teamkanaal. De bevestiging blijft gelden. Zie
[Geplande taken](../handleiding/geplande-taken.md).

**Leest hij al mijn Slack-berichten?**
Nee. Alleen wat je opdracht nodig heeft, op het moment dat je het vraagt.

**Kan ik meerdere werkruimtes koppelen?**
Eén per account. Wisselen betekent verbreken en opnieuw koppelen.

**Kan hij een rapport uit een andere skill in Slack zetten?**
Ja, dat is een sterke combinatie: een [weekrapport](weekly-report.md) of
SEO-audit die vanzelf in je teamkanaal verschijnt.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Slack koppelen](../connectors/slack.md) · [Weekrapport](weekly-report.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Slack, bijgewerkt augustus 2026*
