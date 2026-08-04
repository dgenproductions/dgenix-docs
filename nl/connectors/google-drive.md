# Google Drive koppelen

De Google Drive-connector geeft GENI toegang tot je bestanden, zodat hij documenten kan zoeken, lezen en samenvatten, en mappen kan ordenen zonder dat jij Drive opent.

## Wat je hiermee kunt

| Wat GENI doet | Voorbeeld |
|---|---|
| Bestanden zoeken | "Zoek het contract van Van Dijk" |
| Documenten lezen en samenvatten | "Vat het projectplan in mijn Drive samen" |
| Mappen aanmaken | "Maak een map Offertes 2026" |
| Bestanden verplaatsen | "Zet dit bestand in de map Klanten" |
| Bestanden delen | "Deel dit document met jan@bedrijf.nl" |

De koppeling activeert de **[Google Drive-skill](../skills/google-drive.md)**, beschikbaar vanaf Starter.

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast Google Drive
3. Log in met het Google-account waarvan je de bestanden wilt gebruiken
4. Geef dGENIX de gevraagde rechten
5. Het venster sluit vanzelf, de koppeling is direct actief

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| Drive-bestanden lezen | Zoeken, openen en samenvatten |
| Drive-bestanden beheren | Mappen aanmaken, bestanden verplaatsen en delen |

Dit is een brede toegang: GENI kan bij alle bestanden van het gekoppelde
account. Hij **verwijdert nooit** een bestand, en delen gebeurt alleen op jouw
expliciete opdracht.

## Controleren of het werkt

Vraag GENI direct na het koppelen:

```
Zoek in mijn Drive naar bestanden met "offerte" in de naam
```

Je krijgt een lijst met bestandsnamen en locaties terug. Blijft die leeg terwijl
je wel zulke bestanden hebt, dan is het verkeerde Google-account gekoppeld.

## Grenzen

- GENI verwijdert nooit bestanden of mappen
- Delen gebeurt alleen als je er expliciet om vraagt
- Hij ziet alleen bestanden van het gekoppelde account, plus wat met dat account gedeeld is
- Zeer grote bestanden worden gedeeltelijk gelezen; vraag om een specifiek hoofdstuk of tabblad

## Problemen oplossen

**Koppeling mislukt.** Controleer of je bent ingelogd op het juiste Google-account en probeer het opnieuw.

**GENI vindt een bestand niet.** Het bestand staat in een andere Drive of is niet gedeeld met het gekoppelde account. Controleer de eigenaar van het bestand.

**Delen lukt niet.** Het bestand heeft een gedeelde-schijf-instelling die extern delen blokkeert. Dat is een instelling bij Google, niet bij dGENIX.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Google Drive en kies **Verbreken**.
Je kunt de toegang ook intrekken bij Google zelf via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Veelgestelde vragen

**Is dit dezelfde koppeling als Gmail?**
Nee, het zijn losse connectors. Je koppelt ze apart, ook als het om hetzelfde Google-account gaat.

**Kan GENI in gedeelde schijven werken?**
Ja, als het gekoppelde account toegang heeft tot die gedeelde schijf.

**Leest dGENIX al mijn bestanden?**
Alleen wat nodig is voor je opdracht. Er wordt niets automatisch doorzocht of geïndexeerd zonder dat je erom vraagt.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Google Drive skill](../skills/google-drive.md)

*dGENIX Docs, Google Drive koppelen, bijgewerkt augustus 2026*
