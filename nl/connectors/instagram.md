# Instagram Business koppelen

Koppel je Instagram Business-account via de Meta API om inkomende DMs te lezen en te beantwoorden via je AI-assistent.

---

## Vereisten

- Instagram Business-account (geen persoonlijk account)
- Gekoppeld aan een Facebook-pagina in Meta Business Manager
- Meta Developer-account met goedgekeurde app

---

## Stappen

1. Ga in Meta Business Manager naar *Instagram → API Setup*
2. Kopieer je **Access Token** en **Business Account ID**
3. Ga naar **Dashboard → Connectors**
4. Klik op **"Koppelen"** bij Instagram
5. Voer de credentials in en sla op
6. De connector is direct actief

---

## Webhook instellen

Om inkomende DMs te ontvangen:

1. Ga naar je Meta App → *Instagram → Webhooks*
2. Vul in als Webhook URL: `https://app.dgenix.com/api/instagram/webhook`
3. Vul in als Verify Token: je token uit Dashboard → Connectors → Instagram
4. Abonneer op het event `messages`

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Instagram DM Manager skill](../skills/instagram-dm.md)
