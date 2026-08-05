# Gmail koppelen

De Gmail-connector geeft GENI toegang tot je inbox, zodat hij mail kan lezen, samenvatten en opstellen, en concepten klaarzet die jij alleen nog hoeft te bevestigen.

## Wat je hiermee kunt

| Wat GENI doet | Voorbeeld |
|---|---|
| Je inbox samenvatten | "Wat is er belangrijk in mijn ongelezen mail?" |
| Een specifieke mail openen | "Lees de mail van Sofie over de offerte" |
| Een mail opstellen en versturen | "Mail Jan dat de afspraak van morgen doorgaat" |

De koppeling activeert de **[Gmail-skill](../skills/gmail.md)**, beschikbaar vanaf Starter.

## Koppelen

1. Ga naar **Dashboard → Connectors**
2. Klik op **Verbinden** naast Gmail
3. Je gaat naar het toestemmingsscherm van Google
4. Log in en geef de gevraagde rechten
5. Na goedkeuring staat de connector op **Verbonden**

## Welke toegang je geeft

| Recht | Waarvoor dGENIX het gebruikt |
|---|---|
| E-mail lezen | Inbox samenvatten, berichten opzoeken en openen |
| E-mail versturen | Een opgestelde mail verzenden na jouw bevestiging |
| Labels beheren | Nieuwsbrieven herkennen en archiveren |

dGENIX **verwijdert nooit** e-mail, en verstuurt niets zonder dat jij het
expliciet bevestigt. Je ziet de concepttekst altijd eerst.

## Controleren of het werkt

Vraag GENI direct na het koppelen:

```
Vat mijn 5 laatste ongelezen mails samen
```

Je krijgt per mail de afzender, het onderwerp en de kern. Blijft het leeg
terwijl je wel ongelezen mail hebt, dan is het verkeerde Google-account
gekoppeld.

## Grenzen

- GENI verwijdert nooit e-mail
- Versturen gebeurt pas na jouw bevestiging, ook bij een herhaalde taak
- Hij leest alleen de mailbox van het gekoppelde account, geen gedeelde postvakken van collega's
- Bijlagen worden herkend, maar niet automatisch geopend; vraag er expliciet om

## Problemen oplossen

**Koppeling mislukt.** Controleer of je in je browser bent ingelogd op het juiste Google-account. Log uit bij Google en probeer het opnieuw.

**GENI ziet je mail niet.** Je hebt een ander Google-account gekoppeld dan waar je mail binnenkomt. Verbreek de verbinding en koppel het juiste account.

**Verzenden lukt niet.** De koppeling is gemaakt zonder verzendrechten. Verbreek de verbinding en koppel opnieuw, en geef dan alle gevraagde rechten.

## Verbinding verbreken

Ga naar **Dashboard → Connectors**, klik op Gmail en kies **Verbreken**.
Je kunt de toegang ook intrekken bij Google zelf via
[myaccount.google.com/permissions](https://myaccount.google.com/permissions).

## Veelgestelde vragen

**Koppelt dit ook meteen Calendar, Drive en Sheets?**
Nee. Elke Google-dienst is een eigen connector met eigen rechten, ook binnen hetzelfde account. Zo geef je nooit meer toegang dan je nodig hebt.

**Kan GENI namens mij mailen zonder dat ik het zie?**
Nee. Elke verzending vraagt om bevestiging en je ziet de tekst vooraf.

**Werkt dit met een Google Workspace-account van mijn bedrijf?**
Ja, mits je beheerder toestaat dat externe apps gekoppeld worden.

---

→ Terug naar [Connectors overzicht](README.md)
→ Zie ook: [Gmail skill](../skills/gmail.md)
→ Op de site: [alle koppelingen](https://dgenix.nl/integrations) · [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Gmail koppelen, bijgewerkt augustus 2026*
