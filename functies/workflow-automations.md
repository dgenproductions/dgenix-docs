# Workflow Automations

Workflow Automations zijn terugkerende opdrachten die je assistent automatisch uitvoert op vaste tijdstippen — zonder dat jij er iets voor hoeft te doen.

---

## Hoe werkt het?

1. Maak een workflow aan met een naam, instructie en frequentie
2. De assistent voert de taak automatisch uit op het ingestelde tijdstip
3. Je ontvangt het resultaat via Telegram

---

## Een workflow aanmaken

1. Ga naar **Dashboard → Workflows**
2. Klik **+ Nieuwe workflow**
3. Vul in:
   - **Naam:** korte omschrijving (bijv. "Dagelijks nieuwsoverzicht")
   - **Instructie:** wat moet de assistent precies doen?
   - **Frequentie:** hoe vaak moet de taak worden uitgevoerd?
4. Sla op — de workflow is direct actief

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
| Starter | 1 slot |
| Growth | 5 slots |
| Pro | 10 slots |

**Extra slots bijkopen:** €9,99/mnd per +5 slots (beschikbaar voor Growth & Pro). Koop extra slots via **Billing** of via de info-sectie op de Workflows pagina.

---

## Werkflowbeheer

### In- en uitschakelen
Gebruik de toggle naast een workflow om hem tijdelijk te pauzeren. De workflow wordt niet verwijderd — alleen overgeslagen bij de volgende uitvoeringstijd.

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

Als je Google Calendar hebt verbonden (Settings → Integraties), verschijnt een **GCal** knop naast elke workflow. Klik erop om de workflow toe te voegen als terugkerend agenda-event — zo zie je de taken ook direct in je agenda.

---

## Credits

Elke automatische uitvoering verbruikt credits op basis van de complexiteit van de taak en het gebruikte model. Bekijk de creditkosten per uitvoering in de uitvoeringsgeschiedenis.

---

## Tabs: Workflows en Templates

De pagina heeft twee tabs bovenaan:

- **Workflows** , je actieve geplande workflows met kalender + lijst + slot-pakketten
- **Templates** , kant-en-klare voorbeelden om snel een workflow op te zetten

Je kunt direct linken naar een tab via `?tab=workflows` of `?tab=templates` in de URL , handig om te delen met je team.

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
- **Nieuwe workflow** , maak zelf een workflow vanaf nul (open formulier zonder template)
- **Template aanvragen** , beschrijf welke workflow je mist; je aanvraag komt direct bij dGENIX support en we voegen geschikte templates toe
