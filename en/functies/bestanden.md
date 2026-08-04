# Files and images

Everything GENI makes for you, and everything you send it, comes together in **Dashboard -> Files**.

Those are two different things: files you **send** in a conversation GENI uses on
the spot, and files it **creates** are kept so you can download them later.

## What you can do with it

| What you do | What happens |
|---|---|
| Send a photo | GENI looks at it and describes or assesses what is in it |
| Send a PDF | It reads the content and answers your question about it |
| Send a spreadsheet | It reads the cells and calculates or summarises |
| Send a voice note | It transcribes and works with the content |
| Have an image generated | It appears under the Images tab, ready to download |

## Sending files in the chat

Click the attachment button in the assistant and pick a file. GENI reads the
content and uses it straight away in its answer.

| Type | Extensions | What GENI does |
|---|---|---|
| Images | `.jpg`, `.jpeg`, `.png`, `.webp`, `.gif` | Analyse visually |
| PDF | `.pdf` | Read the content |
| Text | `.txt`, `.md`, `.csv` | Read the content |
| Word | `.docx` | Extract and read the text |
| Excel | `.xlsx` | Extract and read the cells |
| Audio and video | `.mp3`, `.mp4`, `.webm`, `.wav`, `.m4a` | Transcribe and read |

**Audio and video** are transcribed automatically. That costs **12 credits per
minute**; a short clip costs proportionally less. Documents and images cost
nothing extra, just normal message usage.

## What you see

You attach a photo of an invoice and ask what the total is:

> This invoice shows a total of **€1,247.50** including VAT.
>
> - Subtotal: €1,030.99
> - VAT 21%: €216.51
> - Due date: 14 August 2026
>
> Shall I add it to your Workspace as a task "pay before 14 August"?

It works that way for every type: you do not get a raw text dump but an answer
to the question you asked.

## The Images tab

Images GENI generates end up here, each with the prompt used, the model, the
credits spent and the date. Download with the download button, remove with the
trash icon.

See [AI image generation](../skills/ai-beeldgeneratie.md).

## Safety

Every attached file is validated server-side, on type and on content, so a file
cannot be something other than its extension promises. `.json` files are
refused.

## Limits

- **An attachment applies to that one conversation.** To make a document permanently available, use the [Knowledge base](kennisbank.md).
- **Up to three files per message.**
- **There is a maximum file size.** For larger documents or longer audio use the Knowledge base or the [Audio Transcription](../skills/transcriptie.md) skill, which handles up to 200 MB through a URL.
- **`.json` is not accepted.**
- **A scanned PDF without a text layer yields nothing**; there is no text to extract.
- **GENI does not edit your file.** It reads it and answers; the original stays untouched.

## Troubleshooting

**The file is refused.** Check the extension against the table above. `.json` is deliberately not accepted, and neither is a file whose content does not match its extension.

**GENI says it cannot read the PDF.** Probably a scan without a text layer. Run it through an OCR tool.

**Transcription costs more credits than expected.** The price runs per minute of audio, so a long recording adds up. Check the length beforehand.

**An image is not in the overview.** The Images tab only shows what GENI generated itself, not what you sent.

**The file is too large.** Use the Knowledge base for documents or the transcription skill for long audio.

## Storage

Files are kept as long as your account is active. If you delete your account via
**Settings -> Privacy and export**, all files are permanently removed.

## Frequently asked questions

**Can GENI create a file for me?**
Yes, such as PDF reports from the engines and CSV exports. Those land under the
Files tab.

**Is an attached file kept?**
It belongs to that conversation. To use it as lasting knowledge, upload it to
the knowledge base.

**Can anyone else reach my files?**
No. Files sit on your account.

**Is the content used to train AI?**
No.

---

Next: [Knowledge base](kennisbank.md) · [AI assistant](ai-assistent.md) · [Workspace](werkruimte.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Files and images, updated August 2026*
