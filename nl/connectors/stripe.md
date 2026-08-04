# Stripe koppelen

De Stripe-koppeling laat GENI je omzetcijfers, abonnementen en mislukte betalingen ophalen, zodat je ze in gewone taal kunt opvragen.

Je koppelt met een **Restricted API Key** die je zelf aanmaakt en waarop je
alleen leesrechten zet. De koppeling activeert de
[Stripe Inzichten-skill](../skills/stripe-insights.md), beschikbaar vanaf
**Growth**.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Hoe staat mijn omzet ervoor?" | Geeft MRR, ARR, aantal klanten en actieve abonnementen |
| "Zijn er betalingen mislukt?" | Haalt de recente mislukte betalingen op |
| "Wat heeft klant X bij ons afgenomen?" | Zoekt op e-mailadres of Stripe customer-ID |
| "Stuur me elke maandag een omzetoverzicht" | Combineert dit met je e-mailkoppeling in een herhaalde taak |

## Koppelen

1. Log in op je Stripe Dashboard
2. Ga naar *Developers → API Keys → Restricted Keys*
3. Klik op **+ Create restricted key** en geef hem een naam, bijvoorbeeld "dGENIX read-only"
4. Zet deze rechten op **Read**:
   - `Balance`, voor het saldo-overzicht
   - `Charges`, voor betalingen
   - `Customers`, voor klantgegevens
   - `Subscriptions`, voor abonnementen
   - `Payment Intents`, voor transacties
5. Kopieer de sleutel die je krijgt
6. Ga naar **Dashboard → Connectors**, klik op **Koppelen** bij Stripe en plak de sleutel

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| `Balance` (read) | Saldo-overzicht |
| `Charges` (read) | Betalingen en mislukte incasso's |
| `Customers` (read) | Een klant opzoeken |
| `Subscriptions` (read) | Actieve abonnementen en MRR |
| `Payment Intents` (read) | Transactiedetails |

**Schrijfrechten heb je niet nodig.** Zet ze ook niet aan: dan is technisch
uitgesloten dat er via deze koppeling ooit een betaling wordt aangemaakt of
teruggeboekt.

## Controleren of het werkt

Vraag direct na het koppelen:

```
Hoe staat mijn Stripe-omzet ervoor?
```

Je krijgt MRR, ARR en het aantal klanten terug. Krijg je een rechtenfout, dan
mist er een `read`-recht op je restricted key.

## Grenzen

- **Alleen lezen.** GENI kan geen betaling aanmaken, terugboeken of annuleren
- Geen abonnementen wijzigen of opzeggen
- Geen klantgegevens aanpassen in Stripe
- De cijfers komen rechtstreeks uit Stripe; ze worden niet opgeslagen of bijgehouden
- Bij zeer grote accounts wordt een deel van de historie opgehaald, niet alles

## Problemen oplossen

**Rechtenfout bij het opvragen.** Een `read`-recht ontbreekt. Open de restricted key in Stripe en zet de ontbrekende resource op Read.

**De sleutel wordt niet geaccepteerd.** Je gebruikte waarschijnlijk je publishable key (`pk_...`) of een standaard secret key. Het moet een **restricted key** (`rk_...`) zijn.

**Je ziet testdata.** Je maakte de sleutel aan in testmodus. Zet Stripe op live en maak een nieuwe restricted key aan.

## Verbinding verbreken

Trek de restricted key in via Stripe (*Developers → API Keys*), of ga naar
**Dashboard → Connectors**, klik op Stripe en kies **Verbreken**. Een ingetrokken
sleutel werkt onmiddellijk niet meer.

## Veelgestelde vragen

**Kan GENI per ongeluk geld verplaatsen?**
Nee. De sleutel heeft alleen leesrechten, dus de mogelijkheid bestaat technisch
niet, ongeacht wat je vraagt.

**Kan ik dit combineren met andere skills?**
Ja, dat is de meerwaarde: een maandelijks omzetoverzicht dat GENI zelf ophaalt,
samenvat en naar je mailt. Zie [Geplande taken](../handleiding/geplande-taken.md).

**Is dit hetzelfde Stripe-account waarmee ik dGENIX betaal?**
Nee. Deze koppeling gaat over **jouw** Stripe-account en jouw klanten. Je eigen
abonnement staat los en beheer je via Facturering in het dashboard.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Stripe Inzichten skill](../skills/stripe-insights.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Stripe koppelen, bijgewerkt augustus 2026*
