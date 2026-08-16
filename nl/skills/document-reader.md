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

## Een PDF wordt echt gelezen

Geef je een link naar een PDF, dan gaat het bestand zélf naar het model. Dat is
iets anders dan er platte tekst uit persen: **tabellen blijven tabellen, kolommen
lopen niet door elkaar, en een gescand document wordt gewoon gelezen.** Precies
het verschil tussen een factuur uitlezen en ernaar gokken.

Je hoeft niets aan te zetten. Ziet GENI dat de link een PDF is, dan neemt hij die
route automatisch.

## Wat het kost

| Actie | Credits |
|---|---|
| Webpagina of geplakte tekst analyseren | 5 |
| PDF lezen | 10 per pagina, minimaal 25 |

Een PDF van één kantje kost dus 25 credits, een rapport van twintig pagina's 200.
Je betaalt naar wat het model werkelijk moet lezen. GENI noemt de prijs voordat hij
een PDF openslaat. Daar komt het gesprek zelf bij; zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

**Of stuur het bestand mee.** Dezelfde PDF kun je ook als bijlage in de chat sturen
(paperclip, tot 5 MB). Die route loopt niet via deze skill maar via het gesprek zelf,
dus je betaalt daar de gewone gesprekskosten in plaats van een prijs per pagina. Een
link is handig als het bestand ergens online staat; uploaden is handig als je het op
je eigen computer hebt.

## Grenzen en limieten

- **PDF tot 25 pagina's en 10 MB.** Groter wordt geweigerd met de reden erbij, in plaats van half gelezen. Splits het document of geef aan welk deel je bedoelt.
- **Wil je een bestand meesturen in plaats van een link?** Gebruik de bijlage-knop in de chat , dat loopt via de chat zelf en niet via deze skill.
- **Bijlagen in de chat:** afbeeldingen, PDF, txt, markdown en csv, maximaal **5 MB per bestand** en **3 bestanden per bericht**.
- **Een pagina achter een login of paywall kan hij niet ophalen.** Plak de tekst dan zelf.
- **Interne of privé-adressen worden geblokkeerd.** Alleen publiek bereikbare URL's, dat is een bewuste veiligheidsmaatregel.
- **Zeer lange documenten worden gedeeltelijk gelezen.** Stel een gerichte vraag of lever het relevante deel aan.
- **Hij bewaart het document niet.** Wil je er later nog uit kunnen zoeken, gebruik dan de [Support Kennisbank](knowledge-base.md).

## Problemen oplossen

**"URL ophalen mislukt".** De pagina blokkeert geautomatiseerde bezoeken of vraagt om een login. Plak de tekst rechtstreeks in de chat.

**"Geen bruikbare inhoud gevonden".** De pagina bouwt zijn inhoud met JavaScript op, of de PDF zit achter een viewer in plaats van dat de link naar het bestand zelf wijst. Kopieer de tekst, of geef de directe link naar het `.pdf`.

**"Deze PDF heeft ongeveer X pagina's".** Boven de 25 pagina's leest hij hem niet in één keer. Splits het document, of vraag om het deel dat je nodig hebt.

**Het antwoord is te oppervlakkig.** Stel een scherpere vraag. "Wat staat er over de opzegtermijn" levert meer op dan "vat samen".

**Ik wil het document later terugvinden.** Dat kan deze skill niet. Zet het in de [Support Kennisbank](knowledge-base.md) of bewaar de samenvatting als notitie in je [Werkruimte](../functies/werkruimte.md).

## Veelgestelde vragen

**Kan ik een PDF laten lezen?**
Ja. Geef een link naar het `.pdf` en het bestand gaat zelf naar het model, met
tabellen en scans intact. Dat kost 10 credits per pagina, tot 25 pagina's. Wil je een bestand
meesturen in plaats van een link, gebruik dan de bijlage-knop in de chat (tot
5 MB); dat loopt via de chat en niet via deze skill.

**Waarom is een PDF zoveel duurder dan een webpagina?**
Omdat er veel meer te verwerken valt. Een pagina tekst is een paar duizend tokens,
een PDF van 25 pagina's ruim dertigduizend, en bij een PDF gaat ook de opmaak mee
zodat tabellen kloppen. Je betaalt dus voor wat het model werkelijk leest.

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
