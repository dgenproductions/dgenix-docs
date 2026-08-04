# Skills uitgelegd

Skills breiden de mogelijkheden van je assistent uit. Standaard kan hij chatten, teksten schrijven en algemene vragen beantwoorden. Met skills voeg je specifieke capabilities toe.

---

## Wat is een skill?

Een skill is een set tools en instructies die je assistent nieuwe acties geeft. Na activatie weet de assistent wat hij met die skill kan doen en wanneer hij hem inzet.

**Voorbeeld zonder skill:**
> "Stuur een mail naar Jan over de vergadering van morgen"
> Assistent: "Ik kan geen e-mails versturen, ik heb geen toegang tot je inbox."

**Voorbeeld met Gmail-skill:**
> "Stuur een mail naar Jan over de vergadering van morgen"
> Assistent zoekt het e-mailadres van Jan op, schrijft een e-mail en stuurt die. Je ontvangt een bevestiging.

---

## Hoe activeer je een skill?

1. Ga naar **Dashboard → Skills**
2. Blader door de Skills Marketplace
3. Klik **"Activeren"** bij de gewenste skill
4. Volg eventuele setup-stappen (koppelen van een dienst, invoeren van een API-key)
5. De skill is direct beschikbaar, je assistent kan hem meteen gebruiken

Sommige skills vereisen een integratie (bijv. Gmail koppelen). Een tutorial verschijnt direct na activatie.

---

## Hoe weet de assistent wanneer hij een skill gebruikt?

De assistent gebruikt skills automatisch op basis van de context van je vraag. Jij hoeft niet te zeggen "gebruik de Gmail-skill", hij herkent wanneer hij ergens toegang voor nodig heeft.

**Jij vraagt:** "Stuur de offerte als bijlage naar klant@voorbeeld.nl"
**Assistent herkent:** dit is een e-mail met bijlage → gebruikt Gmail-skill + Drive-skill

Je kunt ook expliciet een skill aanroepen als je wil:
> "Gebruik Social Media Manager om een LinkedIn post te schrijven over..."
> "Genereer een afbeelding met FLUX van..."

---

## Skillcategorieën

### Persoonlijk, inbegrepen (Starter+)

Skills voor dagelijkse productiviteit. Gratis te activeren.

| Skill | Wat het doet |
|---|---|
| **Gmail** | E-mails lezen, schrijven en versturen |
| **Google Calendar** | Agenda beheren, afspraken bekijken, aanmaken en verwijderen |
| **Google Drive** | Bestanden zoeken, lezen en aanmaken |
| **Google Sheets** | Spreadsheets lezen en bijwerken |
| **Dagplanner & Life Assistant** | Dagplanning opstellen, prioriteiten rangschikken |
| **Document Lezer** | PDF's en Word-documenten lezen en samenvatten |
| **Short Generator** | Korte clips uit een video-URL (basis) |
| **Telegram Add-on** | Assistent ook via Telegram gebruiken |

### Zakelijk, Growth+

Skills voor zakelijke taken. Beschikbaar vanaf het Growth-plan.

| Skill | Wat het doet |
|---|---|
| **AI Beeldgeneratie** | Afbeeldingen genereren met Google Nano Banana (+ Pro) |
| **FLUX Beeldgeneratie** | Afbeeldingen genereren met het FLUX-1 model |
| **Social Media Manager** | Posts schrijven voor LinkedIn, Instagram, X en Facebook |
| **Voorstel Generator** | Professionele offertes en voorstellen opstellen |
| **Content Repurposing** | Content hergebruiken en omzetten naar andere formats |
| **Weekrapport Generator** | Automatisch wekelijkse rapporten samenstellen |
| **Lead Research & Outreach** | Leads onderzoeken en persoonlijke outreach schrijven |
| **Client Onboarding** | Onboardingdocumenten en welkomstmails opstellen |
| **Audio Transcriptie** | Audio-opnames omzetten naar tekst |
| **Travel Planner** | Reisplanningen en route-overzichten maken |
| **Smart Shopping** | Producten vergelijken en aankoopadvies geven |
| **Meal Planner** | Maaltijdplanningen en boodschappenlijsten opstellen |
| **Persoonlijke Financiën** | Inkomsten en uitgaven analyseren |
| **YouTube Manager** | YouTube-kanaal beheren, titels en beschrijvingen schrijven |
| **SEO Blog Schrijver** | SEO-geoptimaliseerde blogartikelen schrijven |
| **AI Beeldbewerking** | Bestaande afbeeldingen bewerken met AI |

