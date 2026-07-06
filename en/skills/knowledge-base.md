# Support Knowledge Base

## What does this skill do?

Add your own knowledge articles, FAQs and manuals to your assistant. It then answers questions based on your own documentation, accurately and always up to date.

## Requirements

- **Plan:** Pro
- **Integrations:** no extra connections needed

## How do you activate the skill?

1. Go to **Skills** in your dashboard
2. Find **Support Knowledge Base** and click Activate
3. Go to **Files** in your dashboard to add documents
4. Ask your assistant: "Add [document] to my knowledge base"

## What can you do with it?

**Example commands:**

- "Add this PDF manual to my knowledge base"
- "What does my onboarding documentation say about billing?"
- "Answer the customer's question based on my FAQ"

**What the assistant does:**

**Add a document:**
1. Processes the document into chunks
2. Computes semantic embeddings (OpenAI text-embedding-3-small)
3. Stores it in the vector database, ready for search

**Answer a question:**
1. Finds the most relevant chunks in your knowledge base
2. Composes the answer from your own documents
3. Indicates which document the answer comes from

## Credit cost

| Action | Credits |
| --- | --- |
| Add a document to the knowledge base | 50 cr/document |
| Answer a question via the knowledge base | 200 cr |

---

## Pricing

Included in **Pro** and **Custom**, no extra monthly cost for the skill.

---

Back to [Skills marketplace](README.md)
