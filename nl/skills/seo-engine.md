# SEO Engine

## Wat doet deze skill?

De [SEO Engine](https://dgenix.nl/engines/seo) analyseert je webpagina's op alle technische SEO-factoren: on-page elementen, content kwaliteit, technische gezondheid en sitestructuur. Je krijgt een totaalscore, deelscores per categorie, een lijst met gevonden problemen en prioritaire acties om hoger te scoren in Google.

## Vereisten

- **Plan:** Growth+
- **Integraties:** Geen, de audit analyseert je publieke webpagina rechtstreeks

## Hoe activeer je de skill?

1. Ga naar **Dashboard -> Skills** en activeer de **SEO Engine**
2. Ga via het zijmenu naar **Groei Tools -> SEO Engine**
3. Voer je pagina-URL in en klik op de **+**-knop
4. Kies een audit-diepte en start

## Wat kun je ermee?

### Website audit

Voer een audit uit op elke pagina die je wilt verbeteren. Kies uit vier dieptes:

| Type | Inhoud | Credits |
|---|---|---|
| Quick Check | Basisscores, on-page elementen | 1.500 cr |
| Standaard Audit | Volledige analyse, 4 categorieën, 5 pagina's | 4.000 cr |
| Deep Audit | Tot 10 subpagina's analyseren | 10.000 cr |
| **Max Audit** | Deep + JS-rendering + echte Core Web Vitals + keyword-posities & zoekvolume | 22.000 cr |

### Wat wordt gemeten?

**SEO Score**, gewogen totaalscore van de vier categorieën (0–100).

**On-Page**, title tag, meta description, H1–H3 koppen, alt-teksten, interne links.

**Content**, leesbaarheid, keyword density (indien opgegeven), tekstlengte, unieke content signalen.

**Technisch**, HTTPS, canonical tag, viewport meta, **echte Core Web Vitals** (LCP/INP/CLS via Google PageSpeed, instelbaar mobiel/desktop), Open Graph, alt-teksten. Plus de **fundamenten**: robots.txt-validatie, XML-sitemap-check, **gebroken links** (4xx/5xx), **redirect-ketens** (inclusief HTTP→HTTPS), **mixed-content**, **hreflang** en verouderd **beeldformaat** (WebP/AVIF-advies).

**Structuur**, URL-diepte, breadcrumb aanwezigheid, interne linkstructuur, sitemap verwijzingen.

### Max Audit, de diepste analyse

De **Max Audit** voegt drie dingen toe bovenop een Deep Audit:

- **JavaScript-rendering**, de pagina wordt eerst volledig geladen (zoals in een echte browser), zodat content die via JavaScript binnenkomt (Wix, Shopify, React) ook wordt geanalyseerd.
- **Echte Core Web Vitals**, LCP, INP en CLS uit Google PageSpeed Insights in plaats van een schatting.
- **Keyword-posities & zoekvolume**, voor welke zoekwoorden je site rankt, op welke positie, met het maandelijkse zoekvolume (via DataForSEO). Instelbaar **per land en taal**, zodat de data klopt voor jouw markt (NL, BE, DE, UK, US en meer).

### Doelzoekwoord opgeven

Je kunt optioneel een doelzoekwoord meegeven bij elke audit. De SEO Engine analyseert dan ook de keyword density, plaatsing in title/H1 en content relevantie voor dat zoekwoord.

### Issues en aanbevelingen

Per audit krijg je:

- **Issues** gesorteerd op ernst (Kritiek / Hoog / Medium / Laag) met type en beschrijving
- **Aanbevelingen** gesorteerd op prioriteit (High / Medium) met concrete actiestappen en verwacht resultaat

### Exporteren & vergelijken

Exporteer elk rapport als **PDF** (client-ready) of **CSV** (scores, issues, keywords en concurrenten, handig voor bureaus). Bij een tweede audit toont het dashboard automatisch de **verandering t.o.v. de vorige audit** (score, deelscores en aantal problemen) plus je **vooruitgang over tijd**.

## Website-crawl, echte multi-page crawl

Naast de snelle audit heeft de SEO Engine een **Website-crawl**: een echte crawl van je hele site (geen losse pagina). Je krijgt een getabd paneel met **Overzicht**, **Issues** (met "hoe op te lossen" per type), **Crawled pages** en **Statistieken**, plus een **Site Health-meter**.

| Tier | Pagina's | Inhoud | Credits |
|---|---|---|---|
| Light | tot 25 | 100+ checks, duplicate titles/descriptions, gebroken links, redirects | 6.000 cr |
| Standaard | tot 50 | + meer resources en checks | 12.000 cr |
| Pro | tot 100 | + JavaScript-rendering + Lighthouse | 22.000 cr |

De pagina-limiet bepaalt de kosten, je houdt de crawl (en dus de credits) altijd in de hand.

## Keyword Research

Geef een zoekwoord en je krijgt een werkblad met **long-tail-ideeen**: maandelijks **zoekvolume**, **difficulty**, **zoekintentie** (informationeel/commercieel/transactioneel) en een **AI-Overview-kans**-vlag (kandidaten die goed scoren in AI-antwoorden). **500 credits** per zoekopdracht.

## Links & Authority

In de tab **Links** analyseer je je backlink-profiel:

- **Authority Score**, je domein-autoriteit (0–100)
- **Domein-overzicht**, backlinks, verwijzende domeinen, IP's, gebroken links, keywords
- **Nieuwe & verloren** verwijzende domeinen over tijd
- **Toxic / risico-domeinen**, verwijzende domeinen met een hoge spam-score
- **(Pro) Link gap**, domeinen die je concurrent wél linken en jou niet, plus een domein-vs-domein vergelijking

| Tier | Inhoud | Credits |
|---|---|---|
| Links Check | Authority + top verwijzende domeinen | 8.000 cr |
| Links Audit | + new/lost + toxic-links | 15.000 cr |
| Links Audit Pro | + concurrent link-gap + compare | 25.000 cr |

## Creditkosten

| Actie | Credits |
|---|---|
| Quick Check | 1.500 |
| Standaard Audit | 4.000 |
| Deep Audit (tot 10 pagina's) | 10.000 |
| Max Audit (+ render + CWV + keywords) | 22.000 |
| Website-crawl (Light / Standaard / Pro) | 6.000 / 12.000 / 22.000 |
| Keyword Research (per zoekopdracht) | 500 |
| Links & Authority (Check / Audit / Pro) | 8.000 / 15.000 / 25.000 |

## Voorbeeld: wat je krijgt na een audit

Je draait een Standaard Audit op je dienstenpagina. Het resultaat is geen lijst
met technische meldingen maar een geordend oordeel:

> **SEO-score 61 / 100** , was 54 bij je vorige audit *(+7)*
>
> | Categorie | Score |
> |---|---|
> | On-page | 72 |
> | Content | 58 |
> | Technisch | 49 |
> | Structuur | 66 |
>
> **Kritiek (2)**
> - Meta description ontbreekt op deze pagina
> - 3 interne links geven een 404
>
> **Hoog (1)**
> - LCP is 4,1 seconde op mobiel, streef naar onder 2,5
>
> **Aanbevolen actie:** schrijf een meta description van 150-160 tekens rond je
> doelzoekwoord. Verwacht effect: hogere doorklikratio vanuit Google.

De volgorde is de opbrengst: je weet welke drie dingen je maandag doet, in
plaats van dat je zelf uit honderd signalen moet kiezen.

## Grenzen

- **De engine wijzigt niets aan je site.** Hij meet en adviseert; aanpassen doe je zelf of via de [Authority Engine](authority-engine.md).
- **Je pagina moet publiek bereikbaar zijn.** Een staging-omgeving achter een login of wachtwoord kan niet worden geanalyseerd.
- **Een score is geen positiegarantie.** Een hogere score verbetert je fundament, maar posities hangen ook af van concurrentie, autoriteit en zoekintentie.
- **De pagina-limiet per tier is hard.** Een crawl gaat tot 25, 50 of 100 pagina's; grotere sites analyseer je in delen.
- **Zonder Max Audit geen JavaScript-rendering.** Op een site die zijn content via JavaScript laadt, ziet een lagere tier minder dan er staat.
- **Keyword-data is per land en taal.** Kies de juiste markt, anders zijn de volumes niet van jouw publiek.

## Problemen oplossen

**De audit blijft op "bezig" staan.** Grote crawls duren minuten. Blijft het langer dan een kwartier hangen, start dan opnieuw; mislukte audits worden terugbetaald.

**De score is veel lager dan verwacht.** Kijk of je een lagere tier gebruikte op een JavaScript-site: zonder rendering leest de audit een vrijwel lege pagina. Draai een Max Audit of Website-crawl Pro.

**Core Web Vitals zijn leeg.** Google levert die alleen als er genoeg meetdata is. Voor een nieuwe of weinig bezochte pagina is dat normaal.

**Er worden gebroken links gemeld die werken.** Sommige servers blokkeren geautomatiseerde verzoeken. Controleer de link handmatig; werkt hij, dan kun je de melding negeren.

**Je zoekwoorden staan er niet bij.** Controleer het ingestelde land en de taal. Zoekwoorden zonder meetbaar volume worden weggelaten.

## Veelgestelde vragen

**Wat is het verschil tussen een pagina-analyse en een website-crawl?**
Diepte tegenover breedte. De audit gaat de diepte in op één pagina, met
AI-aanbevelingen, keyword-posities en Core Web Vitals. De crawl gaat de breedte
over je hele site, met honderd mechanische checks, dubbele titels en gebroken
links, maar zonder AI-advies per pagina.

**Hoe vaak moet ik auditen?**
Na elke grote wijziging, en verder maandelijks. Je kunt het ook automatisch
laten draaien, dan zie je de trend zonder eraan te denken.

**Kan ik het rapport aan een klant geven?**
Ja. Exporteer als PDF; op Pro en hoger zet je daar je eigen logo, kleur en
bureaunaam op.

**Werkt dit ook voor webshops?**
Ja. Let bij grote webshops op de pagina-limiet en crawl in delen, bijvoorbeeld
per categorie.

**Wat is het verschil met de GEO Engine?**
De SEO Engine meet je positie in Google. De [GEO Engine](geo-engine.md) meet of
AI-assistenten je noemen. Steeds vaker heb je allebei nodig.

## Tips

- **Start met een Standaard Audit** voor een volledig beeld van je belangrijkste landingspagina
- **Geef een doelzoekwoord op** voor pagina's die je op een specifieke term wilt laten ranken
- **Gebruik een Deep Audit** bij een nieuwe site of na een redesign
- **Vergelijk audits** in de historie om te zien of je wijzigingen effect hadden

---

→ Verder: [GEO Engine](geo-engine.md) · [Authority Engine](authority-engine.md) · [Alle Groei Tools](../engines/README.md)
→ Op de site: [SEO Engine](https://dgenix.nl/engines/seo) · [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, SEO Engine, bijgewerkt augustus 2026*
