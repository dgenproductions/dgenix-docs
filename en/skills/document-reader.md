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

## A PDF is genuinely read

Give it a link to a PDF and the file itself goes to the model. That is something
other than squeezing flat text out of it: **tables stay tables, columns do not run
into each other, and a scanned document is simply read.** Exactly the difference
between reading an invoice and guessing at it.

You do not have to switch anything on. If GENI sees the link is a PDF, it takes
that route automatically.

## What it costs

| Action | Credits |
|---|---|
| Analyse a web page or pasted text | 5 |
| Read a PDF | 10 per page, 25 minimum |

A single-page PDF therefore costs 25 credits, a twenty-page report 200. You pay for
what the model actually has to read. GENI mentions the price before opening a PDF.
The conversation itself comes on top; see
[The credit system](../hoe-het-werkt/credits.md).

**Or send the file along.** You can also attach the same PDF in the chat (paperclip,
up to 5 MB). That route does not run through this skill but through the conversation
itself, so you pay the normal conversation cost instead of a per-page price. A link
is handy when the file lives online; uploading is handy when you have it on your own
computer.

## Limits

- **PDF up to 25 pages and 10 MB.** Anything larger is refused with the reason, rather than read halfway. Split the document or say which part you mean.
- **Want to send a file instead of a link?** Use the attachment button in the chat , that runs through the chat itself, not through this skill.
- **Chat attachments:** images, PDF, txt, markdown and csv, up to **5 MB per file** and **3 files per message**.
- **A page behind a login or paywall cannot be fetched.** Paste the text instead.
- **Internal or private addresses are blocked.** Publicly reachable URLs only, which is a deliberate safety measure.
- **Very long documents are read partially.** Ask a specific question or supply the relevant section.
- **It does not store the document.** To search it again later, use the [Support Knowledge Base](knowledge-base.md).

## Troubleshooting

**"Failed to fetch URL".** The page blocks automated visits or asks for a login. Paste the text directly into the chat.

**"No usable content found".** The page builds its content with JavaScript, or the PDF sits behind a viewer instead of the link pointing at the file itself. Copy the text across, or give the direct link to the `.pdf`.

**"This PDF has roughly X pages".** Above 25 pages it will not read it in one go. Split the document, or ask for the part you need.

**The answer is too shallow.** Ask a sharper question. "What does it say about the notice period" yields more than "summarise".

**I want to find the document again later.** This skill cannot do that. Put it in the [Support Knowledge Base](knowledge-base.md) or keep the summary as a note in your [Workspace](../functies/werkruimte.md).

## Frequently asked questions

**Can I have a PDF read?**
Yes. Give a link to the `.pdf` and the file itself goes to the model, with tables
and scans intact. That costs 10 credits per page, up to 25 pages. If you would rather send
a file than a link, use the attachment button in the chat (up to 5 MB); that runs
through the chat, not this skill.

**Why is a PDF so much more expensive than a web page?**
Because there is far more to process. A page of text is a few thousand tokens, a
25-page PDF well over thirty thousand, and with a PDF the layout comes along too
so that tables stay correct. You pay for what the model actually reads.

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
