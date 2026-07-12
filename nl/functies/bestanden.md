# Bestanden & Afbeeldingen

Alle bestanden en afbeeldingen die je assistent aanmaakt, worden bewaard in **Dashboard → Bestanden**.

---

## Tabbladen

### Bestanden
Documenten, exports en andere gegenereerde bestanden. Bekijk, download of verwijder bestanden via de knoppen naast elk bestand.

### Afbeeldingen
AI-gegenereerde afbeeldingen via de [AI Beeldgeneratie skill](../skills/ai-beeldgeneratie.md).

Elke afbeelding toont:
- Thumbnail preview
- Gebruikte prompt
- Gebruikte model
- Credits verbruikt
- Aanmaakdatum

**Downloaden:** klik de downloadknop om de originele afbeelding op te slaan.
**Verwijderen:** klik het prullenbakicoon om een afbeelding permanent te verwijderen.

---

## Bestanden meesturen in de chat

Klik op de bijlage-knop in de AI Assistent om een bestand mee te sturen. GENI leest de inhoud en gebruikt die direct in zijn antwoord.

| Type | Extensies | Wat GENI ermee doet |
|------|-----------|---------------------|
| Afbeeldingen | `.jpg`, `.jpeg`, `.png`, `.webp`, `.gif` | Visueel analyseren |
| PDF | `.pdf` | Inhoud lezen |
| Tekst | `.txt`, `.md`, `.csv` | Inhoud lezen |
| Word | `.docx` | Tekst uitlezen en lezen |
| Excel | `.xlsx` | Cellen uitlezen en lezen |
| Audio / video | `.mp3`, `.mp4`, `.webm`, `.wav`, `.m4a` | Transcriberen (Whisper) en lezen |

**Audio/video** wordt automatisch getranscribeerd via Whisper. Dit kost **12 credits per minuut** audio; kortere fragmenten kosten navenant minder. Documenten en afbeeldingen kosten geen aparte kosten (alleen het gewone berichtverbruik).

Voor veiligheid worden bestanden server-side gecontroleerd (type én inhoud). `.json`-bestanden worden geweigerd. Voor grotere documenten of langere audio kun je de **Kennisbank** of de **Audio Transcriptie**-skill (URL, tot 200 MB) gebruiken.

---

## Bestanden uploaden naar de kennisbank

Wil je een document blijvend als kennis toevoegen (niet alleen voor één bericht)? Upload het via **AI Assistent → Kennisbank → Bestand uploaden**. De assistent doorzoekt je kennisbank wanneer dat relevant is.

---

## Opslag

Bestanden worden opgeslagen zolang je account actief is. Bij accountverwijdering (Settings → Privacy & Export) worden alle bestanden permanent verwijderd.
