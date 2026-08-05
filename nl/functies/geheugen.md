# Geheugen (Memory AI)

Het geheugen van GENI is het bindweefsel van dGENIX. Alles wat je op het platform doet komt automatisch in het geheugen van je assistent, zodat GENI je werk kent, meedenkt en op eerder werk doorbouwt. Je geheugen is strikt privé en alleen van jou.

De Geheugen-pagina (**Dashboard → Geheugen**, Brain-icoon in de zijbalk) geeft je direct inzicht in alles wat GENI over jou onthoudt.

---

## Eén verweven geheugen

Het geheugen bestaat uit drie samenwerkende lagen:

1. **Wat GENI weet over jou**: feiten, voorkeuren, doelen en instructies die je zelf toevoegt of die GENI uit je gesprekken oppikt.
2. **Wat je op het platform doet**: elke afbeelding, audit, transcriptie, afgeronde taak en automation-run landt automatisch in je geheugen. Zo weet GENI waar je mee bezig bent.
3. **Je documenten en notities**: je kennisbank en je Werkruimte-notities zijn doorzoekbaar en verbonden met hetzelfde geheugen.

GENI bereikt hetzelfde geheugen op elk kanaal: het dashboard, Telegram, spraakgesprekken en geplande taken.

---

## Wat zijn herinneringen?

Herinneringen zijn korte, persoonlijke feiten die GENI als context gebruikt. Er zijn acht types:

| Type | Voorbeeld |
| --- | --- |
| **Feit** | "Ik werk bij een marketingbureau in Amsterdam" |
| **Voorkeur** | "Ik wil antwoorden altijd in bullet points" |
| **Doel** | "Ik wil mijn e-mailresponstijd halveren" |
| **Instructie** | "Houd antwoorden altijd onder 150 woorden" |
| **Contact** | "Mijn vaste ontwerper is Lisa" |
| **Patroon** | "Ik plan altijd op maandag" |
| **Situatie** | "We zitten in een groeifase, team van 3" |
| **Vaardigheden** | "Ik ben expert in copywriting, geen developer" |

Feiten, voorkeuren, doelen en instructies staan als knooppunten rond het brein bovenaan de pagina; alle types staan als uitvouwbare rijen eronder.

---

## Vraag je geheugen (semantisch zoeken)

Met de zoekbalk "Vraag je geheugen" doorzoek je alles wat GENI over je weet op **betekenis**, niet op trefwoord. Typ bijvoorbeeld "wat weet je over mijn schrijfstijl?" en GENI haalt de relevante herinneringen terug, ook als je andere woorden gebruikte dan in de herinnering staan.

> Slim doorzoeken gebruikt AI en kost een kleine hoeveelheid credits per zoekopdracht. Beschikbaar vanaf Starter.

---

## Wat GENI over je leerde (activiteit)

De activiteit-tijdlijn toont wat je recent op het platform deed, van gegenereerde afbeeldingen tot voltooide audits en taken. Dit is wat GENI automatisch heeft opgemerkt en meeneemt in zijn context, zodat je vragen kunt stellen als "ga verder met de SEO-audit van gisteren".

---

## Per merk of project (brand-switching)

Werk je voor meerdere merken of klanten? Maak een project aan in de AI Assistent en GENI houdt het geheugen per project gescheiden. Bovenaan de Geheugen-pagina wissel je tussen je **Hoofdgeheugen** en je projecten. Wat je in een project toevoegt, blijft aan dat project gekoppeld en lekt niet naar je andere werk.

---

## Proactieve GENI (optioneel)

Zet je **Proactieve GENI** aan (in **Instellingen → AI-assistent**), dan denkt GENI één keer per dag met je mee op basis van wat je deed: het zet voorgestelde vervolgtaken klaar in je Werkruimte en stuurt een korte update. Standaard uit, geen spam, altijd door jou goed te keuren.

---

## Herinneringen toevoegen, bewerken en verwijderen

- **Toevoegen**: via de invoerbalk (kies type, optioneel een titel, typ de inhoud) of gewoon door het in de chat te zeggen: *"Onthoud dat ik elke ochtend met de inbox begin."* GENI slaat het dan op met de `geheugen_opslaan`-tool.
- **Bewerken**: klik op het potlood-icoon naast een herinnering.
- **Verwijderen**: klik op het prullenbak-icoon. Via de Beheer-balk kun je ook meerdere tegelijk selecteren, importeren/exporteren (JSON) of naar de kennisbank archiveren.

