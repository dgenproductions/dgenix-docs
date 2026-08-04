# Instagram Business koppelen

De Instagram-koppeling laat GENI inkomende DM's uit je Business-inbox lezen, ze sorteren op type en antwoorden voor je klaarzetten.

De koppeling activeert de [Instagram DM-skill](../skills/instagram-dm.md),
beschikbaar vanaf **Growth**. Het opzetten loopt via Meta, net als bij WhatsApp.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Wat staat er in mijn Instagram-DM's?" | Leest de recente inkomende berichten |
| "Welke berichten zijn echte leads?" | Sorteert elk bericht als spam, vraag, lead of afspraak |
| "Antwoord dat we open zijn tot 18:00" | Stuurt een DM naar dat account |
| "Vat de DM's van vandaag samen" | Zet de vragen op een rij, spam eruit gefilterd |

De sortering is het nuttigste onderdeel: bij tientallen DM's per dag zie je in
één blik welke er echt toe doen.

## Vereisten

- Een Instagram **Business**-account, geen persoonlijk account
- Gekoppeld aan een Facebook-pagina in Meta Business Manager
- Een Meta Developer-account met een goedgekeurde app

## Koppelen

1. Ga in Meta Business Manager naar *Instagram → API Setup*
2. Kopieer je **Access Token** en **Business Account ID**
3. Ga naar **Dashboard → Connectors** en klik op **Koppelen** bij Instagram
4. Vul beide gegevens in en sla op; de koppeling is direct actief

## Webhook instellen

Zonder webhook kan GENI wel versturen, maar ontvangt hij geen DM's.

1. Ga naar je Meta App → *Instagram → Webhooks*
2. Vul als Webhook URL in: `https://app.dgenix.com/api/instagram/webhook`
3. Vul als Verify Token de waarde in uit **Dashboard → Connectors → Instagram**
4. Abonneer op het event `messages`

## Welke toegang je geeft

| Gegeven | Waarvoor dGENIX het gebruikt |
|---|---|
| Access Token | DM's ophalen en versturen namens je Business-account |
| Business Account ID | Je Instagram Business-account identificeren |

De koppeling raakt alleen je **DM's**. Posts, verhalen, reacties en je
volgerslijst blijven buiten bereik.

## Controleren of het werkt

Stuur vanaf een ander Instagram-account een DM naar je Business-account en
vraag daarna:

```
Wat staat er in mijn Instagram-DM's?
```

Zie je het testbericht, dan werkt de webhook.

## Grenzen

- Een DM versturen vraagt om bevestiging
- Meta staat vrije tekst alleen toe binnen **24 uur** na het laatste bericht van de klant
- Alleen tekst; afbeeldingen, verhalen-reacties en spraakberichten kunnen niet
- Geen reacties onder posts lezen of beantwoorden
- GENI verwijdert geen berichten en blokkeert geen accounts

## Problemen oplossen

**Er komen geen DM's binnen.** De webhook staat niet goed. Controleer de URL, het Verify Token en het `messages`-abonnement.

**Je account wordt niet geaccepteerd.** Het is waarschijnlijk een persoonlijk of Creator-account. Zet het in de Instagram-app om naar een Business-account en koppel het aan een Facebook-pagina.

**Versturen faalt.** Het 24-uursvenster is verlopen, of het account heeft je geblokkeerd.

**Reacties onder posts ontbreken.** Die vallen bewust buiten deze koppeling; alleen DM's worden opgehaald.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Instagram en kies **Verbreken**.
Verwijder in Meta ook de webhook.

## Veelgestelde vragen

**Kan ik mijn persoonlijke Instagram koppelen?**
Nee. Meta geeft alleen Business-accounts toegang tot de DM-API.

**Beantwoordt GENI DM's automatisch?**
Alleen als je dat inplant. Standaard leest en sorteert hij, en beslis jij wat er
teruggaat.

**Kan ik dit combineren met WhatsApp?**
Ja. Zijn beide gekoppeld, dan kun je in één opdracht vragen wat er op beide
kanalen binnenkwam.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Instagram DM skill](../skills/instagram-dm.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Instagram Business koppelen, bijgewerkt augustus 2026*
