# WhatsApp Business koppelen

De WhatsApp Business-koppeling laat GENI inkomende berichten uit je Business-inbox lezen en antwoorden versturen vanaf je zakelijke nummer.

Dit is de zwaarste koppeling om op te zetten, omdat Meta een Developer-account
en een goedgekeurde app vereist. Reken op een half uur. De koppeling activeert
de [WhatsApp Business-skill](../skills/whatsapp-business.md), beschikbaar vanaf
**Growth**.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Wat is er binnengekomen op WhatsApp?" | Leest de recente inkomende berichten |
| "Antwoord dat we morgen om 10:00 open zijn" | Verstuurt een bericht naar dat nummer |
| "Vat de gesprekken van vandaag samen" | Leest de inbox en zet de vragen op een rij |
| "Beantwoord nieuwe vragen over openingstijden automatisch" | Draait als herhaalde taak, met bevestiging vóór verzending |

## Vereisten

- Een Meta Developer-account
- Een goedgekeurde WhatsApp Business-app in Meta Business Manager
- Een telefoonnummer dat aan de WhatsApp Business API is gekoppeld

Een gewoon WhatsApp- of WhatsApp Business-**app**-account is niet genoeg; het
moet via de API lopen.

## Koppelen

1. Ga in Meta Business Manager naar *WhatsApp → API Setup*
2. Kopieer je **Access Token**, **Phone Number ID** en **Business Account ID**
3. Ga naar **Dashboard → Connectors** en klik op **Koppelen** bij WhatsApp Business
4. Vul de drie gegevens in en sla op; de koppeling is direct actief

## Webhook instellen

Zonder webhook kan GENI wel versturen, maar ontvangt hij geen berichten.

1. Ga naar je Meta App → *WhatsApp → Configuration*
2. Vul als Webhook URL in: `https://app.dgenix.com/api/whatsapp/webhook`
3. Vul als Verify Token de waarde in uit **Dashboard → Connectors → WhatsApp**
4. Abonneer op het event `messages`

## Welke toegang je geeft

| Gegeven | Waarvoor dGENIX het gebruikt |
|---|---|
| Access Token | Berichten ophalen en versturen namens je Business-account |
| Phone Number ID | Bepalen vanaf welk nummer een bericht vertrekt |
| Business Account ID | Je WhatsApp Business-account identificeren |

## Controleren of het werkt

Stuur vanaf je eigen telefoon een bericht naar je zakelijke nummer en vraag
daarna:

```
Wat is er binnengekomen op WhatsApp?
```

Zie je je testbericht terug, dan werkt de webhook. Blijft het leeg terwijl
versturen wel lukt, dan staat de webhook niet goed.

## Grenzen

- Een bericht versturen vraagt om bevestiging
- Meta staat vrije tekst alleen toe binnen **24 uur** na het laatste bericht van de klant; daarbuiten is een goedgekeurde sjabloon nodig
- Alleen tekst; afbeeldingen, documenten en spraakberichten versturen kan niet
- GENI verwijdert geen berichten en blokkeert geen contacten
- Groepsgesprekken worden niet ondersteund

## Problemen oplossen

**Er komen geen berichten binnen.** De webhook staat niet goed. Controleer de URL, het Verify Token en of je op `messages` bent geabonneerd.

**Versturen faalt buiten kantooruren.** Waarschijnlijk is het 24-uursvenster verlopen. Gebruik dan een in Meta goedgekeurde sjabloon.

**Het token verloopt.** Meta geeft standaard tijdelijke tokens uit. Maak in Meta een permanent systeemgebruiker-token aan en werk het bij in Connectors.

**Meta keurt je app niet goed.** Zonder goedgekeurde app werkt de API niet. Dat loopt volledig via Meta; dGENIX kan daar niets aan versnellen.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op WhatsApp Business en kies
**Verbreken**. Verwijder in Meta ook de webhook, anders blijft Meta proberen te
leveren.

## Veelgestelde vragen

**Kan ik mijn persoonlijke WhatsApp koppelen?**
Nee. Alleen een nummer op de WhatsApp Business API; dat is een vereiste van Meta.

**Antwoordt GENI automatisch op alles?**
Alleen als je dat expliciet inplant. Standaard leest hij en stel je zelf voor
wat er teruggaat, met bevestiging vóór verzending.

**Kost een bericht credits?**
Ja, versturen en lezen kosten credits binnen dGENIX. Meta rekent daarnaast zijn
eigen gesprekskosten; die lopen via je Meta-account.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [WhatsApp Business skill](../skills/whatsapp-business.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, WhatsApp Business koppelen, bijgewerkt augustus 2026*
