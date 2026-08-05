# Document Reader

With the Document Reader you have GENI read a web page or a block of text and answer from it: a summary, the key points, or the answer to one specific question.

Available from **Starter**. No connection needed.

## What can GENI do with it?

- **Analyse a document or web page** from a URL or from text you paste into the chat, answering the question you attach to it

One tool, but your question decides what you get back: summarise, pull out the
key points, compare two passages or look up one thing.

## Example: what you ask, what you get

```
Summarise these terms and tell me what stands out
[text pasted]
```

> **Summary , Supplier X terms and conditions**
>
> - Payment term **14 days**, then 2 percent interest per month
> - Notice period **three months**, only at the end of a quarter
> - Liability capped at the invoiced amount of the last 6 months
>
> **What stands out**
> - Article 9 allows a **unilateral** price increase with 30 days notice
> - There is no agreement on delivery time anywhere in the document

And from a URL:

```
https://example.com/research-2026 , what does it say about small business?
```

> The report mentions small business in two passages. The gist: 34 percent use
> AI weekly, against 71 percent at companies above 250 employees. The reason
> given is not price but the time it takes to set up.
>
> *Source: example.com/research-2026*

## Requirements

- **Plan:** Starter and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **Document Reader**
2. Paste a URL or the text into the chat and ask your question

## What it costs

| Action | Credits |
|---|---|
| Analyse a document or page | 5 |

The conversation itself comes on top; see
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **This skill works from a URL or pasted text.** To send a file along, use the attachment button in the chat , that runs through the chat itself, not through this skill.
- **Chat attachments:** images, PDF, txt, markdown and csv, up to **5 MB per file** and **3 files per message**.
- **A page behind a login or paywall cannot be fetched.** Paste the text instead.
- **Internal or private addresses are blocked.** Publicly reachable URLs only, which is a deliberate safety measure.
- **Very long documents are read partially.** Ask a specific question or supply the relevant section.
- **It does not store the document.** To search it again later, use the [Support Knowledge Base](knowledge-base.md).

## Troubleshooting

**"Failed to fetch URL".** The page blocks automated visits or asks for a login. Paste the text directly into the chat.

**"No usable content found".** The page builds its content with JavaScript, or it is a PDF behind a viewer. Copy the text across.

**The answer is too shallow.** Ask a sharper question. "What does it say about the notice period" yields more than "summarise".

**I want to find the document again later.** This skill cannot do that. Put it in the [Support Knowledge Base](knowledge-base.md) or keep the summary as a note in your [Workspace](../functies/werkruimte.md).

## Frequently asked questions

**Can I attach a PDF?**
Yes, through the attachment button in the chat (up to 5 MB). That runs through
the chat, not this skill, so you do not pay this skill's 5 credits for it.

**What is the difference with the Support Knowledge Base?**
This skill reads one thing, now. The [Knowledge Base](knowledge-base.md)
indexes your documentation so you can still search it months later.

**Does it work with a Google Docs link?**
With a publicly shareable link, yes. If the document is restricted, connect
[Google Drive](google-drive.md).

**Can it compare two documents?**
Yes, paste both and ask for the difference.

---

Back to [Skills marketplace](README.md)
See also: [Support Knowledge Base](knowledge-base.md) · [Google Drive](google-drive.md) · [Workspace](../functies/werkruimte.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Document Reader, updated August 2026*
