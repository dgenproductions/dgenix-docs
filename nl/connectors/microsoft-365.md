# Microsoft 365 koppelen

De Microsoft 365-koppeling laat GENI je Outlook-mail lezen en versturen, je agenda bekijken en meelezen in een Teams-kanaal.

> **Binnenkort beschikbaar.** De koppeling is gebouwd en wacht op de
> Azure OAuth-verificatie van Microsoft. Zodra die rond is, verschijnt Microsoft
> 365 in je Connectors-lijst; je hoeft niets voor te bereiden.

Gebruik je Google in plaats van Microsoft, dan kan dat vandaag al: zie
[Gmail](gmail.md) en [Google Calendar](google-calendar.md).

## Wat je hiermee kunt

| Wat je vraagt | Wat GENI doet |
|---|---|
| "Wat staat er in mijn Outlook-inbox?" | Leest je recente e-mails |
| "Mail Sofie dat de offerte klaarstaat" | Verstuurt een e-mail via Outlook |
| "Wat staat er deze week in mijn agenda?" | Haalt je aankomende afspraken op |
| "Wat is er in het projectkanaal besproken?" | Leest recente berichten uit een Teams-kanaal |

## Koppelen (zodra beschikbaar)

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast Microsoft 365
3. Log in met je werk- of schoolaccount
4. Bekijk de gevraagde rechten en klik op **Accepteren**
5. De [Microsoft 365-skill](https://dgenix.nl/skills/microsoft-365) is direct actief

De skill valt onder **Growth** en hoger.

## Welke toegang je geeft

| Scope | Waarvoor dGENIX het gebruikt |
|---|---|
| `Mail.ReadWrite` | Je Outlook-mail lezen en concepten opstellen |
| `Mail.Send` | Een e-mail versturen na jouw akkoord |
| `Calendars.ReadWrite` | Je agenda bekijken en afspraken plannen |
| `Files.ReadWrite.All` | OneDrive-bestanden ophalen en opslaan |
| `User.Read` | Je naam en e-mailadres lezen |

> **Let op:** in veel organisaties moet een beheerder deze rechten goedkeuren.
> Krijg je bij het inloggen de melding "Goedkeuring vereist", vraag dan je
> IT-beheerder om toestemming te geven.

## Controleren of het werkt

Vraag na het koppelen:

```
Wat staat er in mijn Outlook-inbox?
```

Je krijgt een samenvatting van je recente mail terug.

## Grenzen

- Een e-mail versturen of een afspraak inplannen vraagt om bevestiging
- GENI verwijdert geen mail, agenda-items of bestanden
- In Teams alleen **lezen**; berichten posten kan niet
- Alleen kanalen waarvan je het team en kanaal noemt, geen automatisch overzicht van alles
- Gedeelde postvakken en agenda's van collega's vallen erbuiten

## Problemen oplossen

**Microsoft 365 staat niet in Connectors.** De koppeling is nog niet vrijgegeven. Zie de melding bovenaan deze pagina.

**"Goedkeuring van beheerder vereist" bij het inloggen.** Je organisatie staat apps niet zomaar toe. Je IT-beheerder moet de app goedkeuren in Azure.

**Teams levert niets op.** Je moet team en kanaal aanwijzen; zonder die aanduiding weet GENI niet waar hij moet kijken.

**Je hebt een persoonlijk Microsoft-account.** De koppeling is gericht op werk- en schoolaccounts; een persoonlijk account werkt mogelijk beperkt.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Microsoft 365 en kies **Verbreken**.
Je kunt de toegang ook intrekken via *Microsoft-account → Privacy → Apps en
services*.

## Veelgestelde vragen

**Wanneer is de koppeling er?**
Dat hangt af van Microsofts verificatieproces. Zodra het rond is, verschijnt de
koppeling vanzelf in je dashboard.

**Kan ik Google en Microsoft allebei koppelen?**
Ja. Ze staan los van elkaar; GENI kiest op basis van je opdracht welk account
hij gebruikt.

**Ziet mijn werkgever wat GENI doet?**
Je beheerder ziet dat de app is goedgekeurd en kan de toegang intrekken. Wat je
in dGENIX vraagt, blijft binnen je eigen account.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Gmail](gmail.md) · [Google Calendar](google-calendar.md) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, Microsoft 365 koppelen, bijgewerkt augustus 2026*
