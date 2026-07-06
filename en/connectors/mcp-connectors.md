# MCP connectors

MCP connectors link your AI assistant to external tools via the **Model Context Protocol (MCP)**, an open standard that lets dGENIX plug in ready-made connectors from the growing MCP ecosystem. For you, such a connector works exactly like a regular skill: you activate it in the marketplace, connect your own account, and your assistant uses its tools automatically.

---

## How it works

1. Go to **Dashboard -> Skills** and find the connector
2. Click **Activate** (the connector appears as a regular skill toggle)
3. Follow the step-by-step instruction that appears right after activation
4. Connect your own account via **Dashboard -> Connectors** (only if the connector requires it)
5. Ask your assistant to use the connector

Every MCP connector has its own instruction in the dashboard, just like Gmail or WhatsApp. You do not need to do anything technical.

---

## Your own account

MCP connectors run on **your own account** at the external service by default. You connect it with one click (OAuth) or by entering your own API key. Benefits:

- You keep control of your account and your data
- Any costs of the external service run through your account, not dGENIX
- You can disconnect any time via **Connectors -> Disconnect**

---

## Credits

MCP connectors use the same credit system as all other skills. Each connector has a fixed credit price per action. Expensive actions ask for confirmation first ("this costs X credits, continue?") before running, so there are no surprises.

---

## Connecting: OAuth or API key

- **OAuth (one click):** you log in to the service and grant permission. The preferred method.
- **API key:** you paste a key from your account at the external service, just like WhatsApp Business or Stripe.
- **No connection:** some open connectors need no account, activating is enough.

Which method applies is shown in the connector's own instruction.

---

Back to [Connectors](README.md)
