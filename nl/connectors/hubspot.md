# HubSpot koppelen

De HubSpot-koppeling laat GENI contacten opzoeken en aanmaken, deals bijwerken, notities toevoegen en je sales-pipeline samenvatten.

Deze koppeling werkt met een **Private App Token** dat je zelf in HubSpot
aanmaakt, niet met de gebruikelijke inlogknop. Daardoor bepaal jij precies welke
rechten dGENIX krijgt. De koppeling activeert de
[HubSpot-skill](../skills/hubspot.md), beschikbaar vanaf **Growth**.

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Staat jan@bedrijf.nl al in ons CRM?" | Zoekt op e-mail, naam of bedrijf |
| "Voeg deze lead toe als contact" | Maakt een nieuw contact aan |
| "Zet de deal met De Vries op 'offerte verstuurd'" | Maakt of werkt een deal bij |
| "Noteer bij dit contact dat ze in maart terugbellen" | Voegt een notitie toe |
| "Hoe staat mijn pipeline ervoor?" | Geeft alle deals per fase |

## Koppelen

1. Log in op HubSpot en ga naar *Instellingen → Integraties → Private Apps*
2. Klik op **Een private app aanmaken** en geef hem een naam, bijvoorbeeld "dGENIX"
3. Open het tabblad **Scopes** en zet aan:
   - `crm.objects.contacts.read` + `.write`
   - `crm.objects.deals.read` + `.write`
   - `crm.objects.notes.write`
4. Klik op **App aanmaken** en kopieer het token dat je krijgt
5. Ga naar **Dashboard → Connectors**, klik op **Koppelen** bij HubSpot en plak het token

Bewaar het token zorgvuldig: HubSpot toont het maar één keer volledig.

## Welke toegang je geeft

| Scope | Waarvoor dGENIX het gebruikt |
|---|---|
| `crm.objects.contacts.read` | Contacten opzoeken |
| `crm.objects.contacts.write` | Nieuwe contacten aanmaken |
| `crm.objects.deals.read` | De pipeline en losse deals lezen |
| `crm.objects.deals.write` | Een deal aanmaken of van fase wisselen |
| `crm.objects.notes.write` | Notities toevoegen aan een contact of deal |

Zet je een scope niet aan, dan kan GENI dat simpelweg niet. Wil je bijvoorbeeld
alleen laten lezen, laat de `.write`-scopes dan uit.

## Controleren of het werkt

Vraag direct na het koppelen:

```
Hoe staat mijn HubSpot-pipeline ervoor?
```

Je krijgt je deals per fase terug. Komt er een rechtenfout, dan mist er een
scope in je private app.

## Grenzen

- GENI **verwijdert** nooit contacten, deals of notities
- Een contact aanmaken of een deal bijwerken vraagt om bevestiging
- Alleen contacten, deals en notities; tickets, producten en offertes niet
- Aangepaste eigenschappen worden niet automatisch ingevuld
- E-mails versturen loopt niet via HubSpot maar via je e-mailkoppeling

## Problemen oplossen

**Rechtenfout bij een actie.** De bijbehorende scope staat uit. Open je private app in HubSpot, vink hem aan en sla op; het token blijft hetzelfde.

**Het token wordt niet geaccepteerd.** Je plakte waarschijnlijk de Client secret of een oude API-sleutel. Het gaat om het **access token** van de private app.

**Een deal komt in de verkeerde pipeline.** Zonder aanduiding gebruikt HubSpot je standaardpipeline. Noem de pipeline in je opdracht.

## Verbinding verbreken

Verwijder de private app in HubSpot, of ga naar **Dashboard → Connectors**, klik
op HubSpot en kies **Verbreken**. Verwijder je de app in HubSpot, dan is het
token direct ongeldig.

## Veelgestelde vragen

**Waarom geen gewone inlogknop zoals bij Slack?**
Met een private app bepaal je zelf, per scope, wat dGENIX mag. Dat is preciezer
dan een standaard-autorisatie waarbij je alles in één keer goedkeurt.

**Werkt dit met een gratis HubSpot-account?**
Private apps zijn beschikbaar in de gratis CRM-tiers. Sommige velden en
pipelines vragen wel om een betaald HubSpot-plan.

**Kan GENI mijn hele CRM doorzoeken?**
Hij zoekt gericht, op e-mail, naam of bedrijf. Er wordt niets gekopieerd of
geïndexeerd; elke zoekopdracht gaat live naar HubSpot.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [HubSpot CRM skill](../skills/hubspot.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, HubSpot koppelen, bijgewerkt augustus 2026*
