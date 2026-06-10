# Google Search Console

Zoekwoorden rapport, pagina-prestaties en SEO-kansen op basis van echte Google Search Console data. Ontdek welke queries verkeer genereren en waar je rankings kunnen verbeteren.

**Vereisten:** Growth+ abonnement, Google-account koppelen via Instellingen

---

## Beschikbare acties

| Actie | Creditkosten | Omschrijving |
|---|---|---|
| `zoekwoorden_rapport` | 50 cr | Top zoekwoorden met klikken, impressies, CTR en gemiddelde positie |
| `pagina_prestaties` | 35 cr | Prestatie per URL: clicks, impressies, CTR, positie |
| `seo_kansen` | 450 cr | Strategische SEO-analyse met AI-aanbevelingen (Sonnet) |

---

## Verbinding koppelen

1. Ga naar **Instellingen > Integraties**
2. Klik op **Verbinden** bij Search Console
3. Log in met het Google-account dat eigenaar is van de Search Console property
4. Geef toestemming voor `webmasters.readonly`

Bij het eerste gebruik vraagt de assistent naar je website-URL zodat de juiste property geselecteerd kan worden.

---

## Voorbeeldgesprekken

**Zoekwoorden rapport:**
> "Welke zoekwoorden brengen het meeste verkeer naar mijn site de afgelopen 28 dagen?"

**Pagina-analyse:**
> "Analyseer de prestaties van mijn homepage in Search Console"

**SEO-kansen:**
> "Welke SEO-verbeteringen kan ik doorvoeren op basis van mijn Search Console data?"

---

## Tips

- `seo_kansen` gebruikt Claude Sonnet voor de beste analyse (450 cr) — gebruik maandelijks voor strategische planning
- Filter op pagina-URL om diep in te zoomen op specifieke landingspaginas
- Combineer met Google Analytics voor een volledig beeld van verkeer en gedrag
- Lage CTR bij hoge impressies = sterke opportunity voor title/meta optimalisatie

---

## Beperkingen

- Alleen lezen (geen wijzigingen in Search Console mogelijk)
- Data heeft een vertraging van 2-3 dagen
- URL-inspectie en sitemaps zijn niet beschikbaar via deze skill
- Maximaal 1.000 rijen per query (Google API limiet)
