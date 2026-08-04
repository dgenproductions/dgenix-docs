# Hoe alles samenwerkt

dGENIX bestaat uit vijf onderdelen die op elkaar bouwen: je assistent GENI, skills, connectors, credits en de kanalen waarin je hem aanspreekt. Deze pagina laat zien hoe ze in elkaar grijpen.

Losse uitleg per onderdeel staat elders in deze documentatie. Hier gaat het om
het verband, want dat is precies wat mensen missen als iets niet werkt zoals ze
verwachtten.

## De lagen, van onder naar boven

| Laag | Wat het doet | Zonder deze laag |
|---|---|---|
| **Connectors** | Geven toegang tot je eigen accounts | GENI kan nergens bij |
| **Skills** | Geven GENI de vaardigheid om iets te dóén | Toegang zonder handelingen |
| **GENI** | Kiest de juiste skill bij jouw opdracht | Je zou zelf commando's moeten kiezen |
| **Context** | Kennisdocument, geheugen, kennisbank, projecten | Elk gesprek begint bij nul |
| **Credits** | Rekenen het werk af | , |

De belangrijkste regel: **een skill en een connector zijn twee dingen.** De
connector regelt of GENI ergens *mag* komen; de skill bepaalt wat hij daar kan
*doen*. Dat is de meest voorkomende bron van verwarring.

## Waarom skill en connector gescheiden zijn

Stel je zet de Gmail-skill aan maar koppelt geen Google-account. Dan weet GENI
wél hoe hij mail leest en schrijft, maar er is geen postvak. Andersom: koppel je
Google zonder de skill aan te zetten, dan heeft hij toegang maar geen
handelingen.

Dat lijkt omslachtig en is het niet. Je koppelt Google één keer en beslist daarna
per skill wat je aanzet. En trek je de koppeling in, dan zijn alle skills die
ervan afhangen meteen buitenspel , één knop, geen losse eindjes.

## Wat er gebeurt bij één opdracht

Je typt:

```
Vat mijn ongelezen mail samen en zet de actiepunten in mijn agenda
```

Dan gebeurt dit, in deze volgorde:

1. **GENI leest je context.** Kennisdocument, relevante herinneringen en, als je
   in een project zit, de context van dat project.
2. **Hij kiest de skills.** Dit vraagt om Gmail én Google Calendar. Je hoeft ze
   niet te noemen.
3. **Hij controleert de toegang.** Is Google gekoppeld? Zo niet, dan zegt hij dat
   in plaats van te falen.
4. **Hij haalt de mail op** en vat samen.
5. **Hij stelt de agenda-items voor** en vraagt om bevestiging, want dat
   verandert iets.
6. **Na jouw akkoord voert hij uit** en schrijft de credits af.
7. **Hij onthoudt wat relevant is**, bijvoorbeeld dat je actiepunten graag als
   losse agenda-items ziet.

Stap 5 is het patroon dat door het hele platform loopt: **lezen mag altijd,
veranderen vraagt om akkoord.**

## Wat je ziet als er iets ontbreekt

Ontbreekt de koppeling, dan krijg je geen foutmelding maar een uitleg:

> Ik kan je inbox nog niet lezen, want je Google-account is niet gekoppeld.
> Ga naar **Dashboard → Connectors** en klik op Verbinden bij Gmail. Daarna
> pak ik dit direct op.

## Van losse opdracht naar automatisch

Alles wat je met de hand kunt vragen, kun je ook inplannen. Een opdracht die
werkt in de chat, werkt ook als herhaalde taak: elke werkdag om 08:00 een
dagoverzicht, elke maandag een weekrapport.

Het aantal herhaalde taken hangt af van je plan: Starter 1, Growth 5, Pro 10,
Business 20. De uitvoering is identiek aan een handmatige opdracht, inclusief de
bevestiging bij onomkeerbare stappen.

Zie [Geplande taken](../handleiding/geplande-taken.md).

## De Groei Tools staan er bovenop

De vijf engines (SEO, GEO, Authority, Reputation en AI Content) zijn geen losse
skills maar zwaardere machines die op dezelfde lagen draaien. Ze meten iets aan
je website of je reputatie en leveren een rapport plus concrete verbeteringen.

Wat ze bijzonder maakt: GENI kan ze combineren met gewone skills. Een audit
draaien, de resultaten in een document zetten en dat mailen is één opdracht, geen
drie.

Zie [De vijf Growth Engines](../engines/README.md).

## Dezelfde assistent in elk kanaal

Dashboard, Telegram en spraak zijn drie deuren naar dezelfde assistent. Je
gesprekshistorie, je geheugen en je skills zijn overal gelijk. Je begint een
gesprek op je laptop en maakt het af op je telefoon.

Het dashboard is de enige plek waar je instelt: skills aanzetten, accounts
koppelen, verbruik bekijken.

## Grenzen

- **Zonder connector geen toegang.** Er is geen achterdeur; GENI komt alleen waar
  jij hem binnenlaat.
- **Een skill werkt niet half.** Ontbreekt de koppeling, dan zegt GENI dat,
  in plaats van een half resultaat te leveren.
- **Onomkeerbare acties vragen altijd om akkoord**, ook binnen een herhaalde taak.
- **Credits gaan op uitvoering**, niet op nadenken. Mislukt een betaalde actie,
  dan komen ze terug.
- **Projecten delen niets met elkaar.** Dat is opzet, maar betekent dat context
  niet vanzelf overwaait.

## Veelgestelde vragen

**Moet ik zeggen welke skill hij moet gebruiken?**
Nee, GENI kiest zelf. Wil je toch sturen, dan kan het: *"gebruik de Social Media
Manager om..."*.

**Waarom werkt een skill niet terwijl hij aanstaat?**
Bijna altijd omdat de bijbehorende connector ontbreekt of is verlopen. Kijk op
**Dashboard → Connectors** of het account nog als Verbonden staat.

**Kan GENI meerdere skills in één opdracht combineren?**
Ja, en dat is het punt. Mail lezen, samenvatten, een agenda-item maken en het
resultaat in een document zetten kan in één zin.

**Wat gebeurt er als mijn credits op zijn?**
Betaalde acties stoppen tot je maandtegoed wordt aangevuld of je bijkoopt.
Bijkopen kan vanaf Starter; op Free geldt een harde limiet.

---

→ Verder: [Wat is dGENIX](wat-is-dgenix.md) · [Contextopslag vergeleken](context-opslag-vergeleken.md)
→ Diepgang: [Skills uitgelegd](../handleiding/skills-uitgelegd.md) · [Connectors](../connectors/README.md) · [Het creditsysteem](../hoe-het-werkt/credits.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [de vijf Growth Engines](https://dgenix.nl/engines) · [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, Hoe alles samenwerkt, bijgewerkt augustus 2026*
