# dGENIX Docs — CLAUDE.md

> Documentatie subproject voor dGENIX. Publiek beschikbaar via GitBook.
> **Isolatieregel:** dit project raakt NOOIT app/, agent/ of site/ — aparte repo en deployment.

---

## Wat is dit

Publieke gebruikersdocumentatie voor dGENIX, gepubliceerd via GitBook. Bevat geen interne architectuurbeschrijvingen, business logic of credentials — alleen wat eindgebruikers nodig hebben.

| Veld | Waarde |
|---|---|
| **Platform** | GitBook (automatische sync via GitHub) |
| **Repo** | github.com/dgenproductions/dgenix-docs (privé) |
| **Publieke URL** | docs.dgenix.com (of via GitBook subdomain) |
| **Taal** | Nederlands (primair) |
| **Datum** | 15 april 2026 |

---

## Mappenstructuur

```
docs/
├── README.md                        ← Welkomstpagina (root van GitBook)
├── SUMMARY.md                       ← Inhoudsopgave — GitBook navigatie
├── .gitbook.yaml                    ← GitBook config (root + summary vergrendeld)
├── aan-de-slag/
│   ├── README.md                    ← Overzicht sectie
│   ├── toegangscode.md              ← Invite code aanvragen
│   ├── account-aanmaken.md          ← Registratie
│   └── telegram-koppelen.md         ← Telegram + assistent activeren
├── hoe-het-werkt/
│   ├── README.md                    ← Wat doet je assistent?
│   └── credits.md                   ← Creditsysteem uitleg
├── functies/
│   ├── dashboard.md
│   ├── ai-assistent.md
│   ├── workflow-automations.md
│   ├── bestanden.md
│   ├── projecten.md
│   ├── kennisbank.md
│   ├── geheugen.md
│   └── instellingen.md
├── skills/
│   ├── README.md                    ← Skills marketplace overzicht
│   ├── ai-beeldgeneratie.md
│   ├── short-generator.md
│   ├── social-media.md
│   ├── dagplanner.md
│   ├── transcriptie.md              ← Fireworks Whisper v3
│   ├── flux-image.md                ← Fireworks FLUX-1
│   ├── whatsapp-business.md         ← Batch 3
│   ├── instagram-dm.md
│   ├── stripe-insights.md
│   ├── notion.md
│   ├── slack.md
│   ├── cms-publisher.md
│   ├── hubspot.md
│   ├── linkedin.md
│   └── meeting-assistant.md
├── plannen-en-prijzen/
│   ├── README.md                    ← Planvergelijking
│   └── credits-bijkopen.md
├── integraties/
│   ├── telegram.md
│   ├── gmail.md
│   ├── google-calendar.md
│   ├── google-drive.md
│   └── google-sheets.md
└── faq.md
```

---

## Hoe changes publishen

GitBook synct automatisch bij elke push naar de `master` branch van de docs-repo.

```bash
# Altijd instellen in deze repo:
git config user.email "dgendreams@gmail.com"
git config user.name "dGEN Productions"

# Wijziging publiceren:
git add .
git commit -m "Docs: [beschrijving wijziging]"
git push
```

GitBook pikt de wijziging automatisch op. Geen handmatige sync nodig.

---

## Werkregels

### Wat WEL in publieke docs hoort
- Gebruikerstutorials (hoe activeer ik X)
- Feature beschrijvingen (wat kan X)
- Prijzen en planoverzicht (kopieer uit site/pricing)
- Integratie stap-voor-stap handleidingen
- FAQ antwoorden

### Wat NIET in publieke docs hoort
- Architectuurbeschrijvingen (router, credit economy, skill registry)
- Business logic (markup percentages, cost per model)
- Interne tools (admin panel, provisioning)
- Credentials of API-keys
- Interne roadmap of features in ontwikkeling

Interne documentatie hoort in `projects/dgenix/intern/` (niet in deze repo).

### SUMMARY.md is leidend
GitBook navigatie wordt volledig bepaald door `SUMMARY.md`. Elk nieuw `.md` bestand dat niet in `SUMMARY.md` staat is niet bereikbaar via GitBook (beveiligd via `.gitbook.yaml`).

**Bij nieuw bestand:** altijd ook een entry toevoegen in `SUMMARY.md`.

---

## Nieuwe skill documenteren

Bij elke nieuwe skill die live gaat in de agent (FASE 2 van het uitvoerplan):

1. Maak `skills/[slug].md` aan — structuur:
   ```markdown
   # [Skill Naam]
   
   ## Wat doet deze skill?
   [1 alinea omschrijving]
   
   ## Vereisten
   - Plan: [Starter / Growth / Pro]
   - Integraties: [indien van toepassing]
   
   ## Hoe activeer je de skill?
   [stappen]
   
   ## Wat kun je ermee?
   [voorbeelden / use cases]
   
   ## Creditkosten
   [tabel of omschrijving]
   ```
2. Voeg entry toe aan `SUMMARY.md` onder `## Skills`
3. Vermeld skill in `skills/README.md` (marketplace overzicht)

---

## Status pagina's

| Pagina | Status |
|---|---|
| README.md | ✅ Live |
| aan-de-slag/ (4 pagina's) | ✅ Live |
| hoe-het-werkt/ (2 pagina's) | ✅ Live |
| functies/ (8 pagina's) | ✅ Live |
| skills/ (24 skills) | ✅ Live — ai-beeldgeneratie, short-generator, social-media, dagplanner + transcriptie, flux-image + 9 Batch 3 skills (whatsapp-business t/m meeting-assistant) + 7 nieuw (gmail, google-calendar, google-drive, google-sheets, document-reader, travel, shopping) + workflow-import |
| plannen-en-prijzen/ (2 pagina's) | ✅ Live |
| integraties/ (5 pagina's) | ✅ Live |
| faq.md | ✅ Live |
| skills/youtube.md | 🔜 Bouwen zodra YouTube skill live is |
| skills/seo-blog.md | 🔜 Bouwen zodra SEO Blog skill live is |
| skills/dagplanner.md | ✅ Live |
| skills/news.md | 🔜 Bouwen zodra Daily News skill live is |
