# Notion koppelen

De Notion-koppeling geeft GENI toegang tot de pagina's en databases die jij selecteert, zodat hij daar kan lezen, schrijven en zoeken.

Notion werkt anders dan de meeste koppelingen: je geeft geen toegang tot je hele
werkruimte, maar **kiest zelf welke pagina's je deelt**. De koppeling activeert
de [Notion-skill](../skills/notion.md), beschikbaar vanaf **Growth**.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Zet de notulen van vandaag in Notion" | Maakt een nieuwe pagina aan |
| "Voeg de conclusies toe aan de projectpagina" | Werkt een bestaande pagina bij |
| "Waar staat onze onboarding-checklist?" | Zoekt in de gedeelde pagina's en databases |
| "Wat staat er in het meetingverslag van maandag?" | Leest de inhoud van een pagina |
| "Maak een rij aan in mijn klantendatabase" | Maakt een pagina aan in die database |

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast Notion
3. Log in met je Notion-account
4. **Selecteer de pagina's en databases** die je wilt delen
5. Klik op **Toegang geven**; Notion staat daarna op **Verbonden**

Stap 4 is de belangrijkste. Selecteer je niets, dan is de koppeling actief maar
kan GENI nergens bij.

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| Lezen van geselecteerde pagina's | Inhoud ophalen en doorzoeken |
| Inhoud toevoegen | Nieuwe pagina's of database-rijen aanmaken |
| Inhoud bijwerken | Tekst toevoegen aan een bestaande pagina |

De toegang geldt **alleen voor wat je in stap 4 hebt aangevinkt**, inclusief de
sub-pagina's daaronder. Al het andere in je werkruimte blijft buiten bereik.

## Controleren of het werkt

Vraag direct na het koppelen:

```
Welke Notion-pagina's kan je zien?
```

Krijg je een lege lijst terug, dan heb je bij het koppelen geen pagina's
geselecteerd. Herhaal de koppeling en vink deze keer wel iets aan.

## Grenzen

- GENI ziet **alleen** de pagina's die je expliciet deelde
- Pagina's toevoegen kan niet achteraf vanuit dGENIX; je verbreekt de koppeling en autoriseert opnieuw
- GENI verwijdert nooit pagina's of database-rijen
- Een pagina aanmaken of bijwerken vraagt om bevestiging
- Zeer lange pagina's worden gedeeltelijk gelezen; vraag gericht naar een sectie voor een beter resultaat

## Problemen oplossen

**GENI vindt een pagina niet die wel bestaat.** Die pagina is niet gedeeld. Verbreek de koppeling en selecteer hem alsnog.

**Een nieuwe pagina verschijnt niet waar je hem verwacht.** Zonder aangewezen locatie plaatst Notion hem in de eerste gedeelde pagina. Noem de doelpagina of database in je opdracht.

**Je wilt een database toevoegen.** Databases moet je apart aanvinken; de bovenliggende pagina delen is niet genoeg.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Notion en kies **Verbreken**. In
Notion kun je de toegang ook intrekken via *Instellingen → Verbindingen*.

## Veelgestelde vragen

**Kan GENI bij mijn hele Notion-werkruimte?**
Nee, en dat is precies het verschil met de meeste koppelingen. Notion vraagt je
per pagina om toestemming; dGENIX krijgt niet meer dan dat.

**Kan ik later meer pagina's toevoegen?**
Ja, maar dat gaat via de autorisatie van Notion: verbreek de koppeling in
dGENIX en koppel opnieuw met een ruimere selectie.

**Werkt dit met een gratis Notion-account?**
Ja. De koppeling gebruikt de standaard-integratiemogelijkheden van Notion.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Notion skill](../skills/notion.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Notion koppelen, bijgewerkt augustus 2026*
