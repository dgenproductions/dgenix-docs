# Calendly

Met de Calendly-skill vraagt GENI je afspraaktypen, geplande afspraken en vrije tijdsloten op, zodat je niet hoeft te schakelen tussen agenda's.

Beschikbaar vanaf **Growth**. Je hebt een gekoppeld Calendly-account nodig.

## Wat kan GENI met Calendly?

- **Je afspraaktypen opsommen**, bijvoorbeeld kennismaking, adviesgesprek, demo
- **Aankomende afspraken ophalen**
- **Beschikbare tijdsloten opvragen** voor een specifiek afspraaktype

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Wat staat er deze week aan gesprekken gepland?
```

> **5 afspraken via Calendly**
>
> | Wanneer | Type | Met |
> |---|---|---|
> | Ma 09:00 | Kennismaking (30 min) | Sanne de Wit |
> | Di 14:00 | Adviesgesprek (60 min) | Bakkerij De Krent |
> | Wo 11:00 | Kennismaking (30 min) | Mark Jansen |
> | Do 10:30 | Demo (45 min) | Studio Noord |
> | Vr 15:00 | Adviesgesprek (60 min) | Van Dijk BV |
>
> Donderdag is je enige dag met een vrij blok in de ochtend. Zal ik de
> voorbereiding voor het adviesgesprek van dinsdag klaarzetten?

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een Calendly-account via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Calendly**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Vraag naar je afspraken, types of beschikbaarheid

## Wat het kost

Dit zijn lichte leesacties; ze kosten een klein aantal credits per opvraging. Het
bedrag staat op de knop voordat je start. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Alleen lezen.** GENI plant geen Calendly-afspraken in en verzet of annuleert ze niet.
- **Geen afspraaktypen aanmaken of aanpassen.** Dat doe je in Calendly.
- **Geen uitnodigingen versturen.** Je deelt je Calendly-link zelf.
- **Aankomende afspraken**, geen volledige historie.
- **Wil je zelf iets inplannen**, gebruik dan [Google Calendar](google-calendar.md); die kan wel afspraken aanmaken.

## Problemen oplossen

**Er komen geen afspraken.** Er staan er geen gepland in de opgehaalde periode, of het gekoppelde account is niet degene die de afspraken ontvangt.

**Een afspraaktype ontbreekt.** Controleer of het actief staat in Calendly; verborgen types worden niet getoond.

**De beschikbaarheid klopt niet met je gevoel.** Calendly rekent met je ingestelde werkuren en buffers. Pas die daar aan.

**Je wilt een afspraak verzetten.** Dat gaat via Calendly zelf of via de klant; GENI kan het niet.

## Veelgestelde vragen

**Kan GENI mijn dag samenvatten inclusief Calendly?**
Ja, in combinatie met [Google Calendar](google-calendar.md) en
[Gmail](gmail.md) krijg je één dagoverzicht in plaats van drie schermen.

**Kan ik dit inplannen?**
Ja, bijvoorbeeld elke maandag een overzicht van je week. Zie
[Geplande taken](../handleiding/geplande-taken.md).

**Kan hij zich voorbereiden op een gesprek?**
Ja, gecombineerd met [Lead Research](lead-research.md) zoekt hij uit wie je
spreekt voordat je aan tafel zit.

**Wat is het verschil met Google Calendar?**
Calendly gaat over afspraken die anderen bij jou boeken. Google Calendar is je
eigen agenda, waar GENI ook in kan plannen.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Calendar](google-calendar.md) · [Lead Research](lead-research.md) · [Dagplanner](dagplanner.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Calendly, bijgewerkt augustus 2026*