---

## Kennisdocument

Onderaan de pagina vind je een samenvatting van je kennisdocument, de persoonlijke context uit **Instellingen → Kennisdocument**. Dit werkt als langetermijngeheugen: het is altijd aanwezig in de context van je assistent, ongeacht je plan.

---

## Wat je hiermee kunt

| Wat je doet | Wat GENI ermee doet |
|---|---|
| Iets vertellen in een gesprek | Slaat het op als het relevant blijft voor later |
| "Onthoud dat..." zeggen | Legt het direct vast als herinnering |
| Een vraag stellen over eerder werk | Zoekt op betekenis in je geheugen en activiteit |
| Wisselen naar een project | Gebruikt eerst de herinneringen van dat project |
| Een herinnering corrigeren | Past hem aan of gooit hem weg, jij houdt de regie |

## Wat je ziet

Je werkt een paar weken met GENI en vraagt dan iets waar je hem nooit expliciet
over verteld hebt:

```
Schrijf een offerte voor mevrouw De Vries
```

> Ik heb de offerte opgesteld met wat ik van je weet:
>
> - **formele toon**, zoals je voorkeur is
> - **30 dagen geldig**, dat hanteer je standaard
> - je **btw-nummer en bankgegevens** onderaan
> - opgemaakt vanuit **Installatiebedrijf Jansen**
>
> Ik heb de prijzen uit je catalogus gehaald. Zal ik hem als PDF klaarzetten?

Niets daarvan heb je in deze opdracht getypt. Dat is het verschil tussen een
chatvenster en een assistent die je kent.

## Grenzen

- **Je geheugen is strikt van jou.** Niemand anders kan erbij, ook niet binnen hetzelfde bedrijf.
- **GENI verzint niets bij.** Weet hij iets niet, dan vraagt hij het in plaats van te gokken.
- **Een verkeerde herinnering blijft doorwerken** tot je hem aanpast. Klopt iets structureel niet, corrigeer het dan in je kennisdocument in plaats van steeds bij te sturen.
- **De opslaglimiet hangt af van je plan**: 100 op Free en Starter, 500 op Growth, 2.000 op Pro, 5.000 op Business.
- **Bij de limiet archiveert GENI zelf** de minst belangrijke herinneringen naar je kennisbank; er gaat niets zomaar verloren.
- **Projectherinneringen blijven in dat project.** Dat is opzet, maar betekent dat je iets soms twee keer vertelt.
- **Semantisch zoeken zit vanaf Starter.** Op Free werkt het geheugen wel, alleen zonder zoeken op betekenis.

## Problemen oplossen

**GENI weet iets niet meer.** Kijk op de Geheugen-pagina of het er staat. Zo niet, zeg het opnieuw met "onthoud dat...".

**Hij gebruikt verouderde informatie.** Zoek de herinnering op en pas hem aan of verwijder hem; een nieuwe toevoegen laat de oude staan.

**Hij haalt klanten door elkaar.** Klantspecifieke feiten horen in een [project](projecten.md), niet in je algemene geheugen.

**Je zit aan de limiet.** GENI archiveert zelf naar je kennisbank. Wil je zelf opruimen, verwijder dan verouderde herinneringen op de Geheugen-pagina.

**Er wordt te veel opgeslagen.** Je kunt elke herinnering verwijderen, en met "wis alle herinneringen" begin je opnieuw.

## Veelgestelde vragen

**Wat komt er automatisch in mijn geheugen?**
Alles wat je op het platform maakt of doet: afbeeldingen, transcripties, SEO/GEO-audits, afgeronde taken en automations. Plus de feiten die GENI uit je gesprekken oppikt.

**Zijn herinneringen zichtbaar voor anderen?**
Nee. Je geheugen is volledig privé en strikt gekoppeld aan jouw account, nooit gedeeld of gemixt met andere gebruikers.

**Hoeveel kan ik opslaan?**
Afhankelijk van je plan (van 100 op Free en Starter tot 5.000 op Business). Bij de limiet archiveert GENI automatisch de minst belangrijke herinneringen naar je kennisbank.

---

→ Verder: [Werkruimte](werkruimte.md) · [Projecten](projecten.md) · [Kennisbank](kennisbank.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, Geheugen (Memory AI), bijgewerkt augustus 2026*
