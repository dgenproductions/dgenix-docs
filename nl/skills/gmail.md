# Gmail

Met de Gmail-skill leest GENI je inbox, vat hem samen en schrijft en verstuurt e-mail namens jou, in jouw toon.

Beschikbaar vanaf **Starter**. Je hebt een gekoppeld Google-account nodig; zie
[Gmail koppelen](../connectors/gmail.md).

## Wat kan GENI met Gmail?

- **Je inbox lezen** en de recente berichten ophalen
- **Een specifieke mail volledig openen** om de inhoud te beoordelen
- **Een e-mail versturen** naar een of meer ontvangers

Daarmee kun je in de praktijk je inbox laten samenvatten, antwoorden laten
opstellen, nieuwsbrieven laten herkennen en zoeken naar wat een afzender ook
alweer schreef.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Vat mijn ongelezen mail samen
```

> **12 ongelezen, 3 vragen actie**
>
> - **Sofie van Dijk** , offerte akkoord, wil deze week tekenen. *Actie: contract sturen.*
> - **Boekhouder** , btw-aangifte vóór de 25e. *Actie: cijfers aanleveren.*
> - **Jan Bakker** , vraagt of donderdag verzet kan worden.
>
> De andere 9 zijn nieuwsbrieven en notificaties.

Vraag je om een mail te versturen, dan krijg je eerst de tekst te zien:

```
Antwoord Sofie dat het contract er morgen aankomt
```

> **Aan:** sofie@vandijk.nl
> **Onderwerp:** Re: Offerte akkoord
>
> Beste Sofie, fijn dat de offerte akkoord is. Ik stuur het contract morgen
> toe, dan kun je het deze week tekenen.
>
> Zal ik dit versturen?

## Vereisten

- **Plan:** Starter en hoger
- **Koppeling:** een Google-account via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Gmail**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden** bij Gmail
3. Doorloop het Google-toestemmingsscherm
4. Gmail is direct bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| Inbox samenvatten | ~25 |
| E-mail opstellen en versturen | ~35 |
| Mails zoeken | ~15 |

De skill zelf zit in je plan; je betaalt alleen per uitgevoerde actie. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Versturen vraagt altijd om bevestiging.** Je ziet de volledige tekst voordat hij weggaat.
- **GENI verwijdert geen mail.** Ook niet op verzoek; archiveren en opruimen doe je zelf.
- **Bijlagen versturen kan niet.** Hij leest wel bijlagen die jij in de chat meestuurt.
- **Hij leest niet doorlopend mee.** Je inbox wordt alleen opgehaald op het moment dat je erom vraagt.
- **Filters, labels en regels beheren zit er niet in.**
- **Alleen het gekoppelde account.** Meerdere mailboxen tegelijk kan niet.

## Problemen oplossen

**GENI zegt dat hij je inbox niet kan lezen.** De koppeling ontbreekt of is verlopen. Controleer bij **Connectors** of Gmail nog op Verbonden staat.

**Een mail wordt niet gevonden.** Zoek op afzender of onderwerp in plaats van op een losse zin uit de tekst.

**Het antwoord klinkt niet als jij.** Zet je schrijfstijl vast in [Instellingen](../functies/instellingen.md) of leg vaste voorkeuren in je [geheugen](../functies/geheugen.md).

**Versturen mislukt.** Controleer het e-mailadres van de ontvanger op typefouten; Google weigert een ongeldig adres.

## Veelgestelde vragen

**Kan GENI automatisch mijn inbox samenvatten?**
Ja, plan het in als dagelijkse taak. Zie
[Geplande taken](../handleiding/geplande-taken.md).

**Ziet dGENIX mijn wachtwoord?**
Nee. Je logt in bij Google zelf; wij krijgen alleen een intrekbare toegang tot
wat je goedkeurt.

**Werkt dit met een zakelijk Google Workspace-account?**
Ja. Sommige organisaties vragen wel om goedkeuring van een beheerder.

**Kan hij mail versturen vanaf een ander adres?**
Nee, alleen vanaf het gekoppelde account.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Gmail koppelen](../connectors/gmail.md) · [Google Calendar](google-calendar.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Gmail, bijgewerkt augustus 2026*
