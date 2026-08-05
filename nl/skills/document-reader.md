# Document Lezer

Met de Document Lezer laat je GENI een webpagina of een lap tekst lezen en er antwoord uit geven: een samenvatting, de kernpunten of het antwoord op één gerichte vraag.

Beschikbaar vanaf **Starter**. Je hebt geen koppeling nodig.

## Wat kan GENI hiermee?

- **Een document of webpagina analyseren** vanaf een URL of vanaf tekst die je in de chat plakt, met de vraag die je erbij stelt

Eén tool, maar de vraag bepaalt wat je terugkrijgt: samenvatten, kernpunten
eruit halen, twee stukken vergelijken of één ding opzoeken.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Vat deze algemene voorwaarden samen en zeg wat er opvalt
[tekst geplakt]
```

> **Samenvatting , Algemene voorwaarden leverancier X**
>
> - Betaaltermijn **14 dagen**, daarna 2 procent rente per maand
> - Opzegtermijn **drie maanden**, alleen per einde kwartaal
> - Aansprakelijkheid beperkt tot het factuurbedrag van de laatste 6 maanden
>
> **Wat opvalt**
> - Artikel 9 laat prijsverhoging **eenzijdig** toe met 30 dagen aankondiging
> - Er staat geen enkele afspraak over levertijd in

En vanaf een URL:

```
https://voorbeeld.nl/onderzoek-2026 , wat zeggen ze over het MKB?
```

> Het rapport noemt het MKB in twee passages. Kern: 34 procent gebruikt AI
> wekelijks, tegen 71 procent bij bedrijven boven de 250 werknemers. De reden
> die genoemd wordt is niet prijs maar tijd om het in te richten.
>
> *Bron: voorbeeld.nl/onderzoek-2026*

## Vereisten

- **Plan:** Starter en hoger
- **Koppeling:** geen

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Document Lezer**
2. Plak een URL of de tekst in de chat en stel je vraag

## Wat het kost

| Actie | Credits |
|---|---|
| Document of pagina analyseren | 5 |

Daar komt het gesprek zelf bij; zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Deze skill werkt met een URL of geplakte tekst.** Wil je een bestand meesturen, gebruik dan de bijlage-knop in de chat , dat loopt via de chat zelf en niet via deze skill.
- **Bijlagen in de chat:** afbeeldingen, PDF, txt, markdown en csv, maximaal **5 MB per bestand** en **3 bestanden per bericht**.
- **Een pagina achter een login of paywall kan hij niet ophalen.** Plak de tekst dan zelf.
- **Interne of privé-adressen worden geblokkeerd.** Alleen publiek bereikbare URL's, dat is een bewuste veiligheidsmaatregel.
- **Zeer lange documenten worden gedeeltelijk gelezen.** Stel een gerichte vraag of lever het relevante deel aan.
- **Hij bewaart het document niet.** Wil je er later nog uit kunnen zoeken, gebruik dan de [Support Kennisbank](knowledge-base.md).

## Problemen oplossen

**"URL ophalen mislukt".** De pagina blokkeert geautomatiseerde bezoeken of vraagt om een login. Plak de tekst rechtstreeks in de chat.

**"Geen bruikbare inhoud gevonden".** De pagina bouwt zijn inhoud met JavaScript op, of het is een PDF achter een viewer. Kopieer de tekst.

**Het antwoord is te oppervlakkig.** Stel een scherpere vraag. "Wat staat er over de opzegtermijn" levert meer op dan "vat samen".

**Ik wil het document later terugvinden.** Dat kan deze skill niet. Zet het in de [Support Kennisbank](knowledge-base.md) of bewaar de samenvatting als notitie in je [Werkruimte](../functies/werkruimte.md).

## Veelgestelde vragen

**Kan ik een PDF meesturen?**
Ja, via de bijlage-knop in de chat (tot 5 MB). Dat loopt via de chat, niet via
deze skill, dus je betaalt er de 5 credits van deze skill niet voor.

**Wat is het verschil met de Support Kennisbank?**
Deze skill leest één stuk, nu. De [Kennisbank](knowledge-base.md) indexeert je
documentatie zodat je er maanden later nog uit kunt zoeken.

**Werkt het met een Google Docs-link?**
Met een publiek deelbare link wel. Staat het document op besloten, koppel dan
[Google Drive](google-drive.md).

**Kan hij twee documenten vergelijken?**
Ja, plak ze allebei en vraag om het verschil.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Support Kennisbank](knowledge-base.md) · [Google Drive](google-drive.md) · [Werkruimte](../functies/werkruimte.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Document Lezer, bijgewerkt augustus 2026*
