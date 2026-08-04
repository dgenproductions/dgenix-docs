# Context and memory

Your assistant knows who you are, how you work and what matters to you, not because you tell it each time, but because it builds context from several sources. This document explains how that system works.

---

## How does the assistant load context?

Before every conversation your assistant automatically combines these information sources:

```
[Platform knowledge] + [Knowledge document] + [Personal instructions] + [Memory] + [Knowledge base] + [Project instructions]
```

All of it is available the moment you send a message. You do not activate anything, it works automatically.

---

## 1. Knowledge document

The knowledge document is the most important thing your assistant knows about you. It is created during the intake and contains your profile:

- Who you are and what you do
- Your company, sector and role
- How you want to work and communicate
- What your assistant should know about you

**Where to find it:**
- Dashboard -> Assistant (collapsed accordion at the top of the chat)
- Settings -> AI Assistant -> Knowledge document

**How to edit it:** click "Edit" in the accordion. Adjust the text and save, your assistant uses the new version from the next conversation.

**Tip:** the more relevant information here, the better your assistant is tuned to you. Add your company name, sector and audience, your way of working and style preference, fixed formats you use, and people who recur in your work.

**File format:** the knowledge document is a `.md` file (Markdown), plain text with optional formatting. You do not need to know Markdown, plain text reads fine too.

---

## 2. Personal instructions

Personal instructions are fixed rules your assistant always follows, regardless of the conversation or project. They are not overridden by other context.

**Examples:**
- "Always answer in bullet points, never long paragraphs"
- "Use a professional tone for emails, but informal for Slack messages"
- "When I ask about marketing, always use the AIDA structure"

**Where to set them:** Settings -> AI Assistant -> Personal instructions

Write them the way you would explain them to a new colleague.

---

## 3. Memory

Memory is your assistant's automatic knowledge build-up. After conversations it stores relevant facts, with no effort from you.

**What it remembers:**
- **Facts**, who you are, your role, your company
- **Preferences**, how you communicate, which tools you use
- **Contacts**, people who recur
- **Patterns**, recurring ways of working or habits

**How long is it kept?** Until you delete it.

**Manage:** Settings -> Memory, view, delete or export memories.

For more detail see [Memory](../functies/geheugen.md).

---

## 4. Knowledge base, uploading documents

The Knowledge base is for documents your assistant should know as background. Unlike memory (automatic), you fill this yourself.

**Supported formats:** `.md`, `.pdf`, `.docx`, `.txt`

**Using .md files effectively:**

Markdown files are ideal for knowledge base documents because they are easy to write and structure. Example:

```markdown
# Company profile, De Krent Bakery

## Products
- Sourdough bread: €4.50
- Croissants: €1.80 each

## Opening hours
Tuesday to Saturday: 07:30-17:00
Sunday: 08:00-13:00

## Communication style
Warm and personal. Customers are regulars.
```

The assistant reads this file and uses the information for questions like "Write a reply to a complaint about an order".

**Where to upload:** Dashboard -> Assistant -> "Knowledge base" tab

For more detail see [Knowledge base](../functies/kennisbank.md).

---

## 5. Project instructions

Per project folder you can set your own instructions. They apply only to conversations within that project and combine with your global knowledge document.

**How to set:**
1. Go to Dashboard -> Assistant
2. Hover over a project folder in the sidebar
3. Click the gear icon
4. Type the instructions and save

For more detail see [Projects](../functies/projecten.md).

---

## All in one view

| Source | Created by | Purpose | Scope |
|---|---|---|---|
| Knowledge document | You (intake + editing) | Your profile and way of working | Always active |
| Personal instructions | You | Fixed behaviour rules | Always active |
| Memory | Assistant (automatic) | Facts from conversations | Always active |
| Knowledge base | You (uploading) | Background knowledge | Always active (Growth+) |
| Project instructions | You | Client- or project-specific context | Only in that project |

**Priority:** when instructions clash, more specific sources win. Project instructions override nothing, they are combined. Personal instructions always apply.

---

## Practical tips

**Start with a good knowledge document.** This is the investment with the highest payoff. Fill in who you are, what you do, who you work for and how your assistant should communicate.

**Use project instructions for repeat clients.** Create one project per regular client and set the context once.

**Add .md files to your Knowledge base for recurring information.** Price list, product catalogue, standard answers, upload them once and the assistant always uses them.

**Check your memory periodically.** Remove outdated items via Settings -> Memory.

**Write personal instructions as rules, not wishes:** "Always give three options" instead of "Preferably give three options".

---

Next: [Context storage compared](../concepten/context-opslag-vergeleken.md) · [Memory](../functies/geheugen.md) · [Knowledge base](../functies/kennisbank.md) · [Projects](../functies/projecten.md)
On the site: [how dGENIX works](https://dgenix.com/hoe-het-werkt)

*dGENIX Docs, Context and memory, updated August 2026*
