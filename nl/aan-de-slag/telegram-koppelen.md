# Telegram koppelen (optioneel)

dGENIX is **dashboard-first**: je hebt Telegram niet nodig om te starten. Telegram is een **gratis, optionele add-on** waarmee je GENI ook onderweg bereikt. Alles loopt gesynchroniseerd met je dashboard: dezelfde assistent, hetzelfde geheugen, dezelfde skills.

> Je assistent instellen (naam, werkwijze) doe je tijdens de **intake** in het dashboard, niet via Telegram. Zie [Aan de slag](README.md).

---

## Telegram activeren

1. Ga naar **Dashboard -> Skills**
2. Zoek de **Telegram**-add-on en activeer hem (gratis)
3. Volg de koppel-stappen hieronder

---

## Optie A, gedeelde dGENIX-bot (makkelijkst)

Beschikbaar op elk plan.

1. Open **@dGENIXbot** in Telegram
2. Stuur het commando `/start` met je persoonlijke koppelcode (die zie je in het dashboard na het activeren van de add-on)
3. Je account wordt automatisch gekoppeld

## Optie B, eigen Telegram-bot (Pro+)

Wil je GENI onder je eigen botnaam en handle? Op **Pro** en hoger is de eigen bot inbegrepen.

1. Maak een bot via [BotFather](https://t.me/BotFather) in Telegram (commando `/newbot`)
2. Kopieer het bot-token dat je krijgt
3. Plak het token in **Dashboard -> Skills -> Eigen Telegram Bot**
4. dGENIX valideert de verbinding en zet je eigen bot live

[Meer over de skills](../skills/README.md)

---

## Wat kun je via Telegram?

Dezelfde dingen als in het dashboard: een opdracht sturen, een vraag stellen, een spraakbericht inspreken. GENI antwoordt in Telegram en bewaart alles in hetzelfde geheugen en dezelfde gesprekken als je dashboard.

Voorbeelden:

- "Geef me een overzicht van mijn ongelezen mails"
- "Plan een meeting met Jan vrijdag om 14:00"
- "Vat dit spraakbericht samen en zet de actiepunten in mijn agenda"

---

## Commando's in Telegram

Naast gewone opdrachten kent de bot een paar vaste commando's:

| Commando | Wat het doet |
|---|---|
| `/start` | Assistent activeren en je koppelcode invoeren |
| `/credits` | Je huidige creditsaldo opvragen |
| `/help` | Korte lijst met beschikbare commando's |

---

## Spraakberichten

Stuur een spraakbericht in Telegram en GENI zet het automatisch om naar tekst en
verwerkt het als een gewone opdracht. Je hoeft niets in te stellen. Handig
onderweg: inspreken wat er moet gebeuren, GENI regelt de rest.

---

## Web en Telegram lopen synchroon

Wat je in de webchat stuurt verschijnt ook in Telegram, en andersom. Je
gespreksgeschiedenis, je geheugen en je actieve skills zijn in beide kanalen
hetzelfde. Je begint dus een gesprek achter je bureau en maakt het onderweg af.

---

## Problemen oplossen

**GENI reageert niet in Telegram.** Controleer of de koppeling nog actief is via
**Dashboard → Skills → Telegram**, en of je creditsaldo niet op nul staat (je
ziet het saldo rechtsboven in het dashboard).

**Koppeling kwijt na het wisselen van telefoon.** Je Telegram-account blijft
gekoppeld aan je dGENIX-account, niet aan een toestel. Stuur opnieuw `/start`
met je koppelcode uit het dashboard.

**Verkeerde bot.** Gebruik je een eigen bot, dan reageert `@dGENIXbot` niet meer
op jouw account. Chat met je eigen bot.

---

## Telegram ontkoppelen

Ga naar **Dashboard -> Skills**, open de Telegram-add-on en kies ontkoppelen. Je account, credits en geschiedenis blijven bewaard, je blijft gewoon via het dashboard werken.

---

→ Verder: [AI-assistent](../functies/ai-assistent.md) · [Aan de slag](README.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, Telegram koppelen, bijgewerkt augustus 2026*
