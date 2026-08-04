# Google Analytics

Met de Google Analytics-skill vraag je je bezoekerscijfers gewoon in gewone taal op, in plaats van je een weg te klikken door het Analytics-dashboard.

Beschikbaar vanaf **Growth**. Je hebt een gekoppeld Google-account nodig met
toegang tot de GA4-property.

## Wat kan GENI met Google Analytics?

- **Een verkeersoverzicht**: sessies, gebruikers en bouncepercentage
- **Je best bezochte pagina's**, met sessies en gemiddelde tijd op pagina
- **Verkeersbronnen analyseren**: organisch, social, direct en betaald
- **Doelgroepinzichten**: apparaten, landen en terugkerende bezoekers

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Hoe liep mijn website vorige maand?
```

> **Juli 2026** , 3.480 sessies van 2.910 gebruikers *(+12% t.o.v. juni)*
>
> | Bron | Sessies | Aandeel |
> |---|---|---|
> | Organisch zoeken | 1.910 | 55% |
> | Direct | 780 | 22% |
> | Social | 560 | 16% |
> | Overig | 230 | 7% |
>
> Je bouncepercentage ging van 61% naar 54%, wat vooral komt door de
> dienstenpagina. Die trok 340 sessies met een gemiddelde tijd van 2:40, ruim
> boven je siteniveau.
>
> Opvallend: social groeide 40%, maar die bezoekers blijven gemiddeld 22
> seconden. Daar valt winst te halen.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een Google-account met toegang tot de GA4-property

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Google Analytics**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Doorloop het Google-toestemmingsscherm
4. Analytics is direct bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| Best bezochte pagina's | 30 |
| Verkeersoverzicht | 35 |
| Verkeersbronnen | 35 |
| Doelgroepinzichten | 40 |

De skill zit in je plan; je betaalt per actie. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Alleen GA4.** De oude Universal Analytics wordt niet ondersteund; die is door Google uitgezet.
- **Je ziet alleen properties waar jouw account bij kan.**
- **De skill leest, hij wijzigt niets.** Doelen, filters en events stel je in Analytics zelf in.
- **Realtime-data zit er niet in.** Reken op cijfers tot gisteren.
- **Aangepaste dimensies en events worden niet uitgelezen**, alleen de standaardrapporten.

## Problemen oplossen

**Er komt geen data.** Je account heeft geen toegang tot de property, of er is nog geen GA4 ingesteld. Controleer dat in Analytics zelf.

**De cijfers wijken af van Search Console.** Dat hoort. [Search Console](google-search-console.md) telt vertoningen en klikken in Google; Analytics telt wat er op je site gebeurt. Verschillen zijn normaal.

**Je ziet minder bezoekers dan verwacht.** Cookiebanners en adblockers zorgen dat een deel van het verkeer niet gemeten wordt. Dat geldt voor iedereen.

**Je hebt meerdere properties.** Noem de site erbij, dan pakt GENI de juiste.

## Veelgestelde vragen

**Kan ik een maandrapport laten sturen?**
Ja, als geplande taak met de uitkomst per mail. Zie
[Geplande taken](../handleiding/geplande-taken.md).

**Kan GENI dit combineren met andere data?**
Ja, dat is de meerwaarde: samen met
[Search Console](google-search-console.md) zie je niet alleen hoeveel bezoekers
er komen, maar ook waarop ze je vonden.

**Werkt dit voor klantsites?**
Ja, mits je account toegang heeft. Werk per klant in een
[project](../functies/projecten.md).

**Is dit hetzelfde als de SEO Engine?**
Nee. Analytics vertelt wat er gebeurde; de [SEO Engine](seo-engine.md) vertelt
wat je kunt verbeteren.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Search Console](google-search-console.md) · [SEO Engine](seo-engine.md) · [Weekrapport](weekly-report.md)
→ Op de site: [de vijf Growth Engines](https://dgenix.nl/engines) · [gratis scan](https://dgenix.nl/demo)

*dGENIX Docs, Google Analytics, bijgewerkt augustus 2026*
