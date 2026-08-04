# Knowledge base

The knowledge base is where you put whole files for GENI to use as background knowledge: your product catalogue, your terms, your manual.

That way you never have to explain what you sell or how you work again. Ask
something covered by an uploaded document and GENI looks the answer up there and
quotes from it. Available from **Growth**.

## What you can do with it

| What you upload | What GENI does with it |
|---|---|
| Product catalogue or price list | Quotes and answers with the right prices |
| Terms and conditions | Answering questions on lead times, warranty and payment |
| Manual or FAQ | Backing support answers with your own wording |
| Company profile | Writing copy that matches what you actually do |
| Client briefing | Working within that project's agreements |

## Knowledge base, memory or knowledge document?

These three look alike and that is the most common confusion:

- **Memory** holds one sentence ("my VAT number is NL0012345B01")
- **Knowledge document** describes who you are and how GENI writes
- **Knowledge base** holds twenty pages, and GENI searches it when needed

See [Context storage compared](../concepten/context-opslag-vergeleken.md) for the
full comparison.

## How it works

1. Go to **Dashboard -> Assistant -> Knowledge base**
2. Click **Upload file**
3. Pick a PDF, Word file, text file or markdown file
4. The file is processed, usually within a minute
5. GENI consults it from then on whenever a question calls for it

| Type | Extension |
|---|---|
| PDF | `.pdf` |
| Word | `.docx` |
| Text | `.txt` |
| Markdown | `.md` |

## What you see

You upload your price list and then ask:

```
What is our lead time on custom work?
```

> Custom work has a lead time of **4 to 6 weeks**, counted from approval of the
> quote. Rush orders carry a 15 percent surcharge and bring the lead time down
> to 2 weeks.
>
> *Source: Terms and conditions 2026.pdf*

Without a knowledge base GENI would have had to ask what your lead time is. Now
it takes the answer from your own document and says where it came from.

## Per project or account-wide

You can upload files at two levels:

- **At account level**, applying to all your conversations
- **Inside a project**, where GENI uses it only there

The second is why agencies work this way: client A's catalogue never ends up in
work for client B. See [Projects](projecten.md).

## Limits

- **GENI does not fill in the blanks.** If the answer is not in your files, it says so instead of guessing.
- **Only text is read.** Images and diagrams inside a PDF are not interpreted.
- **A scanned PDF without a text layer yields nothing**, because there is no text to extract.
- **Updating means re-uploading.** You replace a changed file; GENI does not notice a change by itself.
- **Files are not shared.** Your knowledge base is yours, even within the same company.
- **The knowledge base sits in Growth and up.** On Free and Starter you use memory and the knowledge document.

## Troubleshooting

**GENI does not use the file.** Make your question more specific. It searches on content, so "what is our lead time" works better than "tell me about our company".

**The answer comes from the wrong file.** If the same information sits in two documents, delete the outdated one.

**Processing fails.** Probably a scanned PDF without a text layer. Run it through an OCR tool or upload the source text.

**You cannot see the knowledge base.** It sits in Growth and up; on a lower plan the section is not visible.

**An old answer keeps coming back.** Actually delete the old file; uploading a new version leaves the old one in place.

## Deleting files

Go to **Dashboard -> Assistant -> Knowledge base**, click the file and choose
**Delete**. It is gone immediately and GENI can no longer reach it.

## Frequently asked questions

**How many files can I upload?**
Enough for normal use. Quality counts more than quantity: five good, current
documents work better than thirty overlapping versions.

**Is my data used to train AI?**
No. Your files stay yours and are not used to train models.

**Does it cost credits?**
Uploading and searching are included in your plan. Only the conversation itself
uses credits, like any message.

**Can I see which file produced an answer?**
Yes, GENI names the source it quotes from.

**What is the difference with attaching a file in chat?**
An attachment applies to that one conversation. The knowledge base is lasting,
and GENI searches it on its own. See [Files](bestanden.md).

---

Next: [Context storage compared](../concepten/context-opslag-vergeleken.md) · [Projects](projecten.md) · [Memory](geheugen.md)
On the site: [all skills](https://dgenix.com/skills) · [pricing](https://dgenix.com/pricing)

*dGENIX Docs, Knowledge base, updated August 2026*
