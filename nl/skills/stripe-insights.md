# Stripe Inzichten

Met Stripe Inzichten vraag je je omzet, mislukte betalingen en klantgegevens op in gewone taal, zonder het Stripe-dashboard te openen.

Beschikbaar vanaf **Growth**. Je hebt een gekoppeld Stripe-account nodig; de
koppeling is alleen-lezen.

## Wat kan GENI hiermee?

- **Een omzetoverzicht opvragen** over een periode: omzet, aantal betalingen, terugbetalingen
- **Mislukte betalingen opvragen** , welke, van wie, en waarom ze misgingen
- **Een klant opzoeken** met zijn betaalgeschiedenis en abonnementsstatus

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Hoe stond juli ervoor?
```

> **Juli 2026**
>
> | | |
> |---|---|
> | Omzet | € 14.280 |
> | Betalingen | 47 geslaagd |
> | Mislukt | 6 |
> | Terugbetaald | € 340 (2 stuks) |
>
> Juni was € 12.910, dus **+10,6 procent**.
>
> Van die 6 mislukte betalingen zijn er 4 om dezelfde reden gestopt:
> onvoldoende saldo, allemaal op de 1e van de maand. Dat is samen € 592 die
> waarschijnlijk gewoon te innen is met een tweede poging later in de maand.

En gericht:

```
Wat is de status van klant De Krent?
```

> **De Krent** , klant sinds maart 2026
> Abonnement **actief**, € 95 per maand, volgende incasso 12 augustus.
> Totaal betaald: € 475 over 5 facturen, geen mislukte betalingen.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** Stripe via **Dashboard → Connectors**. Zie [Stripe koppelen](../connectors/stripe.md)

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Stripe Inzichten**
2. Koppel je Stripe-account via **Dashboard → Connectors**
3. Vraag naar je omzet

## Wat het kost

| Actie | Credits |
|---|---|
| Omzetoverzicht | 25 |
| Mislukte betalingen | 15 |
| Klant opzoeken | 10 |

Zie [Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Alleen lezen.** GENI maakt geen betalingen aan, wijzigt geen abonnementen en doet geen terugbetalingen.
- **Geen facturen versturen.** Daarvoor is de [Factuur Automator](invoice-automator.md).
- **Alleen wat in Stripe staat.** Betalingen buiten Stripe (bank, contant, andere provider) kent hij niet.
- **Geen boekhouding.** Omzet in Stripe is niet hetzelfde als omzet in je aangifte; kosten en btw zitten er niet in.
- **Klantdata is echte klantdata.** Wat je opvraagt komt in je gesprek te staan, houd daar rekening mee.

## Problemen oplossen

**"Geen toegang tot Stripe".** De koppeling is verlopen of de sleutel is ingetrokken. Verbind opnieuw via Connectors.

**De cijfers wijken af van mijn dashboard.** Meestal een periodeverschil of een andere valuta. Noem de periode expliciet.

**Hij vindt de klant niet.** Zoek op het e-mailadres uit Stripe; bedrijfsnamen wijken vaak af van wat er in Stripe staat.

**Ik zie testdata.** De koppeling staat op je testomgeving. Koppel de live-sleutel.

## Veelgestelde vragen

**Kan hij geld terugstorten?**
Nee. De koppeling is bewust alleen-lezen; alles wat geld verplaatst doe je in
Stripe zelf.

**Kan ik een maandelijks omzetrapport krijgen?**
Ja, via [Geplande taken](../handleiding/geplande-taken.md). Op de eerste van de
maand een overzicht in je mail is de meest gebruikte vorm.

**Werkt dit samen met het Financieel Overzicht?**
Ja. [Financieel Overzicht](finance.md) gebruikt je Stripe-omzet automatisch als
deze skill actief is.

**Zijn mijn betaalgegevens veilig?**
De koppeling leest alleen. Zie het [privacybeleid](https://dgenix.nl/privacy) voor hoe gegevens
worden opgeslagen.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Financieel Overzicht](finance.md) · [Factuur Automator](invoice-automator.md) · [Stripe koppelen](../connectors/stripe.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Stripe Inzichten, bijgewerkt augustus 2026*
