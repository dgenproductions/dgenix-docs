# YouTube koppelen

De YouTube-connector geeft GENI leestoegang tot je kanaal, zodat hij statistieken kan ophalen, reacties kan analyseren en op basis daarvan video-ideeën en uploadchecklists maakt.

## Wat je hiermee kunt

| Wat GENI doet | Voorbeeld |
|---|---|
| Kanaalstatistieken ophalen | "Hoe deed mijn kanaal deze maand?" |
| Statistieken per video | "Hoeveel kijktijd had mijn laatste video?" |
| Reacties analyseren | "Welke vragen komen terug onder mijn laatste 3 video's?" |
| Analytics-rapport | "Maak een rapport over kijktijd, CTR en verkeersbronnen" |
| Doelgroep-inzichten | "Wanneer kan ik het beste uploaden?" |
| Video-ideeën genereren | "Geef me 10 ideeën die passen bij mijn best presterende content" |
| Uploadchecklist maken | "Maak een SEO-titel, beschrijving en tags voor deze video" |

De koppeling activeert de **[YouTube Manager-skill](../skills/youtube.md)**, beschikbaar vanaf Growth.

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast YouTube Manager
3. Log in met het Google-account dat aan je YouTube-kanaal gekoppeld is
4. Geef dGENIX de gevraagde rechten (YouTube én Analytics)
5. Het venster sluit vanzelf, de koppeling is direct actief

> Had je YouTube al eerder gekoppeld? Verbreek de verbinding en koppel opnieuw.
> De Analytics-rechten zijn later toegevoegd, dus oudere koppelingen missen het
> analytics-rapport en de doelgroep-inzichten.

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| YouTube-kanaaldata lezen | Statistieken, video's en kanaalinfo ophalen |
| YouTube Analytics lezen | Kijktijd, CTR, verkeersbronnen en uploadtijden |

De koppeling is **alleen-lezen**. dGENIX uploadt geen video's, wijzigt geen
titels of beschrijvingen en plaatst geen reacties.

## Controleren of het werkt

Vraag GENI na het koppelen:

```
Hoe presteerde mijn YouTube-kanaal de afgelopen 30 dagen?
```

Je krijgt abonnees, weergaven en je recente video's terug. Krijg je een melding
over ontbrekende rechten bij het analytics-rapport, dan is de koppeling gemaakt
vóór de Analytics-rechten bestonden: opnieuw koppelen lost dat op.

## Grenzen

- Alleen-lezen: uploaden, bewerken en reageren doet GENI niet
- Eén kanaal per gekoppeld Google-account
- Analytics-data loopt bij YouTube zelf een paar dagen achter
- Reacties worden geanalyseerd op thema's, niet beantwoord

## Problemen oplossen

**Koppeling mislukt.** Controleer of je bent ingelogd op het Google-account dat eigenaar is van het kanaal. Een merkaccount vraagt om het bijbehorende beheerdersaccount.

**Analytics-rapport geeft een rechtenfout.** De koppeling dateert van vóór de Analytics-rechten. Verbreek en koppel opnieuw.

**GENI ziet het verkeerde kanaal.** Je Google-account beheert meerdere kanalen. Verbreek de verbinding en kies bij het opnieuw koppelen expliciet het juiste kanaal.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op YouTube Manager en kies **Verbreken**.
Je kunt de toegang ook intrekken bij Google zelf via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Veelgestelde vragen

**Kan GENI video's voor me uploaden?**
Nee. De koppeling is bewust alleen-lezen; je houdt zelf de controle over wat er op je kanaal verschijnt.

**Werkt dit voor een merkaccount (brand account)?**
Ja, mits je koppelt met het Google-account dat beheerder is van dat merkaccount.

**Heb ik hiervoor ook de YouTube-skill nodig?**
Ja. De connector regelt de toegang, de skill geeft GENI de mogelijkheden. Activeer die via **Dashboard → Skills**.

**Kan GENI van mijn video's ook shorts maken?**
Dat doet een andere skill. De [AI Content Engine](https://dgenix.nl/engines/ai-content) knipt een
lange video in clips met een viraliteitsscore; deze connector gaat over de
statistieken van je kanaal.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [YouTube Manager skill](../skills/youtube.md)

*dGENIX Docs, YouTube koppelen, bijgewerkt augustus 2026*
