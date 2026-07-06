# Connect WhatsApp Business

Connect your WhatsApp Business API via a Meta Developer account to read incoming messages and send replies via your AI assistant.

---

## Requirements

- Meta Developer account
- Approved WhatsApp Business app in Meta Business Manager
- Phone number linked to the WhatsApp Business API

---

## Steps

1. In Meta Business Manager go to *WhatsApp -> API Setup*
2. Copy your **Access Token**, **Phone Number ID** and **Business Account ID**
3. Go to **Dashboard -> Connectors**
4. Click **"Connect"** on WhatsApp Business
5. Enter the three credentials and save
6. The connector is active right away

---

## Setting up the webhook

To receive incoming messages you must set up a webhook in Meta:

1. Go to your Meta App -> *WhatsApp -> Configuration*
2. Set the Webhook URL: `https://app.dgenix.com/api/whatsapp/webhook`
3. Set the Verify Token: your token from Dashboard -> Connectors -> WhatsApp
4. Subscribe to the `messages` event

---

Back to [Connectors overview](README.md)
See also: [WhatsApp Business skill](../skills/whatsapp-business.md)
