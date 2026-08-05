# Google Sheets koppelen

De Google Sheets-connector geeft GENI toegang tot je spreadsheets, zodat hij data kan ophalen, rijen kan toevoegen en cellen kan bijwerken zonder dat jij het bestand opent.

## Wat je hiermee kunt

| Wat GENI doet | Voorbeeld |
|---|---|
| Data ophalen en samenvatten | "Wat staat er in mijn leads-sheet van deze week?" |
| Nieuwe rijen toevoegen | "Zet deze lead in mijn leads-sheet" |
| Cellen bijwerken | "Zet de status van rij 12 op gebeld" |

De koppeling activeert de **[Google Sheets-skill](../skills/google-sheets.md)**, beschikbaar vanaf Starter.

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast Google Sheets
3. Log in met het Google-account dat toegang heeft tot de spreadsheets die je wilt gebruiken
4. Geef dGENIX de gevraagde rechten
5. Het venster sluit vanzelf, de koppeling is direct actief

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| Spreadsheets lezen | Data ophalen en samenvatten |
| Spreadsheets bewerken | Rijen toevoegen en cellen bijwerken |

dGENIX kan **geen** spreadsheets verwijderen en beheert je Google Drive niet.

## Hoe verwijs je naar een spreadsheet?

Geef de spreadsheet-ID of de volledige URL mee in je opdracht. De ID staat in de
URL tussen `/d/` en `/edit`:

```
https://docs.google.com/spreadsheets/d/1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs/edit
                                       ^--------- dit is de ID ---------^
```

Beide vormen werken:

```
Lees de eerste 10 rijen van spreadsheet 1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs
```

```
Voeg een rij toe aan mijn leads-sheet met naam, e-mail en datum van vandaag
```

## Controleren of het werkt

Vraag GENI direct na het koppelen:

```
Lees de eerste 5 rijen van <jouw spreadsheet-URL>
```

Je krijgt de kolomnamen en de eerste rijen terug. Komt er een foutmelding over
toegang, dan is de spreadsheet niet gedeeld met het gekoppelde account.

## Grenzen

- GENI verwijdert nooit een spreadsheet of tabblad
- Hij ziet alleen spreadsheets waar het gekoppelde account toegang toe heeft
- Formules worden gelezen als hun uitkomst, niet als formule
- Je wijst per opdracht een spreadsheet aan; GENI zoekt niet vanzelf je hele Drive af

## Problemen oplossen

**Koppeling mislukt.** Controleer of je bent ingelogd op het juiste Google-account. Log uit bij Google en probeer het opnieuw.

**GENI vindt de spreadsheet niet.** De spreadsheet is niet gedeeld met het gekoppelde account. Deel hem, of koppel het account dat wel toegang heeft.

**Melding over onvoldoende rechten.** De koppeling is gemaakt zonder bewerkrechten. Verbreek de verbinding en koppel opnieuw, en geef dan alle gevraagde rechten.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Google Sheets en kies **Verbreken**.
Je kunt de toegang ook intrekken bij Google zelf via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Veelgestelde vragen

**Heb ik hiervoor ook de Google Sheets-skill nodig?**
Ja. De connector regelt de toegang, de skill geeft GENI de mogelijkheden. Activeer die via **Dashboard → Skills**.

**Werkt dit met gedeelde spreadsheets van collega's?**
Ja, zolang het gekoppelde Google-account toegang heeft tot dat bestand.

**Kan GENI een nieuwe spreadsheet aanmaken?**
Nee. Hij werkt in bestaande spreadsheets. Een nieuw bestand maak je zelf aan en wijs je daarna toe.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Google Sheets skill](../skills/google-sheets.md)
→ Op de site: [alle koppelingen](https://dgenix.nl/integrations) · [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Google Sheets koppelen, bijgewerkt augustus 2026*
