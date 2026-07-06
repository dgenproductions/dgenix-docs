# Platform Manual, dGENIX

Welcome to the full dGENIX user manual. This document explains the platform from A to Z: how your assistant works, how it builds context, which features are available and how to get the most out of everything.

---

## What is dGENIX?

dGENIX is a personal AI platform. Not a chatbot that forgets every conversation, an assistant that gets to know you, runs tasks and is extensible through skills.

**Two interfaces:**

- **Web Dashboard** (`app.dgenix.com`), the primary interface. Here you chat, configure, activate skills and view everything.
- **Telegram** (optional add-on), activate the Telegram link if you also want to work with your assistant on the go from your phone.

---

## How does your assistant work?

Your assistant is a Claude AI model (by Anthropic) that loads context before every conversation. That context consists of several layers that together shape how it responds:

| Layer | What it is | Managed in |
|---|---|---|
| **Platform knowledge** | What dGENIX is, which skills are available, general behaviour rules | Automatic (by dGENIX) |
| **Knowledge document** | Your personal profile document, who you are, how you work, what you want | Settings -> AI Assistant |
| **Personal instructions** | Fixed rules your assistant always follows | Settings -> AI Assistant |
| **Knowledge base** | Documents you upload as background knowledge (.md, .pdf, .docx, .txt) | Dashboard -> Assistant -> Knowledge base |
| **Memory** | Facts, preferences and patterns the assistant remembers automatically | Settings -> Memory |
| **Project instructions** | Specific context per project folder (client, tone, rules) | Per project folder, gear icon |

All these layers are combined for every conversation. That way your assistant knows who you are, how to respond and the context of the conversation, without you having to explain it each time.

More on these systems: [Context and memory explained](context-en-geheugen.md)

---

## Dashboard, the features

### AI Assistant (chat)

The chat interface is your main channel. Send commands as text, via microphone (speech-to-text) or as a Voice Call (fully spoken conversation). The assistant runs tasks, gives answers and saves results.

[AI Assistant](../functies/ai-assistent.md)

### Projects

Create project folders for clients, projects or themes. Each project has its own conversations and optionally its own instructions, so your assistant keeps context separate per client or project.

**Example:** the project "De Krent Bakery" has instructions about tone of voice and the product range. Conversations in that project automatically use that context.

[Projects](../functies/projecten.md)

### Tasks & automation

Set up recurring commands your assistant runs automatically, daily, weekly or at a fixed time. Think of a daily report, a weekly newsletter or a monthly summary.

[Tasks and reminders](geplande-taken.md)

### Files & assets

Everything your assistant generates (documents, images, audio transcripts) is in the Files overview. You can download, share or reuse them.

[Files & Images](../functies/bestanden.md)

### Knowledge base

Upload documents your assistant uses as background knowledge. Supported formats: PDF, Word (.docx), text files (.txt) and Markdown (.md). The assistant reads these documents and uses them for relevant questions and tasks.

[Knowledge base](../functies/kennisbank.md)

### Voice Chat

**Voice Memo:** click the microphone icon in the chat and speak. Your question is converted to text and processed. The answer appears as text in the chat.

**Voice Call:** click the sound-waves icon for a fully spoken conversation. An animated orb screen opens, you speak, the assistant listens, processes and speaks the answer back in a voice of your choice.

[Using Voice Chat](voice-chat.md)

### Workflow Builder (Pro)

Import n8n workflows and let your assistant run them as a tool. Available via the Workflow Builder skill (Pro plan).

---

## Skills, the extensions

Skills add specific capabilities to your assistant. By default it can chat, plan and write text. With skills it can also:

- Send emails via Gmail
- Schedule appointments in Google Calendar
- Create social media posts
- Generate AI images
- Update spreadsheets
- Create invoices
- And dozens of other tasks

Skills are split into two categories: **Personal** (productivity, life) and **Business** (work, clients, marketing). Personal skills are in Starter+; business skills are included from Growth+, and the heaviest engines from Pro+. You pay per action in credits.

[Skills explained](skills-uitgelegd.md)
[Skills marketplace overview](../skills/README.md)

---

## Connectors, linking external services

Connect your assistant to external services via OAuth or API key. Connected services are available as tools for your assistant.

