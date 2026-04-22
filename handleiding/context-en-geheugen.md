# Context en geheugen

Je assistent weet wie je bent, hoe je werkt en wat jij belangrijk vindt — niet omdat je dat elke keer opnieuw vertelt, maar omdat hij context opbouwt uit meerdere bronnen. Dit document legt uit hoe dat systeem werkt.

---

## Hoe laadt de assistent context?

Vóór elk gesprek combineert je assistent automatisch de volgende informatiebronnen:

```
[Platformkennis] + [Kennisdocument] + [Persoonlijke instructies] + [Geheugen] + [Kennisbank] + [Projectinstructies]
```

Al die informatie is beschikbaar op het moment dat je een bericht stuurt. Je hoeft niets te activeren — het werkt automatisch.

---

## 1. Kennisdocument

Het kennisdocument is het belangrijkste bestand dat je assistent over jou weet. Het wordt aangemaakt tijdens de intake en bevat jouw profiel:

- Wie je bent en wat je doet
- Je bedrijf, sector en rol
- Hoe je wil werken en communiceren
- Wat je assistent van jou moet weten

**Waar vind je het?**
- Dashboard → Assistent (ingeklapt accordeon bovenaan de chat)
- Instellingen → AI Assistent → Kennisdocument

**Hoe bewerk je het?**
Klik op "Bewerken" in het accordeon. Je kunt de tekst direct aanpassen. Sla op — je assistent gebruikt de nieuwe versie direct bij het volgende gesprek.

**Tip:** hoe meer relevante informatie hier staat, hoe beter je assistent op jou is afgestemd. Voeg toe:
- Je bedrijfsnaam, sector en doelgroep
- Je werkwijze en stijlvoorkeur
- Vaste formats die je gebruikt (bijv. hoe een offerte eruitziet)
- Mensen die regelmatig terugkomen in je werk

**Bestandsformaat:** het kennisdocument is een `.md` bestand (Markdown). Dit is gewone tekst met optionele opmaak zoals headers en lijstjes. Je hoeft geen Markdown te kennen — de assistent leest ook platte tekst prima.

---

## 2. Persoonlijke instructies (Custom Rules)

Persoonlijke instructies zijn vaste regels die je assistent altijd opvolgt, ongeacht het gesprek of het project. Ze worden niet overschreven door andere context.

**Voorbeelden:**
- "Antwoord altijd in punten, nooit in lange alinea's"
- "Gebruik altijd een professionele toon voor e-mails, maar informeel voor Slack-berichten"
- "Noem me nooit 'u' — altijd 'jij'"
- "Als ik iets vraag over marketing, gebruik dan altijd de AIDA-structuur"

**Waar stel je het in?**
Instellingen → AI Assistent → Persoonlijke instructies

Instructies zijn vrije tekst. Schrijf ze zoals je ze ook aan een nieuwe medewerker zou uitleggen.

---

## 3. Geheugen

Het geheugen is de automatische kennisopbouw van je assistent. Na gesprekken slaat hij relevante feiten op — zonder dat jij er iets voor hoeft te doen.

**Wat onthoudt hij?**
- **Feiten** — wie je bent, je rol, je bedrijf
- **Voorkeuren** — hoe je communiceert, welke tools je gebruikt
- **Contacten** — mensen die regelmatig terugkomen
- **Patronen** — terugkerende werkwijzen of gewoonten

**Hoe lang blijft het bewaard?**
Onbeperkt, tenzij je het verwijdert.

**Beheren:**
Instellingen → Geheugen — bekijk, verwijder of exporteer herinneringen.

**Capaciteit per plan:**

| Plan | Max herinneringen |
|---|---|
| Starter | 100 |
| Growth | 500 |
| Pro | 2.000 |

Wanneer je capaciteit vol raakt, archiveer je herinneringen naar je Kennisbank. Ze blijven beschikbaar als achtergrondcontext.

→ Meer details: [Geheugen](../functies/geheugen.md)

---

## 4. Kennisbank — documenten uploaden

