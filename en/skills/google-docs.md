# Google Docs

Create, read, edit and summarise Google Docs via your AI assistant. No browser needed, the document link is returned directly.

**Requirements:** Growth+ plan, connect a Google account via Connectors

---

## Available actions

| Action | Credit cost | Description |
|---|---|---|
| `read_document` | 15 cr | Fetch a document by document ID or URL |
| `create_document` | 650 cr | Create a new document with full AI-generated content |
| `summarise_document` | 65 cr | Summarise a long document into key points |
| `edit_document` | 25 cr | Adjust or rewrite a specific section |

---

## Connecting

1. Go to **Connectors**
2. Click **Connect** on Google Docs
3. Log in with the Google account that owns the target documents
4. Grant permission for `documents` (read and write)

---

## Example conversations

**Create a document:**
> "Create a Google Doc with a detailed project description for our new webshop"

**Summarise a document:**
> "Summarise this document into 5 key points: docs.google.com/document/d/1abc123..."

**Edit a document:**
> "Rewrite the introduction of my quote document so it sounds more businesslike"

**Read a document:**
> "Pull the content of my strategy document: [document URL]"

---

## Tips

- `create_document` uses Claude Sonnet for the best writing quality (650 cr)
- Give the assistant context: audience, tone, desired length
- Use `summarise_document` for long reports before sharing them
- The returned document link is clickable in the chat

---

## Limitations

- Images and tables are not available via the API (text only)
- Google Forms are not supported
- Shared documents you do not own require explicit read access
