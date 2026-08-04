# Google Calendar

Met de Google Calendar-skill kijkt GENI in je agenda en plant hij afspraken in, zodat je niet zelf hoeft te puzzelen met tijdsloten.

Beschikbaar vanaf **Starter**. Je hebt een gekoppeld Google-account nodig; zie
[Google Calendar koppelen](../connectors/google-calendar.md).

## Wat kan GENI met Google Calendar?

- **Je agenda bekijken** voor een dag, week of zelfgekozen periode
- **Een afspraak inplannen** met datum, tijd, titel en locatie

Daarmee kun je je dagprogramma opvragen, vrije blokken laten zoeken en
afspraken laten maken zonder de agenda-app te openen.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Wat staat er morgen op mijn agenda?
```

> **Donderdag 7 augustus**
>
> - **10:00-11:00** , Klantgesprek De Vries
> - **13:30-14:30** , Leverancier, Industrieweg 4
> - **16:00-17:00** , Teamoverleg
>
> Je hebt één vrij blok van 11:00 tot 13:30.

Bij het inplannen zie je eerst wat er komt te staan:

```
Plan vrijdag om 14:00 een uur in met ABC over de offerte
```

> **Klantgesprek ABC , offerte**
> Vrijdag 8 augustus, 14:00-15:00
>
> Dit staat niet in de weg van je andere afspraken. Zal ik hem aanmaken?

## Vereisten

- **Plan:** Starter en hoger
- **Koppeling:** een Google-account via **Dashboard → Connectors**

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Google Calendar**
2. Ga naar **Dashboard → Connectors** en klik op **Verbinden**
3. Doorloop het Google-toestemmingsscherm
4. De agenda is direct bruikbaar

## Wat het kost

| Actie | Credits |
|---|---|
| Agenda opvragen | ~20 |
| Afspraak aanmaken | ~28 |
| Vrije tijd zoeken | ~20 |

De skill zit in je plan; je betaalt per actie. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Een afspraak aanmaken vraagt om bevestiging.** Je ziet datum, tijd en titel eerst.
- **GENI verwijdert of verzet geen bestaande afspraken.**
- **Genodigden uitnodigen kan niet.** Hij maakt de afspraak; deelnemers voeg je zelf toe.
- **Terugkerende afspraken worden gelezen, niet aangemaakt.**
- **Alleen de agenda's van het gekoppelde account.** Agenda's van collega's blijven buiten beeld.
- **Hij werkt in de tijdzone van je account.** Controleer die als tijden afwijken.

## Problemen oplossen

**Je agenda blijft leeg.** De koppeling ontbreekt of is verlopen, of je afspraken staan in een andere agenda dan de hoofdagenda van het gekoppelde account.

**De afspraak staat op het verkeerde tijdstip.** Waarschijnlijk een tijdzoneverschil. Controleer de tijdzone in [Instellingen](../functies/instellingen.md).

**Een dubbele boeking wordt niet gesignaleerd.** Vraag expliciet of het conflicteert; dan controleert GENI je bestaande afspraken.

**Je wilt iemand uitnodigen.** Dat gaat niet via GENI. Maak de afspraak en voeg de genodigden zelf toe in Google Calendar.

## Veelgestelde vragen

**Kan GENI elke ochtend mijn dag doornemen?**
Ja, als geplande taak. Vaak in combinatie met [Gmail](gmail.md), zodat je agenda
en actiepunten in één bericht krijgt. Zie
[Geplande taken](../handleiding/geplande-taken.md).

**Werkt dit met meerdere agenda's?**
Hij leest de agenda's van het gekoppelde account. Afspraken maakt hij in je
hoofdagenda.

**Kan ik de skill gebruiken zonder Gmail te koppelen?**
Ja. Je geeft per Google-dienst apart toestemming.

**Ziet dGENIX de inhoud van mijn afspraken?**
Alleen wat nodig is om je vraag te beantwoorden, op het moment dat je hem stelt.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Google Calendar koppelen](../connectors/google-calendar.md) · [Gmail](gmail.md) · [Google Taken](google-tasks.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Google Calendar, bijgewerkt augustus 2026*
