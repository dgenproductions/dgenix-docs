# Dashboard

Het dGENIX dashboard is je centrale overzicht voor alles rondom je AI-werknemer — van credits en gebruik tot taken, bestanden en instellingen.

Je bereikt het via [app.dgenix.com](https://app.dgenix.com).

---

## Navigatie

Het dashboard heeft een zijbalk met de volgende secties:

| Sectie | Omschrijving |
|---|---|
| **Home** | Snel overzicht van je saldo, recente activiteit en snelkoppelingen |
| **AI Assistent** | Configureer je assistent, beheer projecten en kennisbank |
| **Skills** | Activeer en beheer extra mogelijkheden |
| **Usage** | Creditverbruik, transactiehistoriek en verloopgrafiek |
| **Billing** | Abonnementsbeheer, facturen en plan upgraden |
| **Bestanden** | Bestanden aangemaakt door je assistent |
| **Taken** | Geplande en terugkerende opdrachten |
| **Settings** | Profiel, integraties, Telegram en assistent-configuratie |

---

## Home

De homepage geeft een direct overzicht van je account:

- **Creditbalans** — je huidige saldo in één oogopslag
- **Recente activiteit** — laatste opdrachten en resultaten
- **Snelkoppelingen** — directe toegang tot veelgebruikte functies

---

## AI Assistent

Hier beheer je de kern van je AI-werknemer:

- **Assistent configureren** — naam, reactiestijl en focusgebieden instellen
- **Projecten** — werkruimtes per klant, campagne of workflow (zie [Projecten](projecten.md))
- **Kennisbank** — documenten uploaden die je assistent als context gebruikt (zie [Kennisbank](kennisbank.md))

---

## Skills

De Skills-pagina toont alle beschikbare uitbreidingen voor je assistent:

- **Actieve skills** — momenteel ingeschakeld, direct beschikbaar via Telegram
- **Marketplace** — nieuwe skills activeren per categorie (persoonlijk, zakelijk, enterprise)
- **Status badges** — actief, binnenkort beschikbaar of plan vereist

Zie [Skills marketplace](../skills/README.md) voor het volledige overzicht.

---

## Usage

De Usage-pagina geeft inzicht in je creditverbruik:

### Huidig saldo
Bovenaan staat een paarse kaart met:
- Je actuele creditbalans
- Je actieve plan (Starter / Growth / Pro)
- Voortgangsbalk: hoeveel van je maandelijkse credits je al hebt gebruikt

### Recente transacties
Een lijst van de laatste creditbewegingen, met:
- Omschrijving van de transactie (bv. "Gmail skill gebruikt")
- Bedrag in credits (rood = verbruik, groen = bijschrijving)
- Datum

Paginering: 10 transacties per pagina, navigeer met ← Vorige / Volgende →.

### Creditverloop (grafiek)
Een lijndiagram dat je creditbalans over tijd weergeeft — vergelijkbaar met een portfolio-grafiek. Je kunt schakelen tussen:

| Periode | Toont |
|---|---|
| **Dag** | Verloop per uur (afgelopen 24 uur) |
| **Week** | Verloop per dag (afgelopen 7 dagen) |
| **Maand** | Verloop per dag (afgelopen 30 dagen) |
| **Jaar** | Verloop per maand (afgelopen 12 maanden) |

Gebruik de grafiek om te zien wanneer er pieken in verbruik ontstaan — handig om te bepalen of je een hoger plan of extra credits nodig hebt.

### Credits bijkopen
Onderaan de pagina koop je eenmalig extra credits bij:

| Pack | Credits | Prijs |
|---|---|---|
| Small | 25.000 | €9 |
| Medium | 60.000 | €20 |
| Large | 150.000 | €45 |

Zie ook [Credits bijkopen](../plannen-en-prijzen/credits-bijkopen.md).

---

## Billing

Beheer hier je abonnement:

- **Huidig plan** — actieve periode en verlengdatum
- **Facturen** — overzicht van eerdere betalingen
- **Plan wijzigen** — upgraden of downgraden via Stripe
- **Betaalmethode** — beheren via het Stripe klantportaal

---

## Bestanden

Overzicht van alle bestanden die je assistent heeft aangemaakt of ontvangen:

- Documenten, samenvattingen, rapporten
- Per bestand: naam, type, aanmaakdatum en de skill die het heeft aangemaakt
- Direct downloaden of bekijken

---

## Taken

Beheer hier geplande en terugkerende opdrachten:

- **Actieve taken** — opdrachten die automatisch worden uitgevoerd
- **Frequentie** — dagelijks, wekelijks of op een vast tijdstip
- **Status** — laatste uitvoering en resultaat
- **Aan/uit** — taken tijdelijk pauzeren zonder ze te verwijderen

---

## Settings

De instellingenpagina heeft meerdere tabs:

### Profiel
- Naam en e-mailadres aanpassen
- Wachtwoord wijzigen

### Integraties
Koppel externe diensten via OAuth:
- Gmail
- Google Calendar
- Google Drive
- Google Sheets

Zie [Integraties](../integraties/gmail.md) voor stap-voor-stap instructies.

### Assistent
- **Naam** — hoe je assistent zich introduceert via Telegram
- **Reactiestijl** — formeel, informeel of kort & bondig
- **Focusgebieden** — op welke taken je assistent prioriteit geeft
- **Aangepaste regels** — eigen instructies die altijd gelden

### Kennisdocument
Upload of bewerk het kennisdocument dat je assistent als vaste context gebruikt — bedrijfsinfo, klantgegevens, werkwijze.

### Telegram
- Verbindingsstatus van je Telegram-koppeling
- Eigen bot instellen (optioneel, via own-bot add-on)

---

## Changelog

| Datum | Wijziging |
|---|---|
| 2026-04-02 | Usage-pagina: 2-kolom layout met transactiepaginering en creditverloopgrafiek (dag/week/maand/jaar) |
| 2026-04-02 | Dashboard-pagina aangemaakt in de documentatie |
