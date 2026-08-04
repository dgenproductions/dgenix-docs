# Skills explained

Skills extend what your assistant can do. By default it can chat, write text and answer general questions. With skills you add specific capabilities.

---

## What is a skill?

A skill is a set of tools and instructions that gives your assistant new actions. After activation the assistant knows what it can do with that skill and when to use it.

**Example without a skill:**
> "Send an email to Jan about tomorrow's meeting"
> Assistant: "I can't send emails, I have no access to your inbox."

**Example with the Gmail skill:**
> "Send an email to Jan about tomorrow's meeting"
> The assistant looks up Jan's email address, writes an email and sends it. You get a confirmation.

---

## How do you activate a skill?

1. Go to **Dashboard -> Skills**
2. Browse the Skills Marketplace
3. Click **"Activate"** on the skill you want
4. Complete any setup steps (connecting a service, entering an API key)
5. The skill is available right away

Some skills need an integration (for example connecting Gmail). A tutorial appears right after activation.

---

## How does the assistant know when to use a skill?

The assistant uses skills automatically based on the context of your question. You do not have to say "use the Gmail skill", it recognises when it needs access to something.

**You ask:** "Send the quote as an attachment to client@example.com"
**Assistant recognises:** this is an email with an attachment -> uses the Gmail skill + Drive skill

You can also call a skill explicitly:
> "Use Social Media Manager to write a LinkedIn post about..."
> "Generate an image with FLUX of..."

---

## Skill categories

### Personal, included (Starter+)

Skills for daily productivity. Free to activate.

| Skill | What it does |
|---|---|
| **Gmail** | Read, write and send emails |
| **Google Calendar** | Manage your calendar |
| **Google Drive** | Find, read and create files |
| **Google Sheets** | Read and update spreadsheets |
| **Daily Planner & Life Assistant** | Build a daily plan, rank priorities |
| **Document Reader** | Read and summarise PDFs and Word docs |
| **Short Generator** | Short clips from a video URL (basic) |
| **Telegram Add-on** | Use the assistant via Telegram too |

### Business, Growth+

Skills for business tasks. Available from the Growth plan.

| Skill | What it does |
|---|---|
| **AI Image Generation** | Generate images with Google Nano Banana (+ Pro) |
| **FLUX Image Generation** | Generate images with the FLUX-1 model |
| **Social Media Manager** | Write posts for LinkedIn, Instagram, X and Facebook |
| **Proposal Generator** | Create professional quotes and proposals |
| **Content Repurposing** | Reuse and reformat content |
| **Weekly Report Generator** | Automatically compile weekly reports |
| **Lead Research & Outreach** | Research leads and write personal outreach |
| **Client Onboarding** | Onboarding documents and welcome emails |
| **Audio Transcription** | Convert audio recordings to text |
| **Travel Planner** | Travel plans and route overviews |
| **Smart Shopping** | Compare products and give buying advice |
| **Meal Planner** | Meal plans and shopping lists |
| **Personal Finance** | Analyse income and expenses |
| **YouTube Manager** | Manage a channel, write titles and descriptions |
| **SEO Blog Writer** | Write SEO-optimised blog articles |
| **AI Image Editing** | Edit existing images with AI |

### Business, Pro+

Skills for advanced use. Included from the Pro plan.

| Skill | What it does |
|---|---|
| **GEO Engine** | Measure AI visibility (Share-of-Voice in ChatGPT/Perplexity/Gemini/Claude) |
| **Authority Engine** | Write content and publish draft-first to your CMS |
| **Reputation Engine** | Review campaigns via branded email with a Google review link |
| **Workflow Builder** | Import and run n8n workflows as an AI tool |
| **Support Knowledge Base** | Build a knowledge base for automated support answers |
| **Meeting Assistant** | Minutes and action items from a conversation or recording |
| **CRM Sync** | Read and update CRM data |
| **Invoice Generator** | Create and send invoices |
| **Renewal & Upsell Intelligence** | Analyse client data for renewal and upsell opportunities |
| **Own Telegram Bot** | GENI under your own bot name and handle |

> No more separate add-on prices: all business skills are **included from Growth+ or Pro+** (depending on the skill). You pay per action in credits, not per skill per month. See [Plans & Pricing](../plannen-en-prijzen/README.md).

---

## Skills and integrations

Most skills need a connection to work. After activation a tutorial walks you through the setup.

**OAuth integrations** (log in once):
- Gmail, Google Calendar, Drive, Sheets -> connect a Google account
- Notion -> connect a Notion account
- Slack -> connect a Slack workspace
- LinkedIn -> connect a LinkedIn account

**API-key integrations** (enter a credential):
- WhatsApp Business -> Meta Business API key
- Instagram DM -> Meta Business API key
- Stripe -> Stripe API key
- HubSpot -> HubSpot API key

You manage integrations via **Connectors**.

---

## Deactivating skills

Go to **Dashboard -> Skills** or **Account -> Subscription** and click "Deactivate" on the skill. Credits already used are not refunded.

---

## Skill credits, what does a skill cost?

Every skill action uses credits. A guideline:

Indicative prices per task type live in one place: **[The credit system](../hoe-het-werkt/credits.md)**.
It shows roughly what a chat question, an email action or an engine audit costs.

Two things determine the price of a skill action. Each skill has a fixed
overhead, and on top of that the language model is billed by usage. A quick
question about three emails therefore costs less than summarising a full inbox,
even though it is the same skill.

Actions with a fixed price, such as an audit or an image generation, are exact.
Those appear as an amount on the button before you start them.

Beyond that, exact costs are shown per skill in the marketplace card and the
related skill documentation.

---

## Frequently asked questions

**Can I choose which skill the assistant uses?**
The assistant chooses automatically based on context. You can also call a skill explicitly: "use the Social Media Manager to...".

**Does a skill work via both the dashboard and Telegram?**
Yes, all activated skills work via both interfaces.

**What if a skill fails?**
The assistant reports the error in chat. Check that your integration is still active (Connectors). If the problem persists, contact Support.

**Can I test a skill before activating?**
No, you have to activate it. Skills included in your plan activate for free and can be deactivated any time.
