# Connect Instagram Business

Connect your Instagram Business account via the Meta API to read and reply to incoming DMs via your AI assistant.

---

## Requirements

- Instagram Business account (not a personal account)
- Linked to a Facebook page in Meta Business Manager
- Meta Developer account with an approved app

---

## Steps

1. In Meta Business Manager go to *Instagram -> API Setup*
2. Copy your **Access Token** and **Business Account ID**
3. Go to **Dashboard -> Connectors**
4. Click **"Connect"** on Instagram
5. Enter the credentials and save
6. The connector is active right away

---

## Setting up the webhook

To receive incoming DMs:

1. Go to your Meta App -> *Instagram -> Webhooks*
2. Set the Webhook URL: `https://app.dgenix.com/api/instagram/webhook`
3. Set the Verify Token: your token from Dashboard -> Connectors -> Instagram
4. Subscribe to the `messages` event

---

Back to [Connectors overview](README.md)
See also: [Instagram DM Manager skill](../skills/instagram-dm.md)
