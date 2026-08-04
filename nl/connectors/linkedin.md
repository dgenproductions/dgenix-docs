# LinkedIn koppelen

De LinkedIn-koppeling laat GENI posts publiceren op jouw profiel en de statistieken van je recente posts ophalen.

De koppeling activeert de [LinkedIn-skill](../skills/linkedin.md), beschikbaar
vanaf **Growth**.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Publiceer deze tekst op LinkedIn" | Plaatst een tekstpost op je profiel |
| "Schrijf een post over ons nieuwe product en zet hem klaar" | Schrijft de tekst en vraagt eerst om akkoord |
| "Hoe deden mijn laatste posts het?" | Haalt views, likes en reacties op |
| "Wat staat er in mijn profiel?" | Leest naam, headline en profielfoto-URL |

Het combineren met andere skills is waar dit interessant wordt: laat GENI een
blogartikel omzetten naar een LinkedIn-post, of een weekrapport samenvatten tot
één bericht.

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast LinkedIn
3. Log in met je LinkedIn-account
4. Geef de gevraagde toegangsrechten
5. LinkedIn staat daarna op **Verbonden**

## Welke toegang je geeft

| Scope | Waarvoor dGENIX het gebruikt |
|---|---|
| `r_liteprofile` | Je naam, headline en profielfoto lezen |
| `r_emailaddress` | Je e-mailadres opvragen |
| `w_member_social` | Posts publiceren op jouw profiel |

> **Let op:** LinkedIn moet de `w_member_social`-scope goedkeuren via hun
> Developer Program. Dat kan 1 tot 2 weken duren. Je profiel lezen en
> statistieken ophalen werkt direct na het koppelen.

## Controleren of het werkt

Vraag direct na het koppelen:

```
Wat staat er in mijn LinkedIn-profiel?
```

Je krijgt je naam en headline terug. Werkt dat, dan staat de leeskant goed. Of
publiceren werkt, hangt af van de goedkeuring hierboven.

## Grenzen

- Een post publiceren vraagt **altijd** om bevestiging; je leest de tekst eerst
- Alleen tekstposts; afbeeldingen, video's en documenten kunnen niet
- Posten op een **bedrijfspagina** kan niet, alleen op je persoonlijke profiel
- GENI verwijdert of bewerkt geen bestaande posts
- Reageren op posts van anderen en connectieverzoeken sturen kan niet

## Problemen oplossen

**Publiceren geeft een rechtenfout.** De `w_member_social`-scope is nog niet goedgekeurd. Lezen werkt al wel; publiceren komt beschikbaar zodra LinkedIn akkoord geeft.

**Statistieken zijn leeg.** LinkedIn levert cijfers pas na enige tijd. Voor een verse post is dat normaal.

**Je wilt op je bedrijfspagina posten.** Dat ondersteunt deze koppeling niet. Laat GENI de tekst schrijven en plaats hem zelf.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op LinkedIn en kies **Verbreken**. In
LinkedIn kun je de toegang ook intrekken via *Instellingen → Gegevensprivacy →
Andere toepassingen*.

## Veelgestelde vragen

**Kan GENI automatisch elke week posten?**
Ja, via een herhaalde taak. Ook dan geldt de bevestiging, dus er gaat nooit iets
de deur uit dat je niet gezien hebt. Zie [Geplande taken](../handleiding/geplande-taken.md).

**Ziet GENI mijn inbox of connecties?**
Nee. De koppeling geeft geen toegang tot berichten, connecties of je feed.

**Kan ik zelf de toon bepalen?**
Ja. Zet in je kennisdocument of geheugen hoe je wilt schrijven, dan houdt GENI
zich daaraan. Zie [Contextopslag vergeleken](../concepten/context-opslag-vergeleken.md).

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [LinkedIn skill](../skills/linkedin.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, LinkedIn koppelen, bijgewerkt augustus 2026*
