# Platform Manual — dGENIX

Welkom bij de volledige gebruikershandleiding van dGENIX. Dit document legt het platform van A tot Z uit: hoe je assistent werkt, hoe hij context opbouwt, welke functies beschikbaar zijn en hoe je alles optimaal benut.

---

## Wat is dGENIX?

dGENIX is een persoonlijk AI-platform. Geen chatbot die je elk gesprek vergeet — een assistent die jou leert kennen, taken uitvoert en uitbreidbaar is via skills.

**Twee interfaces:**

- **Web Dashboard** (`app.dgenix.com`) — de primaire interface. Hier chat je, stel je in, activeer je skills en bekijk je alles.
- **Telegram** (optionele add-on) — activeer de Telegram-koppeling als je ook onderweg via je telefoon met je assistent wil werken.

---

## Hoe werkt je assistent?

Je assistent is een Claude AI-model (van Anthropic) dat vóór elk gesprek context laadt. Die context bestaat uit meerdere lagen die samen bepalen hoe je assistent antwoordt:

| Laag | Wat het is | Beheer |
|---|---|---|
| **Platformkennis** | Wat dGENIX is, welke skills beschikbaar zijn, algemene gedragsregels | Automatisch (door dGENIX) |
| **Kennisdocument** | Jouw persoonlijk profieldocument — wie ben je, hoe werk je, wat wil je | Instellingen → AI Assistent |
| **Persoonlijke instructies** | Vaste regels die je assistent altijd volgt | Instellingen → AI Assistent |
| **Kennisbank** | Documenten die je uploadt als achtergrondkennis (.md, .pdf, .docx, .txt) | Dashboard → Assistent → Kennisbank |
| **Geheugen** | Feiten, voorkeuren en patronen die de assistent automatisch onthoudt | Instellingen → Geheugen |
| **Projectinstructies** | Specifieke context per projectmap (klant, toon, regels) | Per projectmap — tandwieltje-icoon |

Al deze lagen worden gecombineerd bij elk gesprek. Zo weet je assistent wie je bent, hoe hij moet reageren en wat de context van het gesprek is — zonder dat jij het elke keer opnieuw hoeft uit te leggen.

Meer over deze systemen: [Context en geheugen uitgelegd](context-en-geheugen.md)

---

## Dashboard — de functies

### AI Assistent (chat)

De chatinterface is je hoofdkanaal. Stuur opdrachten als tekst, via microfoon (spraak-naar-tekst) of als Voice Call (volledig gesproken gesprek). De assistent voert taken uit, geeft antwoorden en slaat resultaten op.

→ [AI Assistent](../functies/ai-assistent.md)

### Projecten

Maak projectmappen aan voor klanten, projecten of thema's. Elk project heeft eigen gesprekken en optioneel eigen instructies. Zo houdt je assistent de context per klant of project gescheiden.

**Voorbeeld:** project "Bakkerij De Krent" heeft instructies over de tone-of-voice en het assortiment. Gesprekken in dat project gebruiken automatisch die context.

→ [Projecten](../functies/projecten.md)

### Taken & Automatisering

Stel terugkerende opdrachten in die je assistent automatisch uitvoert — dagelijks, wekelijks of op een vast moment. Denk aan een dagelijks rapport, een wekelijkse nieuwsbrief of een maandelijkse samenvatting.

→ [Taken en reminders](geplande-taken.md)

### Bestanden & Assets

Alles wat je assistent genereert (documenten, afbeeldingen, audio-transcripties) staat in het Bestanden-overzicht. Je kunt ze downloaden, delen of opnieuw gebruiken.

→ [Bestanden & Afbeeldingen](../functies/bestanden.md)

### Kennisbank

Upload documenten die je assistent als achtergrondkennis gebruikt. Ondersteunde formaten: PDF, Word (.docx), tekstbestanden (.txt) en Markdown (.md). De assistent leest deze documenten en gebruikt ze bij relevante vragen en taken.

→ [Kennisbank](../functies/kennisbank.md)

### Voice Chat

**Voice Memo:** klik op het microfoon-icoon in de chat en spreek in. Je vraag wordt automatisch omgezet naar tekst en verwerkt. Het antwoord verschijnt als tekst in de chat.

**Voice Call:** klik op het geluidsgolven-icoon voor een volledig gesproken gesprek. Een animerend orb-scherm opent — jij spreekt, de assistent luistert, verwerkt en spreekt het antwoord terug in een stem naar keuze.

→ [Voice Chat gebruiken](voice-chat.md)

### Workflow Builder (Pro)

Importeer n8n-workflows en laat je assistent ze uitvoeren als tool. Beschikbaar via de Workflow Builder skill (Pro plan).

---

## Skills — de uitbreidingen

Skills voegen specifieke capabilities toe aan je assistent. Standaard kan hij chatten, plannen en teksten schrijven. Met skills kan hij ook:

- E-mails versturen via Gmail
- Afspraken inplannen in Google Calendar
- Social media posts aanmaken
- AI-afbeeldingen genereren
- Spreadsheets bijwerken
- Facturen aanmaken
- En nog tientallen andere taken

Skills zijn verdeeld over twee categorieën: **Persoonlijk** (productiviteit, leven) en **Zakelijk** (werk, klanten, marketing). Sommige skills zijn inbegrepen bij je plan, andere zijn beschikbaar als add-on via Stripe.

→ [Skills uitgelegd](skills-uitgelegd.md)
→ [Skills marketplace overzicht](../skills/README.md)

---

## Integraties — externe diensten koppelen

