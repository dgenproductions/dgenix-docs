# Google Sheets koppelen

Door Google Sheets te koppelen kan je AI-werknemer je spreadsheets lezen, bijwerken en nieuwe rijen toevoegen.

> Google Sheets is beschikbaar als add-on skill voor alle plannen.

---

## Wat kan je assistent met Google Sheets?

- Spreadsheet data ophalen en samenvatten
- Nieuwe rijen toevoegen (bijv. leads, notities, taken)
- Bestaande cellen bijwerken
- Data analyseren en inzichten rapporteren

---

## Google Sheets koppelen

1. Ga naar **Dashboard → Instellingen → Integraties**
2. Klik op **"Verbinden"** naast Google Sheets
3. Er opent een venster — log in met je Google-account
4. Geef dGENIX de gevraagde rechten
5. Het venster sluit automatisch — de koppeling is actief

> Je hebt ook de **Google Sheets skill** nodig. Activeer die via **Dashboard → Skills**.

---

## Welke rechten vraagt dGENIX?

| Recht | Waarvoor |
|---|---|
| Spreadsheets lezen | Data ophalen en samenvatten |
| Spreadsheets bewerken | Rijen toevoegen en cellen bijwerken |

dGENIX kan **geen** spreadsheets verwijderen of je Google Drive beheren.

---

## Hoe verwijs je naar een spreadsheet?

Geef de spreadsheet ID of de volledige URL mee in je opdracht:

```
Lees de eerste 10 rijen van spreadsheet 1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgVE2upms
```
```
Voeg een nieuwe rij toe aan mijn leads-sheet: https://docs.google.com/spreadsheets/d/1BxiM...
```

De spreadsheet ID staat in de URL tussen `/d/` en `/edit`.

---

## Google Sheets ontkoppelen

1. Ga naar **Dashboard → Instellingen → Integraties**
2. Klik op **"Verwijder"** naast Google Sheets
3. De verbinding wordt direct verbroken

Je kunt de koppeling ook intrekken via [myaccount.google.com/permissions](https://myaccount.google.com/permissions).

---

## Problemen?

**Koppeling mislukt:** Controleer of je bent ingelogd op het juiste Google-account. Probeer het opnieuw.

**Assistent vindt de spreadsheet niet:** Zorg dat je het Google-account hebt gekoppeld dat toegang heeft tot de betreffende spreadsheet.

**Vragen?** Stuur een bericht naar [support@dgenix.nl](mailto:support@dgenix.nl).
