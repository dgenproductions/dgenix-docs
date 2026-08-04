# Memory, knowledge base, knowledge document and projects compared

dGENIX has four places where GENI keeps information about you, and they look alike. This page puts them side by side so you know what belongs where.

The short version: the **knowledge document** says who you are, **memory**
remembers what GENI picks up along the way, the **knowledge base** holds your
documents, and a **project** keeps all of it separate per client or brand.

## The four in one table

| | Knowledge document | Memory | Knowledge base | Projects |
|---|---|---|---|---|
| **What it holds** | Who you are and how GENI should write | Individual facts, preferences and goals | Whole files as background knowledge | A separate workspace with its own context |
| **Who fills it** | You, during the intake | GENI itself, plus you | You, by uploading | You, per client or brand |
| **Shape** | One text | Individual entries, 8 types | PDFs, Word, text | Folder with its own instructions |
| **When used** | In every conversation | Whenever relevant | When you ask something it covers | Only inside that project |
| **Where** | Intake / Settings | Dashboard -> Memory | Dashboard -> Knowledge base | Dashboard -> Assistant |
| **Available from** | Every plan | Every plan | Growth | Growth |

## Knowledge document

You create the knowledge document once, during the intake. It is the foundation:
your company, your role, your tone, what you sell and to whom. GENI reads it in
*every* conversation, in every channel.

Use it for things that rarely change. "We are an installation company in Tilburg
with eight engineers" belongs here. "Call Jan back about the quote" does not.

You edit it via **Dashboard -> Settings**. Redo the intake and it gets rewritten.

## Memory

Memory is the only one of the four that fills itself. GENI stores what it learns
along the way and uses it later, including in a different channel. There are
eight types:

| Type | Example |
|---|---|
| Fact | "I work at a marketing agency in Amsterdam" |
| Preference | "I always want answers in bullet points" |
| Goal | "I want to halve my email response time" |
| Instruction | "Keep answers under 150 words" |
| Contact | "My regular designer is Lisa" |
| Pattern | "I always plan on Mondays" |
| Situation | "We are scaling up, team of 3" |
| Skills | "I am an expert copywriter, not a developer" |

You can add something yourself by simply saying it: *"Remember that my VAT
number is NL0012345B01."* Everything is viewable, editable and erasable via
**Dashboard -> Memory**.

See [Memory (Memory AI)](../functies/geheugen.md) for the full story.

## Knowledge base

The knowledge base is for **files**, not for individual facts. You upload a
product catalogue, a manual, your terms and conditions or an FAQ, and GENI
searches it whenever you ask something it covers.

The difference with memory: memory holds one sentence, the knowledge base holds
twenty pages. Ask "what is our lead time on custom work?" and GENI looks up the
answer in your uploaded documents and quotes from them.

See [Knowledge base](../functies/kennisbank.md).

## Projects

A project is a **walled-off workspace**. If you work for several clients or
brands, a project keeps the context per client apart: its own instructions, its
own conversations, its own memories.

That is exactly why agencies use it. Inside client A's project GENI knows nothing
about client B, so it never accidentally carries one client's tone of voice or
figures into another's work.

See [Projects](../functies/projecten.md).

## What you see

Say you are an installer and you filled all four. You ask:

```
Write a quote for Mrs De Vries for a heat pump
```

GENI then combines:

- from the **knowledge document**: that you are an installation company and write formally
- from **memory**: that your quotes are always valid for 30 days
- from the **knowledge base**: the prices and specifications from your product catalogue
- from the **project**: that this is client "De Vries", with the earlier correspondence

You get one quote back, not four separate answers. That is how they are meant to
work together.

## Which do you use for what?

- Almost never changes and always applies? -> **knowledge document**
- A single fact or preference? -> **memory**
- It lives in a file? -> **knowledge base**
- It must stay separate from other work? -> **project**

## Limits

- Memory is **strictly per user**. Nobody else can reach it, not even within the
  same company.
- Knowledge base and projects sit in **Growth** and up; knowledge document and
  memory are in every plan.
- GENI does not fill in the blanks. If the answer is not in your knowledge base,
  it says so instead of guessing.
- A project shares no memories with your general chat. That is by design, but it
  does mean you sometimes tell it something twice.

## Frequently asked questions

**Do I have to use all four?**
No. Knowledge document and memory come automatically. Knowledge base and
projects only matter once you have documents or work for several clients.

**What if memory and the knowledge document contradict each other?**
Memory is more specific and more recent, so it weighs more. If something is
structurally wrong, fix your knowledge document rather than correcting memory
over and over.

**Is my data used to train AI?**
No. Your data stays yours and is not used to train models.

**Can I wipe everything?**
Yes. You clear memory entry by entry or all at once via **Dashboard -> Memory**;
knowledge base files you delete one by one.

---

Next: [What is dGENIX](wat-is-dgenix.md) · [How it all fits together](hoe-alles-samenwerkt.md)
In depth: [Memory](../functies/geheugen.md) · [Knowledge base](../functies/kennisbank.md) · [Projects](../functies/projecten.md)
On the site: [how dGENIX works](https://dgenix.com/hoe-het-werkt) · [for agencies](https://dgenix.com/agencies)

*dGENIX Docs, Context storage compared, updated August 2026*
