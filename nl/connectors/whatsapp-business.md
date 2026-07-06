# WhatsApp Business koppelen

Koppel je WhatsApp Business API via een Meta Developer-account om inkomende berichten te lezen en antwoorden te versturen via je AI-assistent.

---

## Vereisten

- Meta Developer-account
- Goedgekeurde WhatsApp Business-app in Meta Business Manager
- Telefoonnummer gekoppeld aan WhatsApp Business API

---

## Stappen

1. Ga in Meta Business Manager naar *WhatsApp → API Setup*
2. Kopieer je **Access Token**, **Phone Number ID** en **Business Account ID**
3. Ga naar **Dashboard → Connectors**
4. Klik op **"Koppelen"** bij WhatsApp Business
5. Voer de drie credentials in en sla op
6. De connector is direct actief

---

## Webhook instellen

Om inkomende berichten te ontvangen moet je een webhook instellen in Meta:

1. Ga naar je Meta App → *WhatsApp → Configuration*
2. Vul in als Webhook URL: `https://app.dgenix.com/api/whatsapp/webhook`
3. Vul in als Verify Token: je token uit Dashboard → Connectors → WhatsApp
4. Abonneer op het event `messages`

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [WhatsApp Business skill](../skills/whatsapp-business.md)