**OAuth connectors** (log in via consent screen):
- Google (Gmail, Calendar, Drive, Sheets, Docs, Tasks, Analytics, Search Console, Business Profile)
- Notion, Slack, LinkedIn, Airtable, Typeform, Calendly, Microsoft 365 _(coming soon)_, Canva _(coming soon)_

**API-key connectors** (enter credentials):
- WhatsApp Business, Instagram DM, Stripe, HubSpot

**Telegram** is a separate add-on, see [Telegram add-on](../integraties/telegram.md).

You manage connectors via **Connectors**.

---

## Credits, how the system works

Every interaction with your assistant uses credits. Credits are topped up monthly based on your plan. You can also buy extra.

| Plan | Credits/month | ~Tasks/month |
|---|---|---|
| Free | 1,000 |, |
| Starter | 75,000 | ~750 |
| Growth | 175,000 | ~1,750 |
| Pro | 350,000 | ~3,500 |
| Business | 1,000,000 | ~10,000 |

**What costs what?**

| Action | ~Credits |
|---|---|
| Simple chat message (Haiku) | 25-50 cr |
| Detailed message or analysis (Sonnet) | 100-200 cr |
| Generate an AI image | 250-1,500 cr |
| Read and reply to email | 50-150 cr |
| Voice Call answer (~500 chars) | ~1,375 cr |
| Transcribe audio (per minute) | 12-20 cr |

Monthly credits expire at the end of your billing period; purchased credit packs do not expire.

[Buy extra credits](../plannen-en-prijzen/credits-bijkopen.md)
[Credit system](../hoe-het-werkt/credits.md)

---

## Personalising your assistant

Your assistant is neutral by default. Via Settings you fully adapt it:

- **Name:** give it its own name
- **Communication style:** casual, formal, direct or detailed
- **Focus areas:** tick what is relevant for you (productivity, marketing, sales, etc.)
- **Personal instructions:** fixed rules that always apply, "always answer in bullet points", "use a formal tone for emails"
- **Knowledge document:** your personal profile, who you are, your company, how you work
- **Voice:** pick a voice for Voice Chat (Dutch or English voices available)

[More on context and memory](context-en-geheugen.md)
[Settings](../functies/instellingen.md)

---

## Telegram add-on

Telegram is not a required part of dGENIX, it is an optional add-on. If you activate it, your assistant also works via the Telegram app on your phone.

**What you can do via Telegram:**
- Ask text questions and give commands
- Send voice messages (transcribed automatically)
- Send photos (the assistant analyses them)
- Use the same skills as via the dashboard

Conversations are synced: what you send in Telegram is also visible in the dashboard.

[Activate the Telegram add-on](../integraties/telegram.md)

---

## Common commands

**Productivity:**
> "What's on my calendar tomorrow?"
> "Schedule a meeting with Jan on Thursday at 2pm"
> "Give me an overview of my unread emails"

**Content & communication:**
> "Write a LinkedIn post about our new service"
> "Draft a reply to client X's latest email"
> "Generate an AI image of a modern office"

**Business:**
> "Analyse last quarter's revenue in my Google Sheets"
> "Create a quote for a website project of €2,500"
> "Send a project summary to the Slack channel #team"

**Automation:**
> "Create a scheduled task: a weekly report of my calendar every Monday"
> "Every day at 9am: three priorities for today"

---

## Frequently asked questions

**My assistant forgets what I said last week, why?**
Per conversation session the assistant loads context (knowledge document, instructions, memory). Short facts or agreements you mention in a conversation are stored as memories, but not every detail of every conversation. Add important information to your knowledge document or personal instructions for permanent context.

**What's the difference between the knowledge document and memory?**
You write the knowledge document yourself: who you are, how you work, what your assistant should know. Memory is built automatically by the assistant from conversations, facts, preferences and patterns it remembers. Both are always loaded.

**Can I have multiple assistants?**
No, you have one assistant per account. But you can set your own instructions and context per project folder, so the assistant behaves differently depending on the project.

**Is my data used for AI training?**
No. Conversations and data are not used to train AI models.

**How do I stop a skill?**
Go to **Connectors** or **Account -> Subscription** and deactivate the skill or add-on. Credits already used are not refunded.

---

_Platform Manual, dGENIX | June 2026_
