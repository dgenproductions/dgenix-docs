# Spraakbericht

Met de Spraakbericht-skill luistert GENI naar een ingesproken bericht en vertelt hij
je wat er gevraagd wordt, hoe het klinkt en wat je ermee moet.

Beschikbaar vanaf **Growth**. Je hebt geen koppeling nodig; je deelt een bestand of
geeft een link op.

## Wat kan GENI met een spraakbericht?

Het verschil met een transcriptie zit hem in het woord "luisteren". Een transcriptie
zet de woorden op papier en daarmee is de toon weg: of iemand twijfelde, gehaast was
of juist iets toezegde staat nergens. Bij deze skill gaat de opname zelf naar het
model, dus die informatie komt mee.

Je krijgt terug:

- **De kern** in één zin, wat wil deze persoon
- **De toon**, en waaraan je dat hoort
- **Wat er gezegd is**, in bondige punten, geen letterlijk transcript
- **Wat jij moet doen**, of expliciet dat er geen actie nodig is
- **Hoe urgent het is**, met de reden erbij

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Luister dit bericht van een klant af en vertel me wat ik moet doen
```

> **Kern:** hij wil weten of de levering van vrijdag nog haalbaar is.
>
> **Toon:** zakelijk maar gespannen. Hij praat snel, herhaalt de datum twee keer
> en eindigt met "laat even weten hè".
>
> **Wat er gezegd is**
> - De order van vorige week is bevestigd, maar hij heeft geen verzenddatum gezien
> - Zijn eigen klant verwacht het product maandag
> - Hij noemt kort dat het vorige keer ook later was
>
> **Actie:** bel vandaag terug met een harde verzenddatum, of meld het als het niet
> vrijdag wordt.
>
> **Urgentie:** hoog. Hij heeft zelf een afspraak richting maandag en verwijst naar
> een eerdere vertraging.

Geef je er context bij, bijvoorbeeld van wie het bericht is of waar het over gaat,
dan wordt de analyse scherper.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** geen

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Spraakbericht**
2. Stuur het bericht mee in de chat, of geef een link naar het audiobestand

## Wat het kost

**60 credits per bericht**, ongeacht de lengte. Een bericht van twintig seconden
kost dus evenveel als een van tien minuten. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Bedoeld voor korte berichten.** Tot ongeveer een kwartier. Voor een vergadering
  van een uur gebruik je [Audio Transcriptie](transcriptie.md).
- **Drie formaten:** WAV, MP3 en M4A. Andere formaten worden geweigerd.
- **Maximaal 25 MB** per bestand.
- **Geen letterlijk transcript.** Je krijgt een samenvatting met toon en actie. Wil
  je de exacte woorden, dan is Audio Transcriptie de juiste skill.
- **Sprekers worden niet met naam herkend.** Bij meerdere stemmen benoemt GENI ze
  als Spreker 1 en Spreker 2.
- **Toon is een inschatting.** Het blijft een interpretatie van hoe iets klinkt,
  geen feit over hoe iemand zich voelt.

## Problemen oplossen

**Het bestand wordt niet opgehaald.** Controleer of de link openbaar bereikbaar is
en direct naar het audiobestand wijst, niet naar een pagina eromheen.

**Hij zegt dat het formaat niet ondersteund wordt.** Zet de opname om naar WAV, MP3
of M4A. WhatsApp levert vaak een ander formaat aan.

**Er komt geen analyse terug.** De opname is dan waarschijnlijk stil of
onverstaanbaar. In dat geval worden de credits teruggestort.

**Ik wilde de letterlijke tekst.** Gebruik [Audio Transcriptie](transcriptie.md);
die schrijft woord voor woord uit.

## Veelgestelde vragen

**Wat is het verschil met Audio Transcriptie?**
Transcriptie geeft je de woorden, deze skill geeft je de betekenis en de toon.
Transcriptie rekent per minuut en is gemaakt voor lange opnames; deze skill heeft
een vaste prijs en is gemaakt voor korte berichten.

**Kan ik een WhatsApp-voicemail rechtstreeks doorsturen?**
Je kunt het bestand meesturen in de chat of een link opgeven. Zie
[Bestanden](../functies/bestanden.md).

**Wat als er meerdere mensen praten?**
Dat werkt, maar zonder namen. GENI onderscheidt de stemmen als Spreker 1 en 2.

**In welke taal krijg ik het antwoord?**
In het Nederlands, ook als het bericht in een andere taal is ingesproken.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Audio Transcriptie](transcriptie.md) · [WhatsApp Business](whatsapp-business.md) · [Bestanden](../functies/bestanden.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)

*dGENIX Docs, Spraakbericht, bijgewerkt augustus 2026*
