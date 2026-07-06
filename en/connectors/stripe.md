# Connect Stripe

Connect your Stripe account via a Restricted API Key to fetch revenue data and payment information via your AI assistant.

---

## Steps

1. Log in to your Stripe Dashboard
2. Go to *Developers -> API Keys -> Restricted Keys*
3. Click **"+ Create restricted key"**
4. Give the key a name (e.g. "dGENIX read-only")
5. Set the following permissions to **Read:**
   - `Balance`, for balance overview
   - `Charges`, for payments
   - `Customers`, for customer data
   - `Subscriptions`, for subscriptions
   - `Payment Intents`, for transactions
6. Copy the generated API key
7. Go to **Dashboard -> Connectors**
8. Click **"Connect"** on Stripe and enter the key

---

## No write access needed

The Stripe Insights skill only needs read access. Via this connection dGENIX cannot create or refund payments.

---

Back to [Connectors overview](README.md)
See also: [Stripe Insights skill](../skills/stripe-insights.md)
