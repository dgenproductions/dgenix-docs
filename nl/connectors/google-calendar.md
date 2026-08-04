# Google Calendar koppelen

De Google Calendar-connector laat GENI je agenda raadplegen, afspraken inplannen en beschikbaarheid controleren, zonder dat je zelf je agenda hoeft te openen.

## Wat je hiermee kunt

| Wat GENI doet | Voorbeeld |
|---|---|
| Je agenda opvragen | "Wat staat er vandaag op mijn agenda?" |
| Beschikbaarheid controleren | "Ben ik dinsdag om 10:00 vrij?" |
| Een afspraak inplannen | "Plan vrijdag 14:00 een meeting met Jan en stuur een uitnodiging" |

De koppeling activeert de **[Google Calendar-skill](../skills/google-calendar.md)**, beschikbaar vanaf Starter.

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast Google Calendar
3. Log in met het Google-account waarvan je de agenda wilt gebruiken
4. Geef dGENIX de gevraagde rechten
5. Het venster sluit vanzelf, de koppeling is direct actief

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| Agenda lezen | Afspraken opvragen en beschikbaarheid controleren |
| Agenda aanpassen | Afspraken aanmaken, verzetten en annuleren |

dGENIX past je agenda **alleen** aan op jouw expliciete opdracht.

## Controleren of het werkt

Vraag GENI direct na het koppelen:

```
Wat staat er deze week op mijn agenda?
```

Je krijgt je afspraken per dag terug. Blijft het leeg terwijl je wel afspraken
hebt, dan is waarschijnlijk het verkeerde Google-account gekoppeld.

## Grenzen

- GENI verzet of annuleert nooit een afspraak zonder dat jij dat vraagt
- Hij ziet alleen agenda's van het gekoppelde account, niet die van collega's die niet met je gedeeld zijn
- Terugkerende afspraken worden gelezen, maar de reeks zelf past hij niet aan
- Een uitnodiging versturen vraagt om bevestiging voordat de mail uitgaat

## Problemen oplossen

**Koppeling mislukt.** Controleer of je in je browser bent ingelogd op het juiste Google-account en probeer het opnieuw.

**GENI ziet je afspraken niet.** Je hebt een ander Google-account gekoppeld dan waar je agenda in staat. Verbreek de verbinding en koppel het juiste account.

**Afspraak komt in de verkeerde tijdzone.** GENI volgt de tijdzone van je Google Calendar. Controleer die in je Google-agenda-instellingen.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Google Calendar en kies **Verbreken**.
Je kunt de toegang ook intrekken bij Google zelf via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Veelgestelde vragen

**Is dit dezelfde koppeling als Gmail?**
Nee, het zijn losse connectors. Je koppelt ze allebei apart, ook als het om hetzelfde Google-account gaat.

**Kan GENI mij herinneren aan een afspraak?**
Ja, via een herhaalde taak in **Dashboard → Taken**. Bijvoorbeeld elke werkdag om 08:00 een overzicht van je dag.

**Werkt dit met meerdere agenda's?**
GENI leest de agenda's van het gekoppelde account. Wijs in je opdracht aan welke je bedoelt als je er meerdere hebt.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Google Calendar skill](../skills/google-calendar.md)

*dGENIX Docs, Google Calendar koppelen, bijgewerkt augustus 2026*
