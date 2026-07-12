# Files & Images

Every file and image your assistant creates is kept in **Dashboard -> Files**.

---

## Tabs

### Files
Documents, exports and other generated files. View, download or delete files via the buttons next to each file.

### Images
AI-generated images via the [AI Image Generation skill](../skills/ai-beeldgeneratie.md).

Each image shows a thumbnail preview, the prompt used, the model used, credits spent and the date.

**Download:** click the download button to save the original image.
**Delete:** click the trash icon to remove an image permanently.

---

## Sending files in the chat

Click the attachment button in the AI Assistant to send a file. GENI reads the content and uses it directly in its answer.

| Type | Extensions | What GENI does |
|------|-----------|----------------|
| Images | `.jpg`, `.jpeg`, `.png`, `.webp`, `.gif` | Analyse visually |
| PDF | `.pdf` | Read the content |
| Text | `.txt`, `.md`, `.csv` | Read the content |
| Word | `.docx` | Extract and read the text |
| Excel | `.xlsx` | Extract and read the cells |
| Audio / video | `.mp3`, `.mp4`, `.webm`, `.wav`, `.m4a` | Transcribe (Whisper) and read |

**Audio/video** is transcribed automatically via Whisper. This costs **12 credits per minute** of audio; shorter clips cost proportionally less. Documents and images have no separate charge (just normal message usage).

For safety, files are validated server-side (type and content). `.json` files are refused. For larger documents or longer audio, use the **Knowledge base** or the **Audio Transcription** skill (URL, up to 200 MB).

---

## Uploading files to the knowledge base

Want to add a document as lasting knowledge (not just for one message)? Upload it via **AI Assistant -> Knowledge base -> Upload file**. The assistant searches your knowledge base whenever relevant.

---

## Storage

Files are kept as long as your account is active. On account deletion (Settings -> Privacy & Export) all files are permanently removed.
