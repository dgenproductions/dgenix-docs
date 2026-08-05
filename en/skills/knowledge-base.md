# Support Knowledge Base

With the Support Knowledge Base GENI indexes your documentation and answers questions from it, stating the source.

Available from **Pro**. No connection needed.

## What can GENI do with it?

- **Index a document** into your personal knowledge base
- **Answer a question** based on what has been indexed

The difference with simply asking: it searches *your* documents and says where
the answer came from. If it is not in there, it says so instead of inventing
something plausible.

## Example: what you ask, what you get

```
What is our warranty period on installations?
```

> Installations carry a **two-year warranty** on materials and fitting, counted
> from the delivery date.
>
> Exceptions:
> - Wear parts are excluded from the warranty
> - Without the annual service, the warranty lapses after one year
>
> *Source: Terms and conditions 2026.pdf, article 8*

That source line is the point. On a support question you want to check where the
answer came from before passing it to a customer.

## Requirements

- **Plan:** Pro and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **Support Knowledge Base**
2. Add your documents
3. Ask your question

## What it costs

| Action | Credits |
|---|---|
| Add a document, per document | 50 |
| Answer a question | 200 |

Indexing happens once per document; answering is the recurring cost. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI does not fill in the blanks.** If the answer is not in your documents, it says so.
- **Only text is read.** Images, schematics and diagrams are not interpreted.
- **A scanned PDF without a text layer yields nothing.**
- **Updating means re-indexing.** You replace a changed document; it does not notice a change by itself.
- **Your knowledge base is yours.** Nothing is shared between users.
- **No source, no answer.** That is deliberate: on support questions a guess is worse than no answer.

## Troubleshooting

**It says the answer is not there.** Check that the document really is indexed and that your question matches the wording in the text.

**The answer comes from an outdated document.** Delete the old version; adding a new one leaves the old in place and they compete.

**Indexing fails.** Probably a scanned PDF without a text layer. Run it through an OCR tool.

**The answer is too short.** Ask for the full passage or for the article it refers to.

## Frequently asked questions

**What is the difference with the knowledge base in the Workspace?**
The [knowledge base](../functies/kennisbank.md) is general background knowledge
GENI uses everywhere. This skill targets support questions: one question, one
answer, with a source.

**Can I use this for customer questions?**
Yes, that is the intent. Note though: GENI answers *your* question; what you
pass on to the customer is your call.

**How many documents can I add?**
Enough for normal use. Quality counts more: five current documents work better
than thirty overlapping versions.

**Is my documentation used to train AI?**
No.

---

Back to [Skills marketplace](README.md)
See also: [Knowledge base](../functies/kennisbank.md) · [Document Reader](document-reader.md) · [AI Receptionist](ai-receptionist.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Support Knowledge Base, updated August 2026*
