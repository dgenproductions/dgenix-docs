# Slack koppelen

Koppel je Slack workspace om berichten te versturen, kanalen te lezen, direct messages te sturen en meer via je AI-assistent.

---

## Stappen

1. Ga naar **Dashboard → Connectors**
2. Klik op **"Verbinden"** bij Slack
3. Je wordt doorgestuurd naar het Slack autorisatiescherm
4. Selecteer de workspace die je wil koppelen
5. Klik op **"Toestaan"**
6. Na goedkeuring verschijnt Slack als **Verbonden**

---

## Welke skills worden vrijgegeven?

- **Slack** — berichten sturen/lezen, DMs, zoeken, kanalen aanmaken, reageren

---

## Toegangsrechten

dGENIX vraagt de volgende Slack-scopes aan:

| Scope | Waarvoor |
|---|---|
| `channels:read` + `channels:history` | Publieke kanalen lezen |
| `groups:read` + `groups:history` | Private kanalen lezen |
| `chat:write` | Berichten versturen |
| `im:read` + `im:write` | Direct messages lezen en sturen |
| `files:read` + `files:write` | Bestanden ophalen en uploaden |
| `search:read` | Berichten doorzoeken |
| `reactions:write` | Reageren op berichten |
| `channels:manage` | Kanalen aanmaken |
| `users:read` | Ledenlijst lezen |

---

## Verbinding verwijderen

Ga naar **Dashboard → Connectors** → klik op Slack → **"Verbreken"**.
Je kunt de koppeling ook intrekken via *Slack → Apps → dGENIX → App verwijderen*.

---

→ Terug naar [Connectors overzicht](README.md)
