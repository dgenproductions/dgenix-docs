# AI Receptionist

Met de AI Receptionist leg je je veelgestelde vragen één keer vast, waarna GENI klantvragen daaruit beantwoordt in de toon die jij instelt.

Beschikbaar vanaf **Pro**. Je hebt geen koppeling nodig.

## Wat kan GENI hiermee?

- **Je FAQ instellen** , bedrijfsnaam, vraag-en-antwoordparen, communicatietoon en extra bedrijfsinformatie zoals openingstijden en adres
- **Een klantvraag beantwoorden** op basis van die FAQ
- **Een klantgesprek samenvatten** met de actiepunten eruit

Het verschil met gewoon vragen: hij antwoordt uit **jouw** antwoorden, niet uit
algemene kennis.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

Eerst instellen:

```
Stel mijn FAQ in voor Bakkerij De Krent, toon: vriendelijk

V: Zijn jullie op zondag open?
A: Ja, van 8:00 tot 13:00.

V: Kan ik een taart bestellen?
A: Ja, minimaal 3 dagen vooraf, telefonisch of aan de balie.
```

> FAQ ingesteld voor **Bakkerij De Krent**, 2 items, toon vriendelijk.
> Openingstijden en adres heb ik nog niet; die vragen klanten meestal als eerste.

Daarna beantwoorden:

```
Een klant vraagt: hebben jullie glutenvrij brood?
```

> Daar staat niets over in je FAQ, dus ik verzin geen antwoord.
>
> Voorstel voor als het klopt:
> > "Ja, we hebben dagelijks glutenvrij brood. Het is beperkt beschikbaar, dus
> > bestel je het van tevoren, dan leggen we het voor je apart."
>
> Zal ik hem aan je FAQ toevoegen?

## Vereisten

- **Plan:** Pro en hoger
- **Koppeling:** geen

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **AI Receptionist**
2. Stel je FAQ in met je veelgestelde vragen en toon
3. Stel een klantvraag om te testen

## Wat het kost

| Actie | Credits |
|---|---|
| FAQ instellen of bijwerken | 5 |
| Vraag beantwoorden | 3 |
| Gesprek samenvatten | 5 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Hij neemt de telefoon niet op.** Er is geen telefonie-koppeling; dit is een tekstlaag voor jou en je team.
- **Hij praat niet zelf met klanten.** Er staat geen chatwidget op je site; jij plakt het antwoord, of koppelt [WhatsApp Business](whatsapp-business.md).
- **Buiten je FAQ verzint hij niets.** Dat is opzet: een gokje richting een klant is erger dan geen antwoord.
- **Geen afspraken inplannen.** Daarvoor koppel je [Google Calendar](google-calendar.md) of [Calendly](calendly.md).
- **Bijwerken doe je zelf.** Wijzigen je openingstijden, dan pas je de FAQ aan.

## Problemen oplossen

**Hij zegt dat het antwoord er niet is.** Klopt, en dat is de bedoeling. Voeg de vraag toe aan je FAQ.

**De toon past niet.** Stel hem opnieuw in met een duidelijke omschrijving, bijvoorbeeld "kort en zakelijk" of "warm, tutoyeren".

**De FAQ komt niet goed binnen.** Gebruik het formaat `V:` en `A:` met een lege regel tussen de items.

**Klanten vragen steeds hetzelfde wat er niet in staat.** Analyseer een week aan vragen en voeg de top vijf toe; dat scheelt de meeste tijd.

## Veelgestelde vragen

**Kan hij zelf op mijn website antwoorden?**
Nee, er is geen widget. Wel kun je hem via
[WhatsApp Business](whatsapp-business.md) op je zakelijke WhatsApp laten
meelezen.

**Wat is het verschil met de Support Kennisbank?**
[Die](knowledge-base.md) doorzoekt je hele documentatie en noemt de bron. De AI
Receptionist werkt met een korte, handmatig ingestelde FAQ en een vaste toon.

**Kan ik meerdere bedrijven instellen?**
Eén FAQ per keer. Werk je voor meerdere klanten, gebruik dan een
[project](../functies/projecten.md) per klant.

**Kan hij gesprekken samenvatten uit WhatsApp?**
Ja, plak het gesprek en vraag om een samenvatting met actiepunten.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Support Kennisbank](knowledge-base.md) · [WhatsApp Business](whatsapp-business.md) · [Projecten](../functies/projecten.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, AI Receptionist, bijgewerkt augustus 2026*