De Kennisbank is voor documenten die je assistent als achtergrondkennis moet kennen. In tegenstelling tot het geheugen (automatisch) vul je dit zelf.

**Ondersteunde formaten:**
- `.md` — Markdown bestanden (ideaal voor gestructureerde informatie)
- `.pdf` — PDF documenten
- `.docx` — Word documenten
- `.txt` — Platte tekst

**Gebruik .md bestanden effectief:**

Markdown-bestanden zijn ideaal voor kennisbank-documenten omdat ze makkelijk te schrijven en te structureren zijn. Voorbeeld:

```markdown
# Bedrijfsprofiel — Bakkerij De Krent

## Producten
- Desembrood: €4,50
- Croissants: €1,80 per stuk
- Gebak op bestelling: prijs op aanvraag

## Openingstijden
Dinsdag t/m zaterdag: 07:30–17:00
Zondag: 08:00–13:00

## Communicatiestijl
Warm en persoonlijk. Klanten zijn vaste gasten.
```

De assistent leest dit bestand en gebruikt de informatie bij vragen als "Schrijf een antwoord op een klacht over een bestelling" of "Maak een e-mail over onze zondagse openingstijden."

**Waar upload je bestanden?**
Dashboard → Assistent → tabblad "Kennisbank"

→ Meer details: [Kennisbank](../functies/kennisbank.md)

---

## 5. Projectinstructies

Per projectmap kun je eigen instructies instellen. Die gelden alleen voor gesprekken binnen dat project en combineren met je globale kennisdocument.

**Hoe werkt het?**

Stel je hebt twee projecten:
- "Bakkerij De Krent" — met instructies over formele toon en merkrichtlijnen
- "Eigen projecten" — met instructies over je persoonlijke werkwijze

In het project "Bakkerij De Krent" weet je assistent automatisch voor welke klant hij werkt en hoe hij moet communiceren — zonder dat je dat in elk bericht herhaalt.

**Projectinstructies instellen:**
1. Ga naar Dashboard → Assistent
2. Hover over een projectmap in de zijbalk
3. Klik op het ⚙️-icoon
4. Typ de instructies in het tekstvak
5. Klik op Opslaan

→ Meer details: [Projecten](../functies/projecten.md)

---

## Alles samengevat

| Bron | Aangemaakt door | Doel | Scope |
|---|---|---|---|
| Kennisdocument | Jij (intake + bewerken) | Jouw profiel en werkwijze | Altijd actief |
| Persoonlijke instructies | Jij | Vaste gedragsregels | Altijd actief |
| Geheugen | Assistent (automatisch) | Feiten uit gesprekken | Altijd actief |
| Kennisbank | Jij (uploaden) | Achtergrondkennis | Altijd actief (Growth+) |
| Projectinstructies | Jij | Klant- of projectspecifieke context | Alleen in dat project |

**Prioriteit:** als instructies botsen, winnen de meer specifieke bronnen. Projectinstructies overschrijven niets — ze worden gecombineerd. Persoonlijke instructies gelden altijd.

---

## Praktische tips

**Begin met een goed kennisdocument.** Dit is de investering die het meest oplevert. Vul in: wie je bent, wat je doet, voor wie je werkt en hoe je assistent moet communiceren.

**Gebruik projectinstructies voor herhaalde klanten.** Maak één keer een project aan per vaste klant en stel de context in. Alle gesprekken voor die klant staan bij elkaar en de assistent weet altijd de context.

**Voeg .md-bestanden toe aan je Kennisbank voor terugkerende informatie.** Prijslijst, productcatalogus, standaardantwoorden — upload ze één keer en de assistent gebruikt ze altijd.

**Check je geheugen periodiek.** Je assistent onthoudt misschien dingen die verouderd zijn (een oud project, een vorige baan). Verwijder ze via Instellingen → Geheugen.

**Schrijf persoonlijke instructies als werkregels.** Niet als wensen maar als regels: "Geef altijd drie opties" in plaats van "Geef liefst drie opties."
