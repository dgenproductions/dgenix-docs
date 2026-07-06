# Audio Transcription

## What does this skill do?

Automatically convert audio recordings to text via Fireworks Whisper v3. Send a URL to an audio or video file and receive a full transcription, optionally with timestamps per segment and speaker recognition.

## Requirements

- Plan: **Growth** or higher
- Integrations: none, works directly via URL

## How do you activate the skill?

1. Go to **Skills** in your dashboard
2. Find **Audio Transcription** and click **Activate**
3. The skill is available right away via Telegram and the web assistant

## What can you do with it?

- Transcribe a meeting recording into minutes
- Write out an interview with timestamps per fragment
- Turn a podcast episode into a blog post or social content
- Process voice notes into structured text

**Example commands:**

- "Transcribe this conversation: [URL]"
- "Write out this interview with timestamps: [URL]"
- "Transcribe in English with speaker recognition: [URL]"

## Supported formats

MP3, WAV, M4A, OGG, FLAC, WebM, up to 200 MB per file.

## Models

| Model | Speed | Accuracy | Credit cost |
| --- | --- | --- | --- |
| **Turbo** (default) | Fast | Good | 12 cr/min |
| **Large** | Slower | Maximum | 20 cr/min |

Diarisation (speaker recognition) costs 40% extra credits.

## Credit cost

Credits are calculated on the **actual duration** of the audio file, not an estimate. After transcription the exact credits are charged.

**Examples:**

| Duration | Model | Credits |
| --- | --- | --- |
| 5 minutes | Turbo | 60 cr |
| 10 minutes | Turbo | 120 cr |
| 30 minutes | Large | 600 cr |
| 60 minutes | Large + diarisation | 1,680 cr |

## Language detection

Without a specified language the transcription detects the language automatically. Optionally pass a language code for higher accuracy on clearly known languages (e.g. `nl`, `en`, `de`).

---

Back to [Skills marketplace](README.md)
