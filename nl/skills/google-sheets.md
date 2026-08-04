# Google Sheets

Met de Google Sheets-skill leest GENI je spreadsheets, rekent ermee en schrijft er nieuwe regels in, zodat je bijhouden niet met de hand hoeft.

Beschikbaar vanaf **Starter**. Je hebt een gekoppeld Google-account nodig; zie
[Google Sheets koppelen](../connectors/google-sheets.md).

## Wat kan GENI met Google Sheets?

- **Data lezen** uit een spreadsheet, een heel blad of een bereik
- **Data schrijven of bijwerken** in bestaande cellen
- **Een rij toevoegen** onderaan een blad

Daarmee kun je cijfers laten samenvatten, een lijst laten aanvullen of een
spreadsheet als eenvoudige database gebruiken.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Wat waren mijn omzetcijfers per maand in mijn omzet-sheet?
```

> Uit **Omzet 2026**, blad *Maandoverzicht*:
>
> | Maand | Omzet | Verschil |
> |---|---|---|
> | Mei | € 18.400 | , |
> | Juni | € 21.900 | +19% |
> | Juli | € 17.200 | -21% |
>
> Juli valt op: dat is je laagste maand sinds maart. De daling zit vooral in
> onderhoudscontracten.

En bij het schrijven zie je eerst wat er komt te staan:

```
Voeg een rij toe: 3 augustus, De Vries, 8450, offerte verstuurd
```

> Toe te voegen aan **Offertes 2026**, onderaan:
> `03-08-2026 | De Vries | € 8.450 | offerte verstuurd`
>
> Zal ik dat doen?

## Vereisten

- **Plan:** Starter en hoger
- **Koppeling:** een Google-account via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Google Sheets**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Doorloop het Google-toestemmingsscherm
4. Sheets is direct bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| Data ophalen en samenvatten | ~25 |
| Rij toevoegen | ~20 |
| Data analyseren | ~35 |

De skill zit in je plan; je betaalt per actie. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Schrijven vraagt om bevestiging.** Je ziet wat er komt te staan voordat het gebeurt.
- **GENI verwijdert geen rijen, bladen of spreadsheets.**
- **Formules worden gelezen als waarde, niet herschreven.** Hij zet geen formules voor je op.
- **Opmaak, kleuren en voorwaardelijke opmaak blijven buiten beeld.**
- **Bij zeer grote bladen wordt een deel gelezen.** Noem een bereik als je een specifiek stuk wilt.
- **Draaitabellen en grafieken worden niet geïnterpreteerd.**

## Problemen oplossen

**Hij vindt het spreadsheet niet.** Noem de exacte naam, of geef de URL van het document. Bij meerdere bestanden met dezelfde naam helpt de URL.

**De verkeerde kolommen worden gelezen.** Noem het bladnaam en het bereik, bijvoorbeeld "blad Maandoverzicht, kolom A tot D".

**Een toegevoegde rij staat op de verkeerde plek.** De rij wordt onderaan toegevoegd. Wil je hem ergens anders, doe dat dan zelf.

**Getallen kloppen niet.** Controleer of de cellen als tekst zijn opgemaakt; dan leest GENI ze ook als tekst.

## Veelgestelde vragen

**Kan ik een spreadsheet als database gebruiken?**
Voor eenvoudige lijsten werkt dat prima: leads, offertes, voorraad. Voor iets
complexers is de Airtable-skill geschikter.

**Kan GENI dit automatisch bijhouden?**
Ja, als geplande taak, bijvoorbeeld wekelijks een regel met je cijfers. Zie
[Geplande taken](../handleiding/geplande-taken.md).

**Werkt dit met gedeelde spreadsheets?**
Ja, mits jouw account er toegang toe heeft.

**Kan hij een nieuw spreadsheet maken?**
Nee, hij werkt in bestaande bladen. Maak het bestand zelf aan en laat GENI het
vullen.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Sheets koppelen](../connectors/google-sheets.md) · [Google Drive](google-drive.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Google Sheets, bijgewerkt augustus 2026*
