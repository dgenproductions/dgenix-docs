# Dagplanner & Life Assistant

Met de Dagplanner maakt GENI een overzicht van je dag, ordent hij je taken op prioriteit en zet hij terugkerende taken voor je klaar.

Beschikbaar vanaf **Starter**. Je hebt geen koppeling nodig, maar met Google
Calendar erbij wordt het overzicht compleet.

## Wat kan GENI hiermee?

- **Een dagoverzicht maken** voor vandaag of een andere datum, inclusief je afspraken als Google Calendar gekoppeld is
- **Taken prioriteren** op urgentie, impact en de tijd die je hebt
- **Je terugkerende taken tonen**
- **Een terugkerende taak aanmaken** (dagelijks, wekelijks of maandelijks, op een vast tijdstip)
- **Een terugkerende taak aanpassen** of tijdelijk uitzetten
- **Een terugkerende taak verwijderen**

Let op het verschil: de eerste twee gaan over jouw dag, de laatste vier beheren
**Automations** , taken die GENI zelf uitvoert op een vast moment. Zie
[Geplande taken](../handleiding/geplande-taken.md).

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Hoe ziet mijn dag eruit?
```

> **Woensdag 5 augustus**
>
> **Vast in de agenda**
> - 09:30-10:00 , Standup
> - 14:00-15:00 , Klantgesprek De Krent
> - 16:30-17:00 , Belafspraak leverancier
>
> **Je hebt twee blokken vrij:** 10:00-14:00 en 15:00-16:30
>
> **Wat er ligt**
> - Offerte De Krent afmaken , vóór het gesprek van 14:00, dus in het ochtendblok
> - Factuur 2026-084 versturen , 10 minuten, kan tussendoor
> - Kwartaalplan schrijven , past niet meer vandaag, morgenochtend
>
> Zal ik je ochtendblok op de offerte zetten?

En bij een terugkerende taak:

```
Stuur me elke maandag om 8 uur een samenvatting van mijn week
```

> Klaar. **Weekstart-samenvatting**, elke maandag om 08:00.
> Je vindt hem terug bij Automations, daar kun je hem ook pauzeren.

## Vereisten

- **Plan:** Starter en hoger
- **Koppeling:** geen. [Google Calendar](google-calendar.md) is optioneel maar sterk aanbevolen

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Dagplanner & Life Assistant**
2. Koppel eventueel Google Calendar via **Dashboard → Connectors**
3. Vraag om een dagoverzicht

## Wat het kost

| Actie | Credits |
|---|---|
| Elke dagplanner-actie | 3 |

Dat is de goedkoopste skill van het platform. Bovenop die 3 credits komt het
gesprek zelf; zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Zonder Google Calendar kent GENI je afspraken niet.** Het overzicht gaat dan alleen over wat je hem vertelt en over je taken.
- **Een dagindeling is een voorstel**, geen agenda-wijziging. Vraag [Google Calendar](google-calendar.md) om het echt in te plannen.
- **Terugkerende taken tellen mee in je slots**: Free 0, Starter 1, Growth 5, Pro 10, Business 20.
- **Het kortste interval is dagelijks.** Meerdere keren per dag kan niet.
- **Prioriteren gaat op wat je aanlevert.** GENI kent je stille deadlines niet als je ze niet noemt of opslaat in je [geheugen](../functies/geheugen.md).

## Problemen oplossen

**Mijn afspraken staan er niet bij.** Google Calendar is niet gekoppeld, of het overzicht gaat over een andere dag. Noem de datum expliciet.

**De prioritering slaat nergens op.** Geef context mee: harde deadlines, hoeveel tijd je hebt, en hoe veeleisend het werk is.

**Mijn terugkerende taak draait niet.** Kijk bij Automations of hij aan staat en of je nog slots vrij hebt; bij te weinig credits wordt hij gepauzeerd.

**Hij maakt een taak aan terwijl ik alleen een overzicht wilde.** Zeg "laat zien" of "geef een overzicht" in plaats van "zet klaar".

## Veelgestelde vragen

**Wat is het verschil met de Werkruimte?**
De [Werkruimte](../functies/werkruimte.md) is waar je notities en to-do's
bewaart. De Dagplanner kijkt naar je dag en ordent wat er ligt.

**Onthoudt hij mijn werkritme?**
Als je het vertelt wel. Zeg bijvoorbeeld dat je 's ochtends het scherpst bent,
dan slaat GENI dat op in je geheugen en houdt hij er rekening mee.

**Kan hij mijn afspraken verzetten?**
Niet vanuit deze skill. Met [Google Calendar](google-calendar.md) erbij wel, en
dan vraagt hij eerst om bevestiging.

**Werkt dit ook via Telegram?**
Ja, als je de Telegram add-on gebruikt. Een dagoverzicht om 8 uur op je telefoon
is een veelgebruikte automation.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Calendar](google-calendar.md) · [Geplande taken](../handleiding/geplande-taken.md) · [Werkruimte](../functies/werkruimte.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Dagplanner & Life Assistant, bijgewerkt augustus 2026*
