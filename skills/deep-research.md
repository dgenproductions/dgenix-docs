# Deep Research

## Wat doet deze skill?

Deep Research voert diepgaand multi-iteratie onderzoek uit. Je geeft één onderzoeksonderwerp, en je assistent splitst het op in 4 tot 8 deelvragen, doet voor elke deelvraag een gerichte web search, en synthetiseert een eindrapport met TLDR, bevindingen per thema en een genummerde bronnenlijst. Ideaal voor markt-, branche- en concurrentie-analyses zonder zelf tien zoekopdrachten te hoeven doen.

## Vereisten

- **Plan:** Growth+
- **Integraties:** geen , de skill gebruikt ingebouwde web search

## Hoe activeer je de skill?

1. Ga naar **Skills** in het dashboard
2. Zoek **Deep Research** en klik op **Activeren**
3. Open de **Assistent** en klik onderaan op **Tools** , kies **Deep Research**
4. Typ je onderzoeksvraag en druk op Enter

Je kunt de skill ook activeren via een suggestie zoals "Diepgaand marktonderzoek" op het lege chatscherm, of door je vraag te beginnen met "Onderzoek diepgaand ..." of "Deep research ..." , de assistent kiest dan automatisch het juiste model en de skill.

## Wat kun je ermee?

### Marktonderzoek
"Voer een diepgaand marktonderzoek uit naar Nederlandse e-commerce platforms voor MKB in 2026, focus op pricing en feature-set."

### Concurrentie-analyse
"Maak een concurrentie-analyse met onderbouwde bronnen voor [bedrijf] versus [concurrent 1] en [concurrent 2]."

### Trendrapport
"Onderzoek de belangrijkste trends in generative AI voor zorgverleners, met praktijkvoorbeelden en bronnen."

### Due diligence
"Doe achtergrond-onderzoek naar [partner of klant], inclusief recente activiteiten, leiderschap en perspublicaties."

## Output

Elk Deep Research-rapport bevat:

- **TLDR** , 3-zinnen samenvatting voor management
- **Bevindingen** , per thema gegroepeerd, met inline citaties zoals `[1]` en `[2]`
- **Bronnen** , genummerde lijst met titel + URL

Geen speculatie zonder bron. Wat niet uit de bronnen komt wordt expliciet als zodanig benoemd.

## Creditkosten

| Type | Deelvragen | Verwachte credits | Hard cap |
|---|---|---|---|
| Standard | 4 | ~3.500 cr | 4.500 cr |
| Deep | 8 | ~7.500 cr | 8.500 cr |

De skill gebruikt het Sonnet model (krachtiger en duurder) omdat decompositie en synthese met bronnen meer redenering vereisen.

## Tips

- Wees specifiek in je onderwerp. "Trends in marketing" geeft te brede resultaten , "Trends in B2B SaaS marketing voor MKB in Nederland 2026" levert betere bronnen op.
- Voeg met `focus` extra context toe ("vooral B2B", "Nederlandse markt", "alleen open data").
- Gebruik **deep** alleen voor grote vraagstukken. Voor de meeste vragen is **standard** snel genoeg en de helft goedkoper.
- Bewaar rapporten in een projectmap , Deep Research-rapporten zijn later goud waard als referentie.
