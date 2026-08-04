# Connectors

Een connector is de koppeling tussen dGENIX en een account dat van jou is: je mailbox, je agenda, je CRM. Zonder connector kan GENI nergens bij.

Je koppelt een tool één keer via **Dashboard → Connectors**. Daarna gebruikt
GENI hem vanzelf zodra een opdracht erom vraagt; je hoeft nooit te zeggen
*welke* koppeling hij moet aanspreken.

## Connector of skill?

Dit is het meest gestelde vraagstuk bij het opzetten, dus kort:

| | Connector | Skill |
|---|---|---|
| **Wat het regelt** | Of GENI ergens **mag** komen | Wat hij daar kan **doen** |
| **Waar je het instelt** | Dashboard → Connectors | Dashboard → Skills |
| **Voorbeeld** | Toegang tot je Google-account | Mail lezen, agenda plannen |

Je hebt ze allebei nodig. Zet je de Gmail-skill aan zonder Google te koppelen,
dan weet GENI hoe hij mail leest maar is er geen postvak. Andersom heeft hij
toegang maar geen handelingen. Zie
[Hoe alles samenwerkt](../concepten/hoe-alles-samenwerkt.md).

## Zo koppel je een tool

1. Ga naar **Dashboard → Connectors**
2. Kies de connector die je wilt koppelen
3. Doorloop de autorisatie: inloggen bij de dienst, of een sleutel plakken
4. De connector staat op **Verbonden** en alle bijbehorende skills werken direct

Duurt zelden langer dan een minuut, behalve bij de Meta-koppelingen
(WhatsApp en Instagram), die een Developer-account vereisen.

## Beschikbare connectors

### Google Workspace

| Connector | Skill | Plan |
|---|---|---|
| [Gmail](gmail.md) | Gmail | Starter+ |
| [Google Calendar](google-calendar.md) | Google Calendar | Starter+ |
| [Google Drive](google-drive.md) | Google Drive | Starter+ |
| [Google Sheets](google-sheets.md) | Google Sheets | Starter+ |
| [YouTube](youtube.md) | YouTube Manager | Growth+ |

Eén Google-koppeling volstaat niet voor alles: je geeft per dienst apart
toestemming, zodat je zelf bepaalt of GENI alleen je agenda of ook je mail mag
zien.

### Communicatie en samenwerking

| Connector | Skill | Plan |
|---|---|---|
| [Slack](slack.md) | Slack | Growth+ |
| [Notion](notion.md) | Notion | Growth+ |
| [LinkedIn](linkedin.md) | LinkedIn | Growth+ |
| [Microsoft 365](microsoft-365.md) | Microsoft 365 | Growth+ (binnenkort) |
| [Canva](canva.md) | Canva | Starter+ (binnenkort) |

### Social media en berichten

| Connector | Skill | Plan |
|---|---|---|
| [WhatsApp Business](whatsapp-business.md) | WhatsApp Business | Growth+ |
| [Instagram Business](instagram.md) | Instagram DM | Growth+ |

### Financieel en CRM

| Connector | Skill | Plan |
|---|---|---|
| [Stripe](stripe.md) | Stripe Inzichten | Growth+ |
| [HubSpot](hubspot.md) | HubSpot CRM | Growth+ |

### Uitbreidbaar

| Connector | Waarvoor | Plan |
|---|---|---|
| [MCP-connectors](mcp-connectors.md) | Groeiend ecosysteem via een open standaard | Growth+ |

## Twee manieren van koppelen

**Inloggen bij de dienst.** Je klikt op Verbinden, logt in en geeft
toestemming. Dit geldt voor Gmail, Google Calendar, Google Drive, Google Sheets,
YouTube, Slack, Notion, LinkedIn, Microsoft 365 en Canva. De koppeling ververst
zichzelf; je hoeft er niet naar om te kijken.

**Een sleutel plakken.** Je maakt in de andere dienst een sleutel of token aan
en plakt die in dGENIX. Dit geldt voor WhatsApp Business, Instagram Business,
Stripe en HubSpot. Voordeel: je bepaalt bij het aanmaken zelf precies welke
rechten die sleutel krijgt.

## Wat een connector niet doet

- **Niets kopiëren.** Je gegevens blijven bij de dienst zelf staan; er wordt niets binnengehaald of geïndexeerd.
- **Niets verwijderen.** GENI wist geen mail, bestanden, kanalen of contacten.
- **Niets ongevraagd wijzigen.** Alles wat iets verandert of verstuurt, vraagt eerst om bevestiging.
- **Niets meer dan je gaf.** Elke connector-pagina toont precies welke rechten je verleent.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op de connector en kies **Verbreken**.
Vanaf dat moment kan GENI er niet meer bij en stoppen alle skills die ervan
afhangen. Bij de meeste diensten kun je de toegang ook aan hun kant intrekken;
dat staat per connector beschreven.

## Veelgestelde vragen

**Moet ik alles koppelen?**
Nee. Koppel wat je gebruikt. De meeste mensen beginnen met mail en agenda en
breiden later uit.

**Kan iemand anders bij mijn koppelingen?**
Nee. Een connector staat op jouw account. Ook binnen hetzelfde bedrijf deelt
niemand jouw koppelingen.

**Werkt een skill niet terwijl hij aanstaat?**
Bijna altijd omdat de bijbehorende connector ontbreekt of verlopen is. Kijk op
**Dashboard → Connectors** of de dienst nog als Verbonden staat.

**Mijn tool staat er niet bij.**
Kijk of hij via [MCP-connectors](mcp-connectors.md) beschikbaar is, of dien een
verzoek in via de skill-marktplaats.

---

→ Verder: [Hoe alles samenwerkt](../concepten/hoe-alles-samenwerkt.md) · [Skills uitgelegd](../handleiding/skills-uitgelegd.md)
→ Op de site: [alle koppelingen](https://dgenix.nl/integrations) · [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Connectors, bijgewerkt augustus 2026*
