# Short Generator

Send a video URL and your assistant analyses the video, automatically detects the best moments and makes viral short clips. Suitable for YouTube Shorts, Instagram Reels, TikToks and more.

**Available from:** Starter and up, included at no extra monthly cost

---

## What can your assistant do?

- **Highlight detection**, AI analyses the transcript and automatically picks the most interesting or viral moments
- **Render clips**, moments are cut and rendered in the format you choose
- **Multiple clips at once**, request several clips from one video in a single command
- **Save to Google Drive**, clips are saved to your Drive automatically (optional)
- **Captions**, add subtitles to the clips automatically (optional)

**Supported sources:** YouTube, Instagram, TikTok, Vimeo and direct video URLs (MP4)

---

## How does it work?

The assistant works in two steps:

1. **Analyse**, send a URL and your preference. The assistant shows an estimate of the number of clips, duration and credit cost. You confirm.
2. **Generate**, after confirmation, processing runs in the background. You get a notification when your clips are ready.

**Background processing:** download (yt-dlp) -> transcribe (Whisper) -> detect best moments (Claude) -> render (FFmpeg) -> upload to storage + optional Google Drive -> notify.

---

## Clip formats

| Format | Use |
|---------|---------|
| **9:16** | Instagram Reels, TikTok, YouTube Shorts (default) |
| **1:1** | Instagram posts, Facebook |
| **16:9** | YouTube, LinkedIn video |

---

## Credit cost

**Formula:** `500 + (video_minutes × 90) + (clips × 150)`

| Example | Length | Clips | Credits |
|-----------|-------------|-------|---------|
| Short test | 5 min | 1 clip | ~1,000 cr |
| Standard | 10 min | 3 clips | ~1,850 cr |
| Podcast excerpt | 30 min | 5 clips | ~3,950 cr |
| Long video | 60 min | 10 clips | ~7,400 cr |

**Limits:** max 60 minutes per video, max 10 clips per command.

---

## Example commands

- "Make a short from this video: youtube.com/watch?v=..."
- "Clip the 3 best moments from this YouTube video in 9:16"
- "Make 5 TikTok clips from this interview, save them to my Drive"
- "Cut the best moment from this video and add subtitles"

---

## Google Drive integration

If Google Drive is connected via Connectors, clips can be saved automatically: mention "save to Drive" in your command. The assistant asks for confirmation if Drive is not connected.

[Google Drive connector](../connectors/google-drive.md)

---

## Troubleshooting

- **Processing takes a while:** longer videos take longer, you get a notification when done
- **Video not supported:** check that the URL is publicly accessible; private or age-restricted videos are not supported
- **Not enough credits:** buy extra credits via your dashboard

---

## Pricing

Included from **Starter** and up, no extra monthly cost for the skill. Credit cost per video: see the table above.

---

Back to [Skills marketplace](README.md)
