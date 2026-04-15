# Audio Transcriptie

## Wat doet deze skill?

Zet audio-opnames automatisch om naar tekst via Fireworks Whisper v3. Stuur een URL naar een audio- of videobestand en ontvang een volledige transcriptie — optioneel met tijdstempels per segment en sprekersherkenning.

## Vereisten

- Plan: **Growth** of hoger
- Integraties: geen — werkt direct via URL

## Hoe activeer je de skill?

1. Ga naar **Skills** in je dashboard
2. Zoek **Audio Transcriptie** en klik op **Activeren**
3. De skill is direct beschikbaar via Telegram en de web-assistent

## Wat kun je ermee?

- Vergaderingsopname transcriberen naar notulen
- Interview uitschrijven met tijdstempels per fragment
- Podcast-aflevering omzetten naar blogtekst of social content
- Spraaknotities verwerken naar gestructureerde tekst

**Voorbeeldopdrachten:**

- "Transcribeer dit gesprek: [URL]"
- "Schrijf dit interview uit met tijdstempels: [URL]"
- "Transcribeer in het Engels met sprekersherkenning: [URL]"

## Ondersteunde formaten

MP3, WAV, M4A, OGG, FLAC, WebM — maximaal 200 MB per bestand.

## Modellen

| Model | Snelheid | Nauwkeurigheid | Creditkosten |
| --- | --- | --- | --- |
| **Turbo** (standaard) | Snel | Goed | 12 cr/min |
| **Large** | Langzamer | Maximaal | 20 cr/min |

Diarisering (sprekersherkenning) kost 40% extra credits.

## Creditkosten

Credits worden berekend op basis van de **werkelijke duur** van het audiobestand — niet op een schatting. Na de transcriptie worden de exacte credits afgeschreven.

**Voorbeelden:**

| Duur | Model | Credits |
| --- | --- | --- |
| 5 minuten | Turbo | 60 cr |
| 10 minuten | Turbo | 120 cr |
| 30 minuten | Large | 600 cr |
| 60 minuten | Large + diarisering | 1.680 cr |

## Taaldetectie

Zonder opgegeven taal detecteert de transcriptie automatisch de taal van het gesprek. Geef optioneel een taalcode mee voor hogere nauwkeurigheid bij duidelijk bekende talen (bijv. `nl`, `en`, `de`).

---

→ [Terug naar Skills marketplace](README.md)
