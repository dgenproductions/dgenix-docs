# Workflow Automations

Workflow Automations zijn terugkerende opdrachten die GENI automatisch uitvoert op vaste tijdstippen, zonder dat jij er iets voor hoeft te doen.

De vuistregel: alles wat je met de hand kunt vragen, kun je ook inplannen. Werkt
een opdracht in de chat, dan werkt hij ook als automation.

## Wat je hiermee kunt

| Wat je inplant | Wanneer het draait |
|---|---|
| Dagoverzicht van je inbox en agenda | Elke werkdag om 08:00 |
| Weekrapport naar je mailbox | Elke maandag |
| SEO-audit van je site | Elke maand |
| Reviewverzoeken naar nieuwe klanten | Elke maandag |
| Social post uit je laatste blog | Wekelijks |

---

## Hoe werkt het?

1. Maak een workflow aan met een naam, instructie en frequentie
2. De assistent voert de taak automatisch uit op het ingestelde tijdstip
3. Het resultaat verschijnt in je dashboard, en wordt gemaild of naar Telegram gestuurd als je dat in de instructie vraagt

---

## Een workflow aanmaken

1. Ga naar **Dashboard → Taken**
2. Klik **+ Nieuwe workflow**
3. Vul in:
   - **Naam:** korte omschrijving (bijv. "Dagelijks nieuwsoverzicht")
   - **Instructie:** wat moet de assistent precies doen?
   - **Frequentie:** hoe vaak moet de taak worden uitgevoerd?
4. Sla op, de workflow is direct actief

**Tip:** schrijf de instructie alsof je de assistent rechtstreeks aanspreekt. Hoe specifieker, hoe beter het resultaat.

---

## Beschikbare frequenties

| Frequentie | Tijdstip |
|------------|----------|
| Dagelijks | 08:00 |
| Werkdagen (ma–vr) | 08:00 |
| Wekelijks | Maandag 08:00 |
| Maandelijks | 1e dag van de maand |

---

## Voorbeelden

- *Dagelijks:* "Geef me een samenvatting van het Nederlandse nieuws van vandaag"
- *Werkdagen:* "Stuur me een motiverende quote voor de dag"
- *Wekelijks:* "Maak een weekplanning voor me op basis van mijn agenda"
- *Maandelijks:* "Herinner me om mijn facturen te controleren en stuur een overzicht van mijn vaste lasten"

---

## Slots per plan

| Plan | Slots inbegrepen |
|------|-----------------|
| Free | 0 slots |
| Starter | 1 slot |
| Growth | 5 slots |
| Pro | 10 slots |
| Business | 20 slots |

**Extra slots bijkopen** (vanaf Pro), via **Account → Abonnement**:

| Pakket | Prijs |
|---|---|
| +1 slot | €6,99/mnd |
| +5 slots | €29,99/mnd |
| +10 slots | €59,99/mnd |

---

## Werkflowbeheer

### In- en uitschakelen
Gebruik de toggle naast een workflow om hem tijdelijk te pauzeren. De workflow wordt niet verwijderd, alleen overgeslagen bij de volgende uitvoeringstijd.

### Uitvoeringsgeschiedenis
Klik op het klok-icoon naast een workflow om de laatste 10 uitvoeringen te bekijken:
- Status (geslaagd / fout)
- Gebruikte credits
- Resultaatsamenvatting

### Bewerken
Klik op het potlood-icoon om naam, instructie of frequentie te wijzigen.

### Verwijderen
Klik op het prullenbakicoon. De workflow wordt permanent verwijderd.

---

## Google Calendar integratie

Als je Google Calendar hebt verbonden (Dashboard → Connectors), verschijnt een **GCal** knop naast elke workflow. Klik erop om de workflow toe te voegen als terugkerend agenda-event, zo zie je de taken ook direct in je agenda.

---

## Credits

Elke automatische uitvoering verbruikt credits op basis van de complexiteit van de taak en het gebruikte model. Bekijk de creditkosten per uitvoering in de uitvoeringsgeschiedenis.

---

## Tabs: Workflows en Templates

De pagina heeft twee tabs bovenaan:

- **Workflows**, je actieve geplande workflows met kalender + lijst + slot-pakketten
- **Templates**, kant-en-klare voorbeelden om snel een workflow op te zetten

Je kunt direct linken naar een tab via `?tab=workflows` of `?tab=templates` in de URL, handig om te delen met je team.

---

## Workflow Templates

In de Templates-tab vind je kant-en-klare voorbeelden voor terugkerende workflows. Elke template heeft een titel, korte beschrijving en de skills die nodig zijn.

