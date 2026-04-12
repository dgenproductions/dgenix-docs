# Telegram koppelen & assistent activeren

Je AI-werknemer communiceert via Telegram. Je hebt dus een Telegram-account nodig. Download de app via [telegram.org](https://telegram.org) als je hem nog niet hebt.

---

## Stap 1 — Telegram koppelen

Na registratie of via **Dashboard → Instellingen → Integraties** kun je Telegram koppelen.

Je hebt twee opties:

### Optie A — dGENIX gedeelde bot (aanbevolen)

De makkelijkste optie. Klik op de **"Verbinden via Telegram"** knop. Je wordt doorgestuurd naar Telegram. Geef toestemming, en je chat ID wordt automatisch opgeslagen.

### Optie B — Handmatig (chat ID invoeren)

1. Open de **@dGENIXbot** in Telegram
2. Stuur het commando `/start`
3. De bot antwoordt met je chat ID (een reeks cijfers)
4. Kopieer dit getal en plak het in het invoerveld op de onboarding pagina

### Optie C — Eigen Telegram bot

Heb je de **Eigen Bot skill** actief? Dan kun je ook je eigen Telegram bot koppelen:

1. Maak een bot aan via [BotFather](https://t.me/BotFather) in Telegram (commando: `/newbot`)
2. Je ontvangt een bot token — kopieer dit
3. Plak het token én je chat ID in de bijbehorende velden
4. dGENIX valideert de verbinding en activeert je eigen bot

→ [Meer over de Eigen Bot skill](../skills/README.md)

---

## Stap 2 — Geef je assistent een naam {#assistent-naam}

Geef je AI-werknemer een naam. Die naam gebruikt hij om zich voor te stellen in Telegram, en is zichtbaar in je dashboard.

**Kies iets wat bij jou past** — een voornaam zoals "Alex" of "Sara", of iets functioneels zoals "Assistent".

De naam wordt opgeslagen bij je account en verschijnt in het welkomstbericht dat je ontvangt zodra je assistent actief is.

---

## Stap 3 — Assistent activeren {#assistent-activeren}

Klik op **"Activeer mijn assistent"**.

dGENIX zet nu je persoonlijke AI-werknemer op. Dit duurt maximaal 30 seconden. Op de achtergrond gebeurt het volgende:

- Je persoonlijke AI-workflow wordt aangemaakt
- Je Telegram verbinding wordt geconfigureerd
- Je startcredits worden ingeladen
- Je assistent wordt live gezet

Je ontvangt een **welkomstbericht in Telegram** zodra alles klaar is — dan ben je live.

---

## Stap 4 — Integraties koppelen (optioneel)

Koppel Gmail, Google Calendar, Google Sheets en Google Drive om je assistent volledige toegang te geven tot je tools.

Ga naar **Dashboard → Instellingen → Integraties** en klik op **"Verbinden"** naast elke tool. Je wordt doorgestuurd naar Google voor toestemming — dit duurt minder dan een minuut per integratie.

→ [Gmail koppelen](../integraties/gmail.md)
→ [Google Calendar koppelen](../integraties/google-calendar.md)
→ [Google Drive koppelen](../integraties/google-drive.md)

---

## Stap 5 — Klaar

Je AI-werknemer is actief. Je kunt direct beginnen door een bericht te sturen in Telegram.

**Voorbeeldopdrachten:**

- `Geef me een overzicht van mijn ongelezen mails`
- `Plan een meeting met Jan vrijdag 14:00`
- `Onderzoek de beste tools voor social media planning in 2026`

Je assistent voert de taak uit en stuurt het resultaat terug in Telegram.

---

## Verbinding verbreken

Ga naar **Dashboard → Instellingen → Integraties** en klik op "Verwijderen" naast Telegram. Dit deactiveert je assistent. Je account en credits blijven bewaard.

> ⚠️ Als je Telegram ontkoppelt, kan je assistent geen berichten meer ontvangen of versturen.
