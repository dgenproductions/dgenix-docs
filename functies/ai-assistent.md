# AI Assistent

De AI Assistent pagina is de web-interface van jouw persoonlijke assistent. Naast Telegram kun je hier rechtstreeks vanuit de browser berichten sturen en ontvangen.

---

## Webchat

Stuur opdrachten en vragen via het invoerveld onderaan de pagina. Als je de Telegram add-on hebt actief, worden berichten gesynchroniseerd — je ziet gesprekken via beide kanalen terug.

**Nieuwe sessie starten:** klik "Nieuwe gesprek starten" om een nieuw gesprek te beginnen. Eerdere gesprekken blijven bewaard in de geschiedenis.

---

## Model kiezen (Growth & Pro)

Boven het invoerveld staan modelknoppen. Kies het model dat past bij je taak:

| Model | Snelheid | Credits | Geschikt voor |
|-------|----------|---------|---------------|
| **Auto** | — | Variabel | Standaard — dGENIX kiest per taak |
| **Haiku** | Snel | ~36/bericht | Eenvoudige vragen, korte taken |
| **Sonnet** | Krachtig | ~135/bericht | Schrijven, analyse, complexe taken |
| **Opus** | Meest intelligent | ~300+/bericht | Diepgaande redenering, grote projecten |

Auto is beschikbaar voor alle plannen. Handmatige modelselectie vereist Growth of Pro.

---

## Zijpaneel — Gesprekken & Kennisbank

Het zijpaneel heeft twee tabbladen:

### Gesprekken
- Recente sessies weergegeven per datum
- Klik op een sessie om de geschiedenis te laden
- Verwijder sessies via het prullenbakicoon

### Kennisbank
- Upload bestanden die de assistent als context gebruikt
- Ondersteunde formaten: **PDF, Word (.docx), afbeeldingen (JPG, PNG, WebP)**
- De assistent leest de inhoud en gebruikt het bij zijn antwoord

---

## Kennisdocument

Je persoonlijke kennisdocument (aangemaakt tijdens de intake) is zichtbaar als ingeklapt accordeon. Klik op de header om het uit te klappen en te lezen.

- **Bewerken:** pas het document aan via de "Bewerken" knop in de accordeon-header
- **Downloaden:** sla het op als tekstbestand via de "Download" knop in de accordeon-header

Het kennisdocument wordt altijd automatisch meegeladen als context door de assistent.

---

## Context per project

Als je een gesprek voert binnen een **projectmap**, combineert de assistent twee bronnen:

1. **Globaal kennisdocument** — je persoonlijke info, werkwijze en voorkeuren (altijd aanwezig)
2. **Projectinstructies** — de specifieke context van dat project (klant, toon, regels)

Stel projectinstructies in via het ⚙️ tandwieltje-icoon op een projectmap in de zijbalk. Gesprekken buiten een project gebruiken alleen het globale kennisdocument.

**Resultaat:** een gesprek in project "Bakkerij De Krent" gebruikt automatisch formele toon en merkrichtlijnen — zonder dat je dat elke keer herhaalt.

---

## Voice Chat — inspreken & terugluisteren

Klik op het **microfoon-icoon** rechts van het invoerveld. Je assistent luistert, transcribeert je vraag automatisch en geeft niet alleen een tekstantwoord — hij leest het ook hardop voor in de stem die jij hebt ingesteld.

**Hoe het werkt:**

1. Klik op 🎤 in het chatvenster — opname start direct
2. Stel je vraag of geef een opdracht in
3. Klik nogmaals om te stoppen
4. Je assistent transcribeert → verwerkt → streamt tekstantwoord → speelt het als spraak af

**Stemkeuze instellen:**
Ga naar **Instellingen → Mijn Assistent → Stem voor spraakantwoord**. Kies uit 6 stemmen:

| Stem | Karakter |
| --- | --- |
| Onyx | Diep & gezaghebbend *(standaard)* |
| Alloy | Neutraal & vriendelijk |
| Echo | Mannelijk, helder |
| Fable | Warm, verhalend |
| Nova | Vrouwelijk, levendig |
| Shimmer | Zacht & vriendelijk |

**Creditkosten Voice Chat:**

| Actie | Credits |
| --- | --- |
| Vraag stellen via microfoon (AI-antwoord) | ~20–36 cr |
| Spraakantwoord ~500 tekens | ~94 cr |
| Spraakantwoord ~1.000 tekens | ~188 cr |

Spraakberichten via Telegram worden ook verwerkt — de assistent transcribeert ze automatisch en reageert als tekst.

---

## Bestanden uploaden voor de assistent

Via het paperclip-icoon in het invoerveld kun je bestanden meesturen met je bericht:
- Afbeeldingen → de assistent bekijkt en beschrijft ze
- PDF/Word → de assistent leest de inhoud

## Camera in de chat

Klik op de **+** knop links van het invoerveld en kies **Camera / Selfie** om een foto te maken zonder de chat te verlaten.

Hoe het werkt:
- Live camera-preview opent in een venster
- Knop in het midden = foto maken
- Knop met pijl = wisselen tussen voor- en achtercamera (op apparaten met meerdere camera's)
- Na het maken kun je de foto opnieuw maken of bevestigen
- Bevestigde foto wordt direct als bijlage toegevoegd aan je volgende bericht

Werkt op desktop (webcam) en mobiel (selfie + achtercamera). Bij eerste gebruik vraagt je browser om toestemming voor de camera.

## Persoonlijke suggesties op het lege chatscherm

Als je een nieuw gesprek opent zie je 6 suggestiekaarten. Klik er één om de tekst direct in je invoerveld te zetten , je kunt nog aanpassen voor je verstuurt.

Hoe ze gekozen worden:
- Op basis van je plan (Free/Starter/Growth/Pro)
- Suggesties voor skills die jij actief hebt komen vaker bovenaan
- Suggesties voor skills die op je plan beschikbaar zijn maar nog niet actief, worden ook getoond , handig om te ontdekken wat dGENIX nog meer kan

Klik op de **Vernieuwen / Shuffle** knop rechtsboven de cards voor een nieuwe set.

## Tools-knop , modes voor diepere antwoorden

Naast de **+** knop staat een **gereedschaps-icoon (Tools)**. Klik om uit 5 modes te kiezen die je antwoord op een andere manier laten genereren:

| Mode | Plan | Wat het doet |
|---|---|---|
| **Deep Research** | Growth+ | Multi-iteratie web search met genummerde bronnenlijst , ideaal voor markt- en concurrentie-analyses |
| **SEO Optimizer** | Growth+ | Audit van een URL met top 5 verbeterpunten |
| **GEO Optimizer** | Pro+ | Audit voor AI-zoekmachines (ChatGPT, Claude, Perplexity) |
| **Stap-voor-stap** | Alle plannen | Antwoord in genummerde stappen, ideaal voor handleidingen |
| **Web zoeken aan** | Alle plannen | Forceer web search bij dit bericht voor actuele info met bronvermelding |

Een actieve mode toont een indigo chip boven het invoerveld met een kruisje om hem uit te schakelen. Bij modes die een specifieke skill nodig hebben (Deep Research, SEO/GEO) krijg je een upgrade- of activeer-melding als je die nog niet hebt.

Bronnen die de assistent gebruikt verschijnen automatisch als klikbare links onderaan zijn antwoord.
