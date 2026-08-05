# Eigen Workflows

Met Eigen Workflows start GENI een webhook op jouw eigen server of in je eigen n8n, zodat je bestaande automatiseringen vanuit een gesprek kunt aansturen.

Beschikbaar vanaf **Pro**. Je configureert zelf welke webhooks bereikbaar zijn.

## Wat kan GENI hiermee?

- **Een workflow triggeren** op naam, met optionele parameters als JSON
- **Je geconfigureerde workflows tonen**

Dit is de brug naar wat je al hebt draaien. dGENIX voert je workflow niet uit,
hij start hem en geeft het antwoord terug.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Welke workflows heb ik staan?
```

> Je hebt er drie geconfigureerd:
>
> | Naam | Wat hij doet |
> |---|---|
> | offerte-pdf | Genereert een offerte-PDF uit je template |
> | voorraad-sync | Synchroniseert voorraad met je webshop |
> | klant-export | Exporteert een klantdossier als zip |

En bij het starten:

```
Start offerte-pdf voor De Krent, bedrag 4.800
```

> Gestart. De workflow gaf terug:
>
> > `{ "status": "ok", "url": "https://jouwserver.nl/offertes/2026-084.pdf" }`
>
> De offerte staat klaar: [2026-084.pdf](https://jouwserver.nl/offertes/2026-084.pdf)

## Vereisten

- **Plan:** Pro en hoger
- **Koppeling:** een bereikbare webhook-URL, geconfigureerd in je account

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Eigen Workflows**
2. Configureer je webhooks (naam + URL) via **Dashboard → Connectors**
3. Vraag GENI welke workflows er staan

## Wat het kost

| Actie | Credits |
|---|---|
| Workflow triggeren | 10 |
| Workflows tonen | 3 |

Wat je eigen server daarna doet, kost bij dGENIX niets , die rekening loopt bij
jou. Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **De webhook moet publiek bereikbaar zijn.** Interne en privé-adressen worden geblokkeerd, dat is een bewuste veiligheidsmaatregel.
- **GENI wacht op een antwoord.** Duurt je workflow minuten, laat hem dan direct bevestigen en het resultaat later terugsturen.
- **Wat je workflow doet, controleert dGENIX niet.** Een verkeerde parameter kan aan jouw kant echt iets wijzigen.
- **Alleen workflows die je zelf configureerde.** GENI kan geen willekeurige URL aanroepen.
- **Het antwoord komt terug zoals je server het geeft.** Stuur leesbare JSON, dan kan GENI er iets zinnigs mee.

## Problemen oplossen

**"Workflow niet gevonden".** De naam wijkt af van wat er geconfigureerd is. Vraag eerst het overzicht op.

**De webhook wordt geweigerd.** Het adres is niet publiek bereikbaar, of het is een intern netwerkadres. Gebruik een publiek endpoint met authenticatie.

**Time-out.** Je workflow doet er te lang over. Laat hem direct antwoorden en het echte werk in de achtergrond doen.

**De parameters komen verkeerd binnen.** Zeg welke velden je workflow verwacht, dan stuurt GENI ze in die vorm mee.

## Veelgestelde vragen

**Wat is het verschil met de Workflow Builder?**
De [Workflow Builder](workflow-import.md) importeert n8n-JSON en voert de stappen
bij dGENIX uit. Eigen Workflows roept jouw server aan en laat de uitvoering
daar.

**Kan ik dit inplannen?**
Ja. Zet het als [geplande taak](../handleiding/geplande-taken.md), bijvoorbeeld
elke nacht een sync.

**Hoe beveilig ik de webhook?**
Zet er een token of een geheime URL op. dGENIX stuurt wat je configureert; de
authenticatie regel je aan jouw kant.

**Werkt dit met andere tools dan n8n?**
Ja. Elke dienst die een HTTP-webhook accepteert werkt, van Make tot een eigen
script.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Workflow Builder](workflow-import.md) · [Automations](../functies/workflow-automations.md) · [Connectors](../connectors/README.md)
→ Op de site: [alle koppelingen](https://dgenix.nl/integrations) · [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Eigen Workflows, bijgewerkt augustus 2026*
