# Canva koppelen

De Canva-koppeling laat GENI designs zoeken, aanmaken uit je brand templates en exporteren als PNG, PDF of MP4.

> **Binnenkort beschikbaar.** De koppeling is gebouwd, maar wacht op goedkeuring
> van het Developer API-programma van Canva. Zodra die er is, staat Canva in je
> Connectors-lijst; je hoeft niets voor te bereiden.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Welke designs heb ik al voor de zomeractie?" | Doorzoekt je bestaande designs |
| "Welke brand templates hebben we?" | Geeft de beschikbare merksjablonen |
| "Maak een leeg Instagram-formaat aan" | Maakt een nieuw design in het gevraagde formaat |
| "Vul de aanbiedingssjabloon met deze tekst en prijs" | Vult een brand template automatisch in |
| "Exporteer dat design als PDF" | Levert een downloadbaar bestand |

Het invullen van **brand templates** is waar dit interessant wordt: één sjabloon
plus wisselende tekst levert een reeks visuals die er allemaal hetzelfde
uitzien.

## Koppelen (zodra beschikbaar)

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast Canva
3. Log in met je Canva-account en geef toegang
4. De [Canva-skill](../skills/canva.md) is direct actief

De skill valt onder **Starter** en hoger.

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| Designs lezen | Je bestaande designs doorzoeken |
| Brand templates lezen | Beschikbare sjablonen ophalen |
| Designs aanmaken | Een nieuw of ingevuld design maken |
| Exporteren | Een design als bestand ophalen |

## Controleren of het werkt

Vraag na het koppelen:

```
Welke Canva-designs kan je zien?
```

Je krijgt een lijst met de titels van je designs terug.

## Grenzen

- GENI bewerkt geen bestaand design; hij maakt een **nieuw** design of vult een template
- Vrije vormgeving kan niet, alleen wat een brand template ondersteunt
- Exporteren van een groot of complex design duurt langer; GENI wacht het af en meldt het resultaat
- Designs worden nooit verwijderd
- Brand templates vragen mogelijk om een betaald Canva-plan

## Problemen oplossen

**Canva staat niet in Connectors.** De koppeling is nog niet vrijgegeven. Zie de melding bovenaan deze pagina.

**Er zijn geen brand templates.** Die zitten in Canva's betaalde plannen. Zonder templates kun je wel lege designs aanmaken en exporteren.

**Een export lijkt te blijven hangen.** Canva verwerkt de export op de achtergrond; bij een zwaar design duurt dat langer. GENI meldt zich zodra het bestand klaar is.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Canva en kies **Verbreken**. In
Canva kun je de toegang ook intrekken via je accountinstellingen.

## Veelgestelde vragen

**Wanneer komt de koppeling beschikbaar?**
Dat hangt af van de goedkeuring door Canva. We hebben er geen invloed op; zodra
het rond is, verschijnt de koppeling vanzelf in je dashboard.

**Is dit hetzelfde als AI-beeldgeneratie?**
Nee. Beeldgeneratie maakt een nieuwe afbeelding uit een beschrijving; Canva
werkt met jouw eigen sjablonen en huisstijl. Zie
[AI Beeldgeneratie](../skills/ai-beeldgeneratie.md).

**Kan GENI zelf een campagne opmaken?**
Hij kan een reeks designs uit een template vullen. De vormgeving van dat
sjabloon maak je in Canva.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Canva skill](../skills/canva.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Canva koppelen, bijgewerkt augustus 2026*
