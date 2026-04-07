# Short Video Generator

Stuur een video-URL — je assistent analyseert de video, detecteert automatisch de beste fragmenten en maakt virale korte clips. Geschikt voor YouTube Shorts, Instagram Reels, TikToks en meer.

**Inbegrepen bij:** Starter, Growth, Pro, Custom

---

## Wat kan je assistent?

- **Highlight detectie** — AI analyseert het transcript en kiest automatisch de meest interessante of virale momenten
- **Clips renderen** — fragmenten worden gesneden en gerenderd in het formaat naar keuze
- **Meerdere clips tegelijk** — vraag meerdere clips van één video in één opdracht
- **Google Drive opslaan** — clips worden automatisch opgeslagen in je Drive (optioneel)
- **Captions** — automatisch ondertitels toevoegen aan de clips (optioneel)

**Ondersteunde video-bronnen:** YouTube, Instagram, TikTok, Vimeo, en directe video-URL's (MP4)

---

## Hoe werkt het?

De assistent werkt in twee stappen:

1. **Analyseer** — stuur een URL en je voorkeur. De assistent toont een schatting van het aantal clips, de duur en de creditkosten. Jij bevestigt.
2. **Genereer** — na bevestiging start de verwerking op de achtergrond. Je ontvangt een melding zodra je clips klaar zijn.

**Achtergrondverwerking:**
1. Video downloaden (yt-dlp)
2. Audio transcriberen (Whisper)
3. Beste fragmenten detecteren (Claude)
4. Clips renderen (FFmpeg)
5. Clips uploaden naar Supabase + optioneel Google Drive
6. Resultaat sturen via Telegram

---

## Clip-formaten

| Formaat | Gebruik |
|---------|---------|
| **9:16** | Instagram Reels, TikTok, YouTube Shorts (standaard) |
| **1:1** | Instagram posts, Facebook |
| **16:9** | YouTube, LinkedIn video |

---

## Creditkosten

**Formule:** `500 + (video_minuten × 90) + (clips × 150)`

| Voorbeeld | Video-lengte | Clips | Credits |
|-----------|-------------|-------|---------|
| Korte test | 5 min | 1 clip | ~1.000 cr |
| Standaard | 10 min | 3 clips | ~1.850 cr |
| Podcast-fragment | 30 min | 5 clips | ~3.950 cr |
| Lange video | 60 min | 10 clips | ~7.400 cr |

**Limieten:** maximaal 60 minuten per video, maximaal 10 clips per opdracht.

---

## Voorbeeldopdrachten

- "Maak een short van deze video: youtube.com/watch?v=..."
- "Clip de 3 beste momenten uit deze YouTube video in 9:16"
- "Maak 5 TikTok-clips van dit interview, sla ze op in mijn Drive"
- "Knip het beste fragment uit deze video en voeg ondertitels toe"
- "Genereer 2 clips van 30-60 seconden uit deze podcast aflevering"

---

## Google Drive integratie

Als Google Drive verbonden is via Instellingen → Integraties, kun je clips automatisch laten opslaan:

- Vermeld "sla op in Drive" of "in mijn Drive" in je opdracht
- De assistent vraagt om bevestiging als Drive niet gekoppeld is

→ [Google Drive koppelen](../integraties/google-drive.md)

---

## Problemen oplossen

**Verwerking duurt lang:**
- Langere video's duren langer — je ontvangt automatisch een Telegram-bericht zodra klaar

**Video niet ondersteund:**
- Controleer of de URL publiek toegankelijk is
- Privé YouTube-video's en leeftijdsbeperkte content worden niet ondersteund

**Credits niet voldoende:**
- Koop extra credits bij via [app.dgenix.com/billing](https://app.dgenix.com/billing)

---

→ [Terug naar Skills marketplace](README.md)
