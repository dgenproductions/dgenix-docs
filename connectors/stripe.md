# Stripe koppelen

Koppel je Stripe-account via een Restricted API Key om omzetdata en betalingsinformatie op te halen via je AI-assistent.

---

## Stappen

1. Log in op je Stripe Dashboard
2. Ga naar *Developers → API Keys → Restricted Keys*
3. Klik op **"+ Create restricted key"**
4. Geef de key een naam (bijv. "dGENIX read-only")
5. Zet de volgende rechten op **Read:**
   - `Balance` — voor saldooverzicht
   - `Charges` — voor betalingen
   - `Customers` — voor klantdata
   - `Subscriptions` — voor abonnementen
   - `Payment Intents` — voor transacties
6. Kopieer de gegenereerde API-sleutel
7. Ga naar **Dashboard → Connectors**
8. Klik op **"Koppelen"** bij Stripe en voer de sleutel in

---

## Geen schrijfrechten nodig

De Stripe Inzichten-skill heeft alleen leesrechten nodig. dGENIX kan via deze koppeling geen betalingen aanmaken of terugboeken.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Stripe Inzichten skill](../skills/stripe-insights.md)
