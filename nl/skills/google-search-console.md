# Google Search Console

Met de Search Console-skill haalt GENI je échte Google-data op: op welke zoekwoorden je gevonden wordt, hoeveel klikken dat oplevert en waar je net buiten de top staat.

Dit is geen schatting maar je eigen meetdata. Beschikbaar vanaf **Growth**. Je
hebt een gekoppeld Google-account nodig met toegang tot de property.

## Wat kan GENI met Search Console?

- **Een zoekwoordenrapport** met klikken, vertoningen, CTR en gemiddelde positie
- **Pagina-prestaties**: welke pagina's de meeste organische klikken opleveren
- **SEO-kansen**: zoekwoorden die net buiten de top staan, met AI-aanbevelingen

Die laatste is waar het interessant wordt: positie 11 tot 20 betekent dat je al
meetelt maar net niet gevonden wordt, en dat is meestal de goedkoopste winst.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Waar liggen mijn SEO-kansen?
```

> **3 zoekwoorden net buiten de eerste pagina**
>
> | Zoekwoord | Positie | Vertoningen | Klikken |
> |---|---|---|---|
> | warmtepomp installateur eindhoven | 11 | 1.240 | 18 |
> | warmtepomp subsidie aanvragen | 13 | 890 | 7 |
> | kosten warmtepomp woning | 14 | 2.100 | 11 |
>
> Het derde zoekwoord heeft de meeste vertoningen en de laagste CTR. Je pagina
> daarover is dun en beantwoordt de vraag niet direct in de eerste alinea.
> Twee posities winst hier is meer waard dan tien posities op de rest.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een Google-account dat toegang heeft tot de Search Console-property

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Search Console**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Doorloop het Google-toestemmingsscherm
4. Search Console is direct bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| Pagina-prestaties | 35 |
| Zoekwoordenrapport | 50 |
| SEO-kansen met aanbevelingen | 450 |

De laatste is duurder omdat er een uitgebreide analyse aan te pas komt. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Je ziet alleen properties waar jouw account toegang toe heeft.**
- **Search Console-data loopt twee tot drie dagen achter.** Dat is Google's vertraging, niet die van ons.
- **Zoekwoorden met weinig verkeer worden door Google weggelaten** uit privacyoverwegingen; die kan niemand zien.
- **De skill wijzigt niets aan je site.** Hij leest en adviseert.
- **Geen historische data van vóór je koppeling.** Google bewaart standaard 16 maanden.

## Problemen oplossen

**Er komt geen data.** De property is niet geverifieerd in Search Console, of jouw account heeft er geen rechten op. Controleer dat eerst in Search Console zelf.

**De cijfers wijken af van je analytics.** Dat hoort: Search Console telt vertoningen en klikken in Google, [Analytics](google-analytics.md) telt bezoeken op je site. Verschillen van tientallen procenten zijn normaal.

**Een nieuwe pagina staat er niet bij.** Google moet hem eerst indexeren en er moet verkeer op zitten. Reken op enkele weken.

**Je ziet minder zoekwoorden dan verwacht.** Google filtert zeldzame zoekopdrachten weg.

## Veelgestelde vragen

**Wat is het verschil met de SEO Engine?**
Deze skill toont je eigen Google-data: waar je nú op gevonden wordt. De
[SEO Engine](seo-engine.md) analyseert je pagina's en zegt wat je moet
verbeteren. Samen zijn ze sterker: meten waar de kans zit, dan verbeteren.

**Kan ik dit maandelijks laten rapporteren?**
Ja, als geplande taak met de uitkomst per mail. Zie
[Geplande taken](../handleiding/geplande-taken.md).

**Werkt dit voor klantsites?**
Ja, mits je account toegang heeft tot hun property. Werk per klant in een
[project](../functies/projecten.md).

**Heb ik hier de SEO Engine ook nog voor nodig?**
Niet per se. Deze skill is gratis data uit je eigen Google-account; de engine
voegt analyse en concurrentievergelijking toe.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Analytics](google-analytics.md) · [SEO Engine](seo-engine.md) · [Authority Engine](authority-engine.md)
→ Op de site: [de vijf Growth Engines](https://dgenix.nl/engines) · [gratis scan](https://dgenix.nl/demo)

*dGENIX Docs, Google Search Console, bijgewerkt augustus 2026*
