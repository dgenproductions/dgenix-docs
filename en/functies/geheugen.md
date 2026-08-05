# Memory (Memory AI)

GENI's memory is the connective tissue of dGENIX. Everything you do on the platform automatically flows into your assistant's memory, so GENI knows your work, thinks along and builds on earlier work. Your memory is strictly private and only yours.

The Memory page (**Dashboard → Memory**, Brain icon in the sidebar) gives you direct insight into everything GENI remembers about you.

---

## One connected memory

Memory consists of three layers that work together:

1. **What GENI knows about you**: facts, preferences, goals and instructions you add yourself or that GENI picks up from your conversations.
2. **What you do on the platform**: every image, audit, transcript, completed task and automation run automatically lands in your memory. So GENI knows what you're working on.
3. **Your documents and notes**: your knowledge base and your Workspace notes are searchable and connected to the same memory.

GENI reaches the same memory on every channel: the dashboard, Telegram, voice calls and scheduled tasks.

---

## What are memories?

Memories are short, personal facts GENI uses as context. There are eight types:

| Type | Example |
| --- | --- |
| **Fact** | "I work at a marketing agency in Amsterdam" |
| **Preference** | "Always give answers in bullet points" |
| **Goal** | "I want to halve my email response time" |
| **Instruction** | "Keep answers under 150 words" |
| **Contact** | "My regular designer is Lisa" |
| **Pattern** | "I always plan on Mondays" |
| **Context** | "We're in a growth phase, team of 3" |
| **Skills** | "I'm an expert copywriter, not a developer" |

Facts, preferences, goals and instructions appear as nodes around the brain at the top of the page; all types appear as expandable rows below it.

---

## Ask your memory (semantic search)

With the "Ask your memory" search bar you search everything GENI knows about you by **meaning**, not by keyword. Type "what do you know about my writing style?" and GENI brings back the relevant memories, even if you used different words than the ones in the memory.

> Smart search uses AI and costs a small amount of credits per search. Available from Starter.

---

## What GENI learned about you (activity)

The activity timeline shows what you recently did on the platform, from generated images to completed audits and tasks. This is what GENI automatically noticed and carries into its context, so you can ask things like "continue with yesterday's SEO audit".

---

## Per brand or project (brand switching)

Working across multiple brands or clients? Create a project in the AI Assistant and GENI keeps memory separated per project. At the top of the Memory page you switch between your **Main memory** and your projects. What you add inside a project stays tied to that project and never leaks into your other work.

---

## Proactive GENI (optional)

Turn on **Proactive GENI** (in **Settings → AI assistant**) and GENI thinks along once a day based on what you did: it stages suggested follow-up tasks in your Workspace and sends a short update. Off by default, no spam, always for you to approve.

---

## Adding, editing and deleting memories

- **Add**: via the input bar (pick a type, optional title, type the content) or simply by saying it in chat: *"Remember that I start every morning with my inbox."* GENI then saves it with the `geheugen_opslaan` tool.
- **Edit**: click the pencil icon next to a memory.
- **Delete**: click the trash icon. From the Manage bar you can also select several at once, import/export (JSON) or archive to your knowledge base.

---

## Knowledge document

At the bottom of the page you'll find a summary of your knowledge document, the personal context from **Settings → Knowledge document**. This acts as long-term memory: it's always present in your assistant's context, regardless of your plan.

---

## What you can do with it

| What you do | What GENI does with it |
|---|---|
| Mention something in a conversation | Stores it if it stays relevant later |
| Say "remember that..." | Records it as a memory straight away |
| Ask about earlier work | Searches your memory and activity by meaning |
| Switch to a project | Uses that project's memories first |
| Correct a memory | Adjusts or discards it, you stay in control |

## What you see

You work with GENI for a few weeks and then ask something you never explicitly
told it:

```
Write a quote for Mrs De Vries
```

> I drafted the quote using what I know about you:
>
> - **formal tone**, as you prefer
> - **valid for 30 days**, your standard
> - your **VAT number and bank details** at the bottom
> - issued from **Installatiebedrijf Jansen**
>
> I took the prices from your catalogue. Shall I prepare it as a PDF?

None of that was in your request. That is the difference between a chat window
and an assistant that knows you.

## Limits

- **Your memory is strictly yours.** Nobody else can reach it, not even within the same company.
- **GENI does not fill in the blanks.** If it does not know something, it asks rather than guesses.
- **A wrong memory keeps having effect** until you fix it. If something is structurally off, correct your knowledge document instead of steering every time.
- **The storage limit depends on your plan**: 100 on Free and Starter, 500 on Growth, 2,000 on Pro, 5,000 on Business.
- **At the limit GENI archives** the least important memories to your knowledge base itself; nothing is simply lost.
- **Project memories stay in that project.** That is by design, but it means you sometimes say something twice.
- **Semantic search sits in Starter and up.** On Free memory works, just without searching by meaning.

## Troubleshooting

**GENI no longer knows something.** Check the Memory page to see whether it is there. If not, say it again with "remember that...".

**It uses outdated information.** Find the memory and edit or delete it; adding a new one leaves the old in place.

**It mixes up clients.** Client-specific facts belong in a [project](projecten.md), not in your general memory.

**You have hit the limit.** GENI archives to your knowledge base itself. To clear space yourself, delete outdated memories on the Memory page.

**Too much is being stored.** You can delete any memory, and "clear all memories" starts you over.

## Frequently asked questions

**What flows into my memory automatically?**
Everything you create or do on the platform: images, transcripts, SEO/GEO audits, completed tasks and automations. Plus the facts GENI picks up from your conversations.

**Are memories visible to others?**
No. Your memory is fully private and strictly tied to your account, never shared or mixed with other users.

**How much can I store?**
Depends on your plan (from 100 on Free and Starter up to 5,000 on Business). At the limit GENI automatically archives the least important memories to your knowledge base.

---

Next: [Workspace](werkruimte.md) · [Projects](projecten.md) · [Knowledge base](kennisbank.md)
On the site: [all skills](https://dgenix.com/skills) · [pricing](https://dgenix.com/pricing)

*dGENIX Docs, Memory (Memory AI), updated August 2026*