Verbind je assistent met externe diensten via OAuth of API-key. Gekoppelde diensten zijn beschikbaar als tools voor je assistent.

**OAuth-integraties** (inloggen via consent screen):
- Google (Gmail, Calendar, Drive, Sheets)
- Notion, Slack, LinkedIn, Microsoft 365 _(binnenkort)_

**API-key integraties** (credentials invoeren in Settings):
- WhatsApp Business, Instagram DM, Stripe, HubSpot

**Telegram** is een aparte add-on — zie [Telegram add-on](../integraties/telegram.md).

Integraties beheer je via **Instellingen → Integraties**.

---

## Credits — hoe werkt het systeem?

Elke interactie met je assistent verbruikt credits. Credits worden maandelijks bijgecrediteerd op basis van je plan. Je kunt ze ook losse bij bijkopen.

| Plan | Credits/mnd | ~Taken/mnd |
|---|---|---|
| Starter | 88.000 | ~900 |
| Growth | 212.000 | ~2.150 |
| Pro | 495.000 | ~5.050 |

**Wat kost wat?**

| Actie | ~Credits |
|---|---|
| Simpel chatbericht (Haiku) | 25–50 cr |
| Uitgebreid bericht of analyse (Sonnet) | 100–200 cr |
| AI-afbeelding genereren | 250–1.500 cr |
| E-mail lezen en beantwoorden | 50–150 cr |
| Voice Call-antwoord (~500 tekens) | ~1.375 cr |
| Audio transcriberen (per minuut) | 12–20 cr |

Credits verlopen niet. Je saldo rolt over naar volgende maand.

→ [Credits bijkopen](../plannen-en-prijzen/credits-bijkopen.md)
→ [Creditsysteem](../hoe-het-werkt/credits.md)

---

## Assistent personaliseren

Je assistent is standaard neutraal ingesteld. Via Instellingen pas je hem volledig aan:

- **Naam:** geef hem een eigen naam
- **Communicatiestijl:** casual, formeel, direct of gedetailleerd
- **Focusgebieden:** vink aan wat voor jou relevant is (productiviteit, marketing, sales, etc.)
- **Persoonlijke instructies:** vaste regels die altijd gelden — "antwoord altijd in stikpunten", "gebruik formele toon bij e-mails"
- **Kennisdocument:** je persoonlijk profieldocument — wie je bent, je bedrijf, hoe je werkt
- **Stem:** kies een stem voor Voice Chat (Nederlandse of Engelse stemmen beschikbaar)

→ [Meer over context en geheugen](context-en-geheugen.md)
→ [Instellingen](../functies/instellingen.md)

---

## Telegram add-on

Telegram is geen verplicht onderdeel van dGENIX — het is een optionele add-on. Als je het activeert, werkt je assistent ook via de Telegram-app op je telefoon.

**Wat je kunt doen via Telegram:**
- Tekstvragen stellen en opdrachten geven
- Spraakberichten insturen (worden automatisch getranscribeerd)
- Foto's meesturen (de assistent analyseert ze)
- Dezelfde skills gebruiken als via het dashboard

Gesprekken worden gesynchroniseerd: wat je in Telegram stuurt, is ook zichtbaar in het dashboard.

→ [Telegram add-on activeren](../integraties/telegram.md)

---

## Veel gebruikte opdrachten

**Productiviteit:**
> "Wat staat er morgen op mijn agenda?"
> "Plan een meeting met Jan op donderdag om 14:00"
> "Geef me een overzicht van mijn ongelezen e-mails"

**Content & communicatie:**
> "Schrijf een LinkedIn post over onze nieuwe dienst"
> "Maak een conceptantwoord voor de laatste mail van klant X"
> "Genereer een AI-afbeelding van een moderne kantooromgeving"

**Zakelijk:**
> "Analyseer de omzet in mijn Google Sheets van afgelopen kwartaal"
> "Maak een offerte voor een website-project van €2.500"
> "Stuur een samenvatting van het project naar het Slack-kanaal #team"

**Automatisering:**
> "Maak een geplande taak: elke maandag een weekrapport van mijn agenda"
> "Elke dag om 09:00: drie prioriteiten voor vandaag"

---

## Veelgestelde vragen

**Mijn assistent vergeet wat ik vorige week heb gezegd — waarom?**
Per gesprekssessie laadt de assistent de context (kennisdocument, instructies, geheugen). Korte feiten of afspraken die je noemt in een gesprek worden bewaard als herinneringen — maar niet elk detail van elk gesprek. Voeg belangrijke informatie toe aan je kennisdocument of persoonlijke instructies voor permanente context.

**Wat is het verschil tussen het kennisdocument en het geheugen?**
Het kennisdocument schrijf je zelf: wie je bent, hoe je werkt, wat je assistent moet weten. Het geheugen bouwt de assistent automatisch op uit gesprekken — feiten, voorkeuren en patronen die hij zelf onthoudt. Beide worden altijd meegeladen.

**Kan ik meerdere assistenten hebben?**
Nee, je hebt per account één assistent. Wel kun je per projectmap eigen instructies en context instellen, waardoor de assistent zich anders gedraagt afhankelijk van het project.

**Worden mijn gegevens gebruikt voor AI-training?**
Nee. Gesprekken en data worden niet gebruikt voor het trainen van AI-modellen.

**Hoe stop ik een skill?**
Ga naar **Instellingen → Integraties** of **Billing** en deactiveer de skill of add-on. Credits die al verbruikt zijn worden niet teruggestort.

---

_Platform Manual v1.0 — dGENIX | April 2026_
