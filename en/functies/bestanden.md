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

## Uploading files (for the assistant)

Files you want to give your assistant as context are uploaded via:
**AI Assistant -> Knowledge base tab -> Upload file**

Supported formats:
| Type | Extensions |
|------|-----------|
| PDF | `.pdf` |
| Word | `.doc`, `.docx` |
| Images | `.jpg`, `.jpeg`, `.png`, `.webp` |

The assistant reads the content and uses it as context in its answer. Images are analysed visually.

---

## Supported file types (overview)

| Type | Supported | Note |
|------|-------------|-------------|
| PDF | ✅ | Upload as context |
| Word (.docx) | ✅ | Upload as context |
| Excel (.xlsx) | Via Google Sheets | Use the Google Sheets skill |
| Images (JPG/PNG) | ✅ | Upload + AI Image Generation |
| Video | ❌ | Not supported for upload |
| Voice/audio | Via Telegram or transcription | Send voice messages, or use the Audio Transcription skill |

---

## Storage

Files are kept as long as your account is active. On account deletion (Settings -> Privacy & Export) all files are permanently removed.
