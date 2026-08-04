# WhatsApp Business

Met de WhatsApp Business-skill leest GENI je zakelijke inbox en stelt hij antwoorden op, zodat je niet de hele dag achter je telefoon hoeft te zitten.

Beschikbaar vanaf **Growth**. Je hebt een nummer op de WhatsApp Business API
nodig; zie [WhatsApp Business koppelen](../connectors/whatsapp-business.md).

## Wat kan GENI met WhatsApp Business?

- **Je Business-inbox lezen** en de recente inkomende berichten ophalen
- **Een bericht versturen** vanaf je zakelijke nummer

In de praktijk betekent dat: laat je binnengekomen vragen samenvatten, zie welke
er echt om actie vragen, en laat de antwoorden opstellen.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Wat is er binnengekomen op WhatsApp?
```

> **9 berichten sinds gisteren, 4 vragen actie**
>
> - **+31 6 12…** , vraagt of je zaterdag open bent. *Komt vaker terug.*
> - **+31 6 44…** , wil de offerte van vorige week nog ontvangen.
> - **+31 6 78…** , meldt een storing aan de installatie van maart. *Urgent.*
> - **+31 6 21…** , vraagt naar prijzen voor onderhoud.
>
> De overige 5 zijn bedankjes en bevestigingen.
>
> De storing zou ik als eerste oppakken. Zal ik een antwoord opstellen?

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** een nummer op de WhatsApp Business API, via Meta
- Een **Meta Developer-account** met een goedgekeurde app

Een gewoon WhatsApp- of WhatsApp Business-**app**-account is niet genoeg.

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **WhatsApp Business**
2. Ga naar **Dashboard → Connectors** en voer je Meta-gegevens in
3. Stel de webhook in bij Meta, anders ontvang je geen berichten
4. WhatsApp Business is bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| Berichten lezen en samenvatten | ~50 |
| Bericht opstellen en versturen | ~80 |

Meta rekent daarnaast zijn eigen gesprekskosten; die lopen via je Meta-account
en staan los van je credits. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Versturen vraagt om bevestiging.** Je leest de tekst voordat hij weggaat.
- **Meta staat vrije tekst alleen toe binnen 24 uur** na het laatste bericht van de klant. Daarbuiten is een goedgekeurde sjabloon nodig.
- **Alleen tekst.** Afbeeldingen, documenten en spraakberichten versturen kan niet.
- **Geen groepsgesprekken.**
- **GENI verwijdert geen berichten en blokkeert geen contacten.**
- **Zonder webhook geen inkomende berichten**, ook al werkt versturen wel.

## Problemen oplossen

**Er komen geen berichten binnen.** De webhook staat niet goed. Controleer de URL, het Verify Token en of je op `messages` bent geabonneerd.

**Versturen faalt buiten kantooruren.** Waarschijnlijk is het 24-uursvenster verlopen. Gebruik dan een in Meta goedgekeurde sjabloon.

**Het token verloopt steeds.** Meta geeft standaard tijdelijke tokens uit. Maak een permanent systeemgebruiker-token aan.

**Meta keurt je app niet goed.** Zonder goedgekeurde app werkt de API niet. Dat loopt volledig via Meta.

## Veelgestelde vragen

**Antwoordt GENI automatisch op alles?**
Alleen als je dat expliciet inplant. Standaard leest hij en beslis jij wat
teruggaat.

**Kan ik mijn persoonlijke WhatsApp koppelen?**
Nee. Alleen een nummer op de Business API; dat is een eis van Meta.

**Kan hij veelgestelde vragen zelf afhandelen?**
Je kunt het inplannen, met bevestiging vóór verzending. Voor een echt
antwoordscript is de [AI Receptionist](ai-receptionist.md) geschikter.

**Kan ik WhatsApp en Instagram samen bekijken?**
Ja. Zijn beide gekoppeld, dan kun je in één opdracht vragen wat er op beide
kanalen binnenkwam.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [WhatsApp Business koppelen](../connectors/whatsapp-business.md) · [Instagram DM](instagram-dm.md) · [AI Receptionist](ai-receptionist.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, WhatsApp Business, bijgewerkt augustus 2026*
