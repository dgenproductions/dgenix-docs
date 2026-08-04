# Reputation Engine

De [Reputation Engine](https://dgenix.nl/engines/reputation) vraagt je eigen klanten om een Google-review, via een branded e-mail met een directe review-link, en houdt bij wie er reageert.

Reviews komen zelden vanzelf. De meeste tevreden klanten laten er geen achter
omdat niemand het vraagt, of omdat ze de link niet kunnen vinden. Deze engine
haalt precies die twee drempels weg. Beschikbaar vanaf **Pro**.

## Wat de Reputation Engine doet

| Onderdeel | Wat het oplevert |
|---|---|
| **Review-link opzoeken** | De directe "schrijf een review"-link van je Google-bedrijfsprofiel |
| **Campagne** | Een lijst klanten die je in één keer benadert |
| **Branded e-mail** | Een verzoek met jouw bedrijfsnaam, de link en een uitschrijfoptie |
| **Statusoverzicht** | Per ontvanger: verzonden, wachtend of uitgeschreven |

## Voorbeeld: wat je vraagt, wat je terugkrijgt

Je vraagt GENI naar de stand van je campagnes:

> **Campagne "Klanten juli"** , 48 contacten
>
> - Verzonden: 44
> - Wachtend: 3
> - Uitgeschreven: 1
>
> Er staan **3 verzoeken klaar** om verstuurd te worden. Zal ik dat doen? Dat
> kost 150 credits.

Zeg je ja, dan gaan die drie de deur uit. Bij meer dan 25 ontvangers vraagt GENI
altijd eerst om bevestiging, ook als je het inplant.

## Hoe je het opzet

1. Ga naar **Groei Tools → Reputation** en maak een campagne aan
2. Geef je bedrijfsnaam op en klik op **Zoek link**; voeg de plaats toe als je bedrijf een veelvoorkomende naam heeft. Je kunt de link ook zelf plakken.
3. Voeg een persoonlijke boodschap toe, optioneel
4. **Plak de e-mailadressen** van je klanten, of klik op **Importeer uit Sheets** en geef een Google Sheets-link (koppel eerst [Google Sheets](../connectors/google-sheets.md))
5. Klik op **Verstuur**

Uitgeschreven adressen worden automatisch overgeslagen; daar hoef je zelf niet
op te letten.

## Met GENI

Je kunt GENI vragen je review-link op te zoeken, de status van een campagne te
geven of een bestaande campagne te versturen. Het opzetten van campagnes en het
toevoegen van contacten doe je in het dashboard, want daar hoort de controle
over een verzendlijst thuis.

Versturen is ook [in te plannen](../handleiding/geplande-taken.md), bijvoorbeeld
elke maandag de nieuwe klanten van die week.

## Veiligheid en AVG

Review-verzoeken zijn e-mail naar echte mensen, dus hier zitten bewust remmen op:

- **Uitschrijflink in elke mail.** Wie zich uitschrijft komt op een suppression-lijst en krijgt nooit meer een verzoek, ook niet uit een andere campagne.
- **Alleen je eigen klanten.** Gekochte of geschraapte lijsten horen hier niet; dat is bovendien in strijd met de AVG.
- **Maandlimiet per plan**: Pro 500, Business 2.000 verzoeken per maand.
- **Bevestiging** bij meer dan 25 ontvangers.
- **Nooit een review-tekst schrijven.** GENI vraagt om een review, hij verzint er geen.

## Wat het kost

| Actie | Credits |
|---|---|
| Review-verzoek, per verzonden e-mail | 50 |
| Review-link opzoeken | 300 |

Een mislukte verzending wordt terugbetaald. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen

- **Alleen Google-reviews.** Trustpilot en andere platformen volgen later.
- **Alleen e-mail.** SMS-verzoeken staan op de planning als optionele add-on.
- **Geen reviews beantwoorden.** De engine vraagt erom; reageren doe je zelf in je Google-profiel.
- **Geen negatieve reviews filteren.** Je kunt niet vooraf selecteren wie waarschijnlijk positief is; dat mag niet van Google en het is niet eerlijk tegenover lezers.
- **Geen garantie op respons.** Een goed getimede vraag helpt, maar of iemand schrijft blijft aan de klant.
- **Reviews verwijderen kan niet.** Dat kan alleen via Google zelf, en alleen bij overtreding van hun beleid.

## Problemen oplossen

**De review-link wordt niet gevonden.** Voeg de plaatsnaam toe. Heeft je bedrijf geen geclaimd Google-bedrijfsprofiel, dan is er ook geen review-link; claim het profiel eerst.

**Mails komen niet aan.** Controleer de adressen op typefouten en vraag de klant in de spammap te kijken. Uitgeschreven adressen worden bewust overgeslagen.

**De Sheets-import leest niets in.** Google Sheets moet gekoppeld zijn en het blad moet een kolom met e-mailadressen bevatten. Een gedeelde link zonder koppeling werkt niet.

**Je zit aan de maandlimiet.** De limiet loopt vanaf je factuurdatum. Wacht op de nieuwe periode of stap over naar Business.

**Een klant kreeg twee keer een verzoek.** Hetzelfde adres staat in twee campagnes. De suppression-lijst geldt voor uitschrijvers, niet voor dubbelingen in je eigen lijsten.

## Veelgestelde vragen

**Mag ik klanten zomaar om een review vragen?**
Je eigen klanten benaderen over een geleverde dienst mag, mits je een
uitschrijfmogelijkheid biedt. Die zit standaard in elke mail. Wat niet mag is
gekochte lijsten gebruiken.

**Kan ik zelf de tekst bepalen?**
Je voegt een persoonlijke boodschap toe die in de mail komt. De opmaak en de
uitschrijflink liggen vast, zodat de mail AVG-proof blijft.

**Werkt dit voor meerdere vestigingen?**
Ja, zet per vestiging een eigen campagne op met de bijbehorende review-link.

**Wat als iemand een slechte review achterlaat?**
Dan heb je waardevolle feedback en de kans om publiek te reageren. Reageren doe
je in je Google-bedrijfsprofiel.

**Ik ben een bureau, kan ik dit voor klanten draaien?**
Ja. Werk per klant in een eigen project, dan blijven lijsten en context
gescheiden. Zie [Projecten](../functies/projecten.md).

---

→ Verder: [GEO Engine](geo-engine.md) · [Authority Engine](authority-engine.md) · [Alle Groei Tools](../engines/README.md)
→ Op de site: [Reputation Engine](https://dgenix.nl/engines/reputation) · [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, Reputation Engine, bijgewerkt augustus 2026*