### Voor jou

Bovenaan staat een rij **Voor jou**: zes templates die het beste passen bij jouw plan en de skills die je actief hebt. Klik op de **Vernieuwen** knop voor een nieuwe selectie.

### Categorie-secties

Daaronder zie je de templates per categorie: Marketing, Sales, Content, Onderzoek, Communicatie, Rapportage, Operaties en Persoonlijk. Elke categorie heeft zijn eigen indigo icoon.

### Zoeken en filteren

- **Zoekbalk** rechts bovenaan filtert op titel, beschrijving en skill-slug
- **Categorie-dropdown** beperkt de weergave tot één categorie

### Een template gebruiken

Klik op een template-card om een formulier te openen met:
- Titel en instructie al ingevuld
- Frequentie (dagelijks, wekelijks, maandelijks)
- Tijdstip en eventueel dag van de week of maand

In de instructie zie je teksten tussen blokhaken zoals `[mijn segment-naam]`. **Vervang die door je eigen gegevens** (e-mailadres, segmentnaam, klantnaam, bestemming, etc). Wat je weglaat, vraagt de assistent bij de eerste uitvoering.

### Skills die nog niet actief zijn

Als een template skills nodig heeft die jij nog niet hebt geactiveerd, zie je:
- **Geel waarschuwingsbadge** op de template-card (rechts naast de tier-badge) met het aantal ontbrekende skills
- **Oranje waarschuwingsbanner in het formulier** met directe link naar de Skills marketplace

Je kunt de workflow nog wel aanmaken, maar hij faalt bij elke uitvoering tot de skills geactiveerd zijn.

### Geen template gevonden?

Als je zoekopdracht geen resultaten oplevert verschijnen twee knoppen:
- **Nieuwe workflow**, maak zelf een workflow vanaf nul (open formulier zonder template)
- **Template aanvragen**, beschrijf welke workflow je mist; je aanvraag komt direct bij dGENIX support en we voegen geschikte templates toe

---

## Grenzen

- **Het aantal slots hangt af van je plan**: Free 0, Starter 1, Growth 5, Pro 10, Business 20. Extra slots zijn los bij te kopen vanaf Pro.
- **Onomkeerbare acties vragen ook binnen een automation om bevestiging.** Er gaat nooit ongezien een mail of publicatie de deur uit.
- **Een automation faalt als een benodigde skill of koppeling ontbreekt.** Je ziet dat vooraf als waarschuwing bij de template.
- **Credits worden per uitvoering afgeschreven.** Een dagelijkse zware taak telt dus op; kijk vooraf naar de kosten per run.
- **Zonder credits stopt de uitvoering** tot je saldo is aangevuld.
- **De kleinste frequentie is dagelijks.** Voor iets dat vaker moet, start je het handmatig.

## Problemen oplossen

**Je automation draait niet.** Kijk of hij aan staat en of je nog credits hebt. Een gepauzeerde taak blijft staan maar voert niets uit.

**Hij faalt elke keer.** Waarschijnlijk mist een skill of een koppeling. In het overzicht staat de laatste uitvoering met de foutmelding erbij.

**Je kunt geen nieuwe automation aanmaken.** Je slots zijn vol. Verwijder een bestaande of koop extra slots bij.

**Het resultaat komt niet binnen.** Controleer of de taak een bezorgstap heeft, bijvoorbeeld "mail het resultaat naar mij". Zonder die stap blijft het resultaat in het dashboard staan.

**De tijd klopt niet.** Uitvoering volgt de tijdzone van je account; controleer die in Instellingen.

## Veelgestelde vragen

**Wat is het verschil met een taak in de Werkruimte?**
Een automation voert GENI zelf uit op een tijdstip. Een Werkruimte-taak is een
to-do die jij afvinkt. Zie [Werkruimte](werkruimte.md).

**Kan ik een automation tijdelijk uitzetten?**
Ja, met de aan/uit-schakelaar. Je instellingen blijven bewaard.

**Kost een automation extra?**
De automation zelf niet; alleen het werk dat hij uitvoert kost credits, net als
wanneer je het met de hand vraagt.

**Kan ik zien wat er gedraaid heeft?**
Ja, per automation staat de laatste uitvoering met resultaat, en alles komt ook
in de tijdlijn van je Werkruimte.

---

→ Verder: [Geplande taken](../handleiding/geplande-taken.md) · [Werkruimte](werkruimte.md) · [Het creditsysteem](../hoe-het-werkt/credits.md)
→ Op de site: [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, Workflow Automations, bijgewerkt augustus 2026*
