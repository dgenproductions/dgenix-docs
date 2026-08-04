# Bestanden en afbeeldingen

Alles wat GENI voor je maakt, en alles wat je hem meestuurt, komt samen in **Dashboard → Bestanden**.

Dat zijn twee verschillende dingen: bestanden die je **meestuurt** in een gesprek
gebruikt GENI ter plekke, en bestanden die hij **maakt** blijven bewaard zodat je
ze later kunt downloaden.

## Wat je hiermee kunt

| Wat je doet | Wat er gebeurt |
|---|---|
| Een foto meesturen | GENI bekijkt hem en beschrijft of beoordeelt wat erop staat |
| Een PDF meesturen | Hij leest de inhoud en beantwoordt je vraag erover |
| Een spreadsheet meesturen | Hij leest de cellen en rekent of vat samen |
| Een spraakmemo meesturen | Hij transcribeert het en verwerkt de inhoud |
| Een afbeelding laten maken | Die verschijnt onder het tabblad Afbeeldingen, klaar om te downloaden |

## Bestanden meesturen in de chat

Klik op de bijlage-knop in de assistent en kies een bestand. GENI leest de
inhoud en gebruikt die meteen in zijn antwoord.

| Type | Extensies | Wat GENI ermee doet |
|---|---|---|
| Afbeeldingen | `.jpg`, `.jpeg`, `.png`, `.webp`, `.gif` | Visueel analyseren |
| PDF | `.pdf` | Inhoud lezen |
| Tekst | `.txt`, `.md`, `.csv` | Inhoud lezen |
| Word | `.docx` | Tekst uitlezen en lezen |
| Excel | `.xlsx` | Cellen uitlezen en lezen |
| Audio en video | `.mp3`, `.mp4`, `.webm`, `.wav`, `.m4a` | Transcriberen en lezen |

**Audio en video** worden automatisch getranscribeerd. Dat kost **12 credits per
minuut**; een kort fragment kost navenant minder. Documenten en afbeeldingen
kosten niets extra, alleen het gewone berichtverbruik.

## Wat je ziet

Je stuurt een foto van een factuur mee en vraagt wat het totaalbedrag is:

> Op deze factuur staat een totaalbedrag van **€ 1.247,50** inclusief btw.
>
> - Subtotaal: € 1.030,99
> - Btw 21%: € 216,51
> - Vervaldatum: 14 augustus 2026
>
> Zal ik hem in je Werkruimte zetten als taak "betalen vóór 14 augustus"?

Zo werkt het bij elk type: je krijgt geen ruwe tekstdump maar een antwoord op de
vraag die je stelde.

## Het tabblad Afbeeldingen

Beelden die GENI genereert komen hier terecht, met per afbeelding de gebruikte
prompt, het model, de verbruikte credits en de datum. Downloaden doe je met de
downloadknop, verwijderen met het prullenbakicoon.

Zie [AI Beeldgeneratie](../skills/ai-beeldgeneratie.md).

## Veiligheid

Elk meegestuurd bestand wordt server-side gecontroleerd, op type én op inhoud,
zodat een bestand niet iets anders kan zijn dan zijn extensie belooft.
`.json`-bestanden worden geweigerd.

## Grenzen

- **Een bijlage geldt voor dat ene gesprek.** Wil je een document blijvend beschikbaar maken, gebruik dan de [Kennisbank](kennisbank.md).
- **Maximaal drie bestanden per bericht.**
- **Er geldt een maximale bestandsgrootte.** Voor grotere documenten of langere audio gebruik je de Kennisbank of de [Audio Transcriptie](../skills/transcriptie.md)-skill, die tot 200 MB aankan via een URL.
- **`.json` wordt niet geaccepteerd.**
- **Een gescande PDF zonder tekstlaag levert niets op**; er valt geen tekst uit te halen.
- **GENI bewerkt je bestand niet.** Hij leest het en antwoordt; het origineel blijft ongewijzigd.

## Problemen oplossen

**Het bestand wordt geweigerd.** Controleer de extensie tegen de tabel hierboven. `.json` wordt bewust niet geaccepteerd, en een bestand waarvan de inhoud niet bij de extensie past ook niet.

**GENI zegt dat hij de PDF niet kan lezen.** Waarschijnlijk een scan zonder tekstlaag. Haal hem door een OCR-tool.

**De transcriptie kost meer credits dan verwacht.** De prijs loopt per minuut audio, dus een lange opname telt op. Kijk vooraf naar de lengte.

**Een afbeelding staat niet in het overzicht.** Het tabblad Afbeeldingen toont alleen wat GENI zelf genereerde, niet wat jij meestuurde.

**Het bestand is te groot.** Gebruik de Kennisbank voor documenten of de transcriptie-skill voor lange audio.

## Opslag

Bestanden blijven bewaard zolang je account actief is. Verwijder je je account
via **Instellingen → Privacy en export**, dan worden alle bestanden definitief
verwijderd.

## Veelgestelde vragen

**Kan GENI een bestand voor me maken?**
Ja, zoals PDF-rapporten uit de engines en CSV-exports. Die komen onder het
tabblad Bestanden terecht.

**Blijft een meegestuurd bestand bewaard?**
Het hoort bij dat gesprek. Wil je het blijvend als kennis gebruiken, upload het
dan naar de kennisbank.

**Kan iemand anders bij mijn bestanden?**
Nee. Bestanden staan op jouw account.

**Wordt de inhoud gebruikt om AI te trainen?**
Nee.

---

→ Verder: [Kennisbank](kennisbank.md) · [AI-assistent](ai-assistent.md) · [Werkruimte](werkruimte.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Bestanden en afbeeldingen, bijgewerkt augustus 2026*
