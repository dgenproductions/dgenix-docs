# Slack koppelen

De Slack-koppeling laat GENI meelezen en meepraten in je werkruimte: kanalen lezen, threads samenvatten, berichten sturen en zoeken in wat er al besproken is.

Je koppelt Slack één keer met een paar klikken. Daarna activeert het de
[Slack-skill](../skills/slack.md), beschikbaar vanaf **Growth**.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Wat is er vandaag in #support gezegd?" | Leest het kanaal en vat samen |
| "Vat de discussie over de release samen" | Leest de hele thread inclusief reacties |
| "Zoek waar we het over de nieuwe prijzen hadden" | Doorzoekt berichten op een zoekterm |
| "Post in #algemeen dat de release live is" | Stuurt een bericht naar een kanaal |
| "Stuur Lisa een DM dat de offerte klaarstaat" | Stuurt een direct message |
| "Zet een duimpje op het laatste bericht van Jan" | Voegt een emoji-reactie toe |
| "Maak een kanaal #project-dewit" | Maakt een nieuw kanaal aan |

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast Slack
3. Kies de werkruimte waarin je GENI wilt toelaten
4. Bekijk de gevraagde rechten en klik op **Toestaan**
5. Het venster sluit vanzelf en Slack staat op **Verbonden**

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| `channels:read` + `channels:history` | Publieke kanalen lezen |
| `groups:read` + `groups:history` | Privékanalen lezen waar de app in zit |
| `chat:write` | Berichten posten |
| `im:read` + `im:write` | Direct messages lezen en sturen |
| `search:read` | Berichten doorzoeken |
| `reactions:write` | Reageren met een emoji |
| `channels:manage` | Een kanaal aanmaken op jouw verzoek |
| `users:read` | Ledenlijst lezen, om de juiste persoon te vinden |
| `files:read` + `files:write` | Bestanden ophalen en uploaden |

GENI komt alleen in kanalen waartoe de koppeling toegang heeft. Een privékanaal
waar de app niet in zit, blijft onzichtbaar.

## Controleren of het werkt

Vraag direct na het koppelen:

```
Welke Slack-kanalen kan je zien?
```

Je krijgt een lijst met kanaalnamen terug. Mist er een kanaal dat je wel
verwacht, dan is het een privékanaal waar de app nog niet in zit.

## Grenzen

- Een bericht versturen vraagt om bevestiging; je ziet de tekst eerst
- GENI verwijdert nooit berichten, kanalen of bestanden
- Privékanalen zijn pas zichtbaar nadat je de app erin uitnodigt
- Berichten worden alleen opgehaald op het moment dat je iets vraagt, er wordt niets doorlopend meegelezen

## Problemen oplossen

**GENI ziet een kanaal niet.** Het is een privékanaal. Typ in Slack `/invite @dGENIX` in dat kanaal.

**Posten lukt niet.** Je werkruimte staat posten door apps mogelijk niet toe. Vraag je Slack-beheerder om de app goed te keuren.

**Je koppelde de verkeerde werkruimte.** Verbreek de koppeling, log in Slack uit bij die werkruimte en koppel opnieuw.

**Oudere berichten zijn niet vindbaar.** Op een gratis Slack-werkruimte beperkt Slack zelf de bewaarde geschiedenis.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Slack en kies **Verbreken**. Je kunt
de app ook verwijderen via *Slack → Instellingen → Apps beheren*.

## Veelgestelde vragen

**Leest GENI al mijn Slack-berichten mee?**
Nee. Hij haalt alleen op wat jouw opdracht nodig heeft, op het moment dat je het
vraagt. Er draait geen achtergrondproces dat je werkruimte indexeert.

**Kan hij automatisch in een kanaal posten?**
Ja, via een herhaalde taak, bijvoorbeeld elke maandag een weekoverzicht in je
teamkanaal. Zie [Geplande taken](../handleiding/geplande-taken.md).

**Kan ik meerdere werkruimtes koppelen?**
Eén werkruimte per account. Wil je wisselen, verbreek de koppeling en koppel de
andere werkruimte.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Slack skill](../skills/slack.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Slack koppelen, bijgewerkt augustus 2026*
