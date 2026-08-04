# LinkedIn

Met de LinkedIn-skill schrijft en publiceert GENI posts op je profiel, en haalt hij de cijfers van je recente posts op.

Beschikbaar vanaf **Growth**. Je hebt een gekoppeld LinkedIn-profiel nodig; zie
[LinkedIn koppelen](../connectors/linkedin.md).

## Wat kan GENI met LinkedIn?

- **Een tekstpost publiceren** op je profiel
- **Je profiel lezen**: naam, headline en profielfoto
- **Statistieken ophalen** van je recente posts: weergaven, likes en reacties

De waarde zit vooral in het combineren: laat GENI een blogartikel, een
weekrapport of een case omzetten naar een post die bij je toon past.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Maak een LinkedIn-post van mijn laatste blogartikel
```

> **Concept, 142 woorden**
>
> Vorige week belde een klant met een vraag die ik vaker hoor: "waarom staan we
> niet in ChatGPT als iemand naar ons vakgebied vraagt?"
>
> Het antwoord bleek pijnlijk simpel. Hun robots.txt blokkeerde precies de bots
> die hen hadden kunnen citeren. Al twee jaar.
>
> Drie dingen die ik sindsdien bij elke site check: […]
>
> **Geschatte leestijd:** 40 seconden. Geen hashtags, die doen op LinkedIn
> weinig meer.
>
> Zal ik hem publiceren?

En achteraf:

```
Hoe deden mijn laatste posts het?
```

> | Post | Weergaven | Reacties |
> |---|---|---|
> | "De fout die me 40.000 kostte" | 4.820 | 31 |
> | "Waarom AI je niet noemt" | 2.140 | 12 |
> | "Drie jaar ondernemen" | 890 | 4 |
>
> Persoonlijke verhalen halen hier ruim vijf keer zoveel bereik als algemene
> tips.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een LinkedIn-profiel via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **LinkedIn**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Log in bij LinkedIn en geef toestemming
4. LinkedIn is direct bruikbaar

> **Let op:** LinkedIn moet het publiceren-recht goedkeuren via hun Developer
> Program, wat 1 tot 2 weken kan duren. Je profiel lezen en statistieken
> ophalen werkt direct.

## Wat het kost

| Actie | Credits |
|---|---|
| Statistieken opvragen | ~40 |
| Post schrijven en publiceren | ~120 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Publiceren vraagt altijd om bevestiging.** Je leest de tekst eerst.
- **Alleen tekstposts.** Afbeeldingen, video's, documenten en carrousels kunnen niet.
- **Alleen je persoonlijke profiel.** Posten op een bedrijfspagina wordt niet ondersteund.
- **GENI bewerkt of verwijdert geen bestaande posts.**
- **Geen reacties, connectieverzoeken of berichten.** Deze skill raakt je inbox en netwerk niet.
- **Statistieken komen met vertraging.** Voor een verse post is een leeg resultaat normaal.

## Problemen oplossen

**Publiceren geeft een rechtenfout.** Het publiceren-recht is nog niet goedgekeurd door LinkedIn. Lezen werkt al wel; publiceren komt beschikbaar zodra zij akkoord geven.

**Statistieken zijn leeg.** LinkedIn levert cijfers pas na enige tijd.

**Je wilt op je bedrijfspagina posten.** Dat ondersteunt de koppeling niet. Laat GENI de tekst schrijven en plaats hem zelf.

**De toon klopt niet.** Leg je schrijfstijl vast in [Instellingen](../functies/instellingen.md) of in je [geheugen](../functies/geheugen.md), dan houdt GENI zich daaraan.

## Veelgestelde vragen

**Kan GENI wekelijks automatisch posten?**
Ja, als geplande taak. Ook dan zie je de tekst eerst; er gaat nooit iets
ongezien de deur uit. Zie [Geplande taken](../handleiding/geplande-taken.md).

**Kan hij een blog omzetten naar een post?**
Ja, dat is de meest gebruikte combinatie. Zie ook
[Content Repurposing](content-repurposing.md).

**Ziet hij mijn inbox of connecties?**
Nee. De koppeling geeft daar geen toegang toe.

**Wat is het verschil met de Social Media Manager?**
Die plant content over meerdere kanalen. Deze skill is specifiek voor LinkedIn,
inclusief de cijfers achteraf. Zie [Social Media Manager](social-media.md).

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [LinkedIn koppelen](../connectors/linkedin.md) · [Content Repurposing](content-repurposing.md) · [Social Media Manager](social-media.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, LinkedIn, bijgewerkt augustus 2026*
