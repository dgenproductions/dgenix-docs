# Instagram DM

Met de Instagram DM-skill leest GENI je Business-inbox, sorteert hij elk bericht op type en stelt hij antwoorden op.

Dat sorteren is het nuttigste onderdeel: bij tientallen DM's per dag zie je in
één blik welke er echt toe doen. Beschikbaar vanaf **Growth**; zie
[Instagram Business koppelen](../connectors/instagram.md).

## Wat kan GENI met Instagram DM?

- **Je Business-inbox lezen** en de recente DM's ophalen
- **Een bericht classificeren** als spam, veelgestelde vraag, lead of afspraakverzoek
- **Een DM versturen** naar een account

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Welke DM's van vandaag zijn echt de moeite waard?
```

> **23 DM's, gesorteerd**
>
> | Type | Aantal |
> |---|---|
> | Lead | 3 |
> | Afspraakverzoek | 2 |
> | Veelgestelde vraag | 9 |
> | Spam | 9 |
>
> **De 3 leads:**
> - **@sportschool_veldhoven** , vraagt naar een offerte voor 40 man
> - **@marieke.k** , wil weten of je ook in Tilburg werkt
> - **@bouwbedrijf_jansen** , vraagt naar samenwerking
>
> De 9 veelgestelde vragen gaan bijna allemaal over je openingstijden. Zal ik
> daar één antwoord voor opstellen dat je kunt hergebruiken?

## Vereisten

- **Plan:** Growth en hoger
- Een Instagram **Business**-account, geen persoonlijk account
- Gekoppeld aan een Facebook-pagina in Meta Business Manager
- Een **Meta Developer-account** met een goedgekeurde app

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Instagram DM**
2. Ga naar **Dashboard → Connectors** en voer je Meta-gegevens in
3. Stel de webhook in bij Meta, anders ontvang je geen DM's
4. Instagram DM is bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| DM's lezen en samenvatten | ~50 |
| Antwoord opstellen en versturen | ~80 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Versturen vraagt om bevestiging.**
- **Meta staat vrije tekst alleen toe binnen 24 uur** na het laatste bericht van de klant.
- **Alleen tekst.** Afbeeldingen, verhaal-reacties en spraakberichten kunnen niet.
- **Alleen DM's.** Reacties onder posts worden niet gelezen of beantwoord.
- **GENI verwijdert geen berichten en blokkeert geen accounts.**
- **De classificatie is een inschatting**, geen zekerheid. Loop de leads zelf na.

## Problemen oplossen

**Er komen geen DM's binnen.** De webhook staat niet goed. Controleer de URL, het Verify Token en het `messages`-abonnement.

**Je account wordt niet geaccepteerd.** Het is waarschijnlijk een persoonlijk of Creator-account. Zet het om naar Business en koppel het aan een Facebook-pagina.

**Een echte lead werd als spam bestempeld.** De classificatie is een inschatting. Vraag om de volledige lijst als je niets wilt missen.

**Versturen faalt.** Het 24-uursvenster is verlopen, of het account heeft je geblokkeerd.

## Veelgestelde vragen

**Beantwoordt GENI DM's automatisch?**
Alleen als je dat inplant. Standaard leest en sorteert hij, en beslis jij.

**Kan ik mijn persoonlijke Instagram koppelen?**
Nee. Meta geeft alleen Business-accounts toegang tot de DM-API.

**Kan ik dit combineren met WhatsApp?**
Ja, dan vraag je in één opdracht wat er op beide kanalen binnenkwam. Zie
[WhatsApp Business](whatsapp-business.md).

**Kan hij reacties onder mijn posts beantwoorden?**
Nee, die vallen buiten deze koppeling.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Instagram Business koppelen](../connectors/instagram.md) · [WhatsApp Business](whatsapp-business.md) · [Social Media Manager](social-media.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Instagram DM, bijgewerkt augustus 2026*
