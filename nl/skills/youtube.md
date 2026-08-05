# YouTube Manager

Met de YouTube Manager leest GENI de cijfers van je eigen kanaal uit, analyseert hij je reacties en doelgroep, en bedenkt hij op basis daarvan wat je hierna zou moeten maken.

Beschikbaar vanaf **Growth**. Je hebt een gekoppeld YouTube-account nodig. De
skill leest alleen; uploaden kan niet.

## Wat kan GENI hiermee?

- **Je kanaal analyseren** , abonnees, weergaves, welke video's het doen en welke niet
- **Video-ideeën genereren** op basis van wat op jouw kanaal werkt
- **Een upload-checklist maken** , titel, beschrijving, tags, thumbnail-advies
- **Videostatistieken opvragen** voor een specifieke video
- **Reacties analyseren** , wat vragen kijkers, waar zit de kritiek, welke onderwerpen komen terug
- **Een analytics-rapport maken** over een periode
- **Doelgroepinzichten geven** , wie kijkt er, wanneer, en hoe lang blijven ze

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Analyseer mijn reacties van de laatste maand
```

> **312 reacties over 6 video's**
>
> **Wat er het vaakst gevraagd wordt**
> - "Werkt dit ook zonder abonnement?" , 23 keer, vooral onder de instructievideo's
> - "Waar vind ik het bestand?" , 18 keer. Je link staat in de beschrijving maar
>   onder de vouw; kijkers zien hem niet.
>
> **Waar de kritiek zit**
> - Het geluid in video 4 is te zacht, 9 losse opmerkingen
> - Twee kijkers vinden de intro te lang (46 seconden)
>
> **Onderwerpen die kijkers zelf aandragen**
> - Een vergelijking met de gratis variant (11 keer genoemd)
> - Een vervolg op de installatie-video (7 keer)
>
> Die eerste vraag beantwoorden in de eerste 30 seconden scheelt je waarschijnlijk
> de helft van de reacties.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** YouTube via **Dashboard → Connectors**. Zie [YouTube koppelen](../connectors/youtube.md)

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **YouTube Manager**
2. Koppel je YouTube-account via **Dashboard → Connectors**
3. Vraag om een kanaalanalyse

## Wat het kost

| Actie | Credits |
|---|---|
| Kanaal analyseren | 10 |
| Videostatistieken | 25 |
| Doelgroepinzichten | 30 |
| Reacties analyseren | 35 |
| Upload-checklist | 40 |
| Analytics-rapport | 40 |
| Video-ideeën genereren | 50 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Alleen lezen.** GENI uploadt geen video's, wijzigt geen titels en reageert niet op reacties.
- **Alleen je eigen kanaal.** Analytics van andermans kanaal zijn niet openbaar; publieke statistieken van een losse video wel.
- **Analytics loopt een dag of twee achter**, dat is YouTube zelf.
- **Een nieuw kanaal geeft weinig terug.** Onder een paar honderd weergaves is er te weinig data voor een zinnig patroon.
- **Geen thumbnails maken.** Hij adviseert erover; het beeld genereer je met [AI Beeldgeneratie](ai-beeldgeneratie.md).

## Problemen oplossen

**"Geen toegang tot analytics".** De koppeling is gemaakt vóór de analytics-rechten erbij kwamen. Verbreek de koppeling en verbind opnieuw.

**De cijfers wijken af van YouTube Studio.** Analytics loopt achter en Studio rekent soms met een andere periode. Noem de periode expliciet.

**Hij vindt mijn video niet.** Geef de video-URL of de exacte titel.

**De ideeën passen niet bij mijn kanaal.** Zeg voor wie je maakt en wat je niet wilt; zonder dat vult hij het in met wat gemiddeld werkt.

## Veelgestelde vragen

**Kan hij video's uploaden?**
Nee. De koppeling is bewust alleen-lezen.

**Werkt dit met Shorts?**
Ja, Shorts zitten in dezelfde statistieken. Voor het máken van shorts is er de
[Short Generator](short-generator.md).

**Kan ik wekelijks een rapport krijgen?**
Ja, via [Geplande taken](../handleiding/geplande-taken.md), bijvoorbeeld elke
maandag een analytics-rapport in je mail.

**Wat is het verschil met de AI Content Engine?**
[Die](ai-content-engine.md) maakt clips uit je video's. De YouTube Manager
analyseert je kanaal en denkt mee over wat je maakt.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Short Generator](short-generator.md) · [AI Content Engine](ai-content-engine.md) · [YouTube koppelen](../connectors/youtube.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, YouTube Manager, bijgewerkt augustus 2026*