### Zakelijk, Pro+

Skills voor geavanceerde toepassingen. Inbegrepen vanaf het Pro-plan.

| Skill | Wat het doet |
|---|---|
| **GEO Engine** | AI-zichtbaarheid meten (Share-of-Voice in ChatGPT/Perplexity/Gemini/Claude) |
| **Authority Engine** | Content schrijven en draft-first publiceren naar je CMS |
| **Reputation Engine** | Review-campagnes via branded e-mail met Google review-link |
| **Workflow Builder** | n8n-workflows importeren en uitvoeren als AI-tool |
| **Support Kennisbank** | Kennisbank opbouwen voor geautomatiseerde supportantwoorden |
| **Vergadering Assistent** | Notulen en actiepunten uit een gesprek of opname |
| **CRM Sync** | CRM-data lezen en bijwerken |
| **Factuur Generator** | Facturen aanmaken en versturen |
| **Renewal & Upsell Intelligence** | Klantdata analyseren voor hernieuwings- en upsell-kansen |
| **Eigen Telegram Bot** | GENI onder je eigen botnaam en handle |

> Geen losse add-on-prijzen meer: alle zakelijke skills zijn **inbegrepen vanaf Growth+ of Pro+** (afhankelijk van de skill). Je betaalt per uitgevoerde actie in credits, niet per maand per skill. Zie [Plannen & Prijzen](../plannen-en-prijzen/README.md).

---

## Skills en integraties

De meeste skills hebben een koppeling nodig om te werken. Na activatie verschijnt een tutorial die je stap voor stap door de setup leidt.

**OAuth-integraties** (eenmalig inloggen):
- Gmail, Google Calendar, Drive, Sheets → Google-account koppelen
- Notion → Notion-account koppelen
- Slack → Slack-workspace koppelen
- LinkedIn → LinkedIn-account koppelen

**API-key integraties** (credential invoeren in Instellingen):
- WhatsApp Business → Meta Business API-key
- Instagram DM → Meta Business API-key
- Stripe → Stripe API-key
- HubSpot → HubSpot API-key

Integraties beheer je via **Connectors**.

---

## Skills deactiveren

Ga naar **Dashboard → Skills** of **Billing** en klik "Deactiveren" bij de skill.

- **Gratis skills** worden direct gedeactiveerd
- **Add-on skills** (Stripe) worden gedeactiveerd aan het einde van de betaalperiode

Verbruikte credits worden niet teruggestort.

---

## Skill-credits, wat kost een skill?

Elke skill-actie verbruikt credits. Een richtlijn:

De richtprijzen per taaktype staan op één plek: **[Het creditsysteem](../hoe-het-werkt/credits.md)**.
Daar zie je wat een chatvraag, een e-mailactie of een engine-audit ongeveer kost.

Twee dingen bepalen de prijs van een skill-actie. Er is een vaste opslag per
skill, en daarbovenop reken je het taalmodel af naar gebruik. Een korte vraag
over drie mails kost dus minder dan een samenvatting van een volle inbox, ook al
is het dezelfde skill.

Acties met een vaste prijs, zoals een audit of een beeldgeneratie, zijn wél
exact. Die staan als bedrag op de knop voordat je ze start.

Exacte kosten staan verder per skill in de marketplace-kaart en in de
bijbehorende skill-documentatie.

---

## Veelgestelde vragen

**Kan ik zelf kiezen welke skill de assistent gebruikt?**
De assistent kiest automatisch op basis van context. Je kunt ook expliciet een skill aanroepen: "gebruik de Social Media Manager om..."

**Werkt een skill via zowel het dashboard als Telegram?**
Ja, alle geactiveerde skills werken via beide interfaces.

**Wat als een skill faalt?**
De assistent meldt de fout in de chat. Controleer of je integratie nog actief is (Connectors). Als het probleem aanhoudt, neem contact op via Support.

**Kan ik een skill testen voor ik activeer?**
Nee, je moet hem activeren. Gratis skills zijn direct te deactiveren. Add-ons lopen via Stripe, zorg dat je de beschrijving goed leest voor activatie.
