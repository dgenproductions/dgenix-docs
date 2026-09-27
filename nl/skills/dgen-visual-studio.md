# dGEN Visual Studio

dGEN Visual Studio is een AI-studio voor beeld en video, met je eigen stijl en met
terugkerend werk als flow op een canvas. Met deze skill doet GENI dat werk daar voor je: een afbeelding of video maken, of een flow draaien die jij hebt gebouwd.

Beschikbaar vanaf **Growth**. Je hebt de
[dGEN Visual Studio-koppeling](../connectors/dgen-visual-studio.md) nodig en een eigen
studio-account.

## Wat kan GENI hiermee?

Het verschil met [AI Beeldgeneratie](ai-beeldgeneratie.md) en [FLUX](flux-image.md) zit in
het woord *jouw*. Die twee maken snel een los beeld op onze modellen. Deze skill werkt in
jouw studio, met jouw modellen, jouw LoRA-s en jouw bibliotheek, en hij kan iets wat de
andere twee niet kunnen: een flow draaien die jij hebt gebouwd.

| Tool | Wat hij doet |
|---|---|
| `visualstudio_beeld_maken` | Maakt een afbeelding in je studio |
| `visualstudio_video_maken` | Maakt een video (duurt minuten) |
| `visualstudio_flows` | Toont je opgeslagen flows met hun id |
| `visualstudio_flow_draaien` | Draait een flow van begin tot eind |
| `visualstudio_modellen` | De catalogus, met wat elk model aanneemt |
| `visualstudio_bibliotheek` | Je laatste bestanden met een link |
| `visualstudio_bestand_ophalen` | Haalt een bestand op zodat een volgende stap het kan gebruiken |
| `visualstudio_saldo` | Je creditsaldo in de studio |

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Draai mijn weekbanner-flow en zet het resultaat klaar
```

> Je hebt drie flows klaarstaan. Ik draai **Weekbanner** (4 stappen).
>
> Dit kost credits in je studio, niet op je dGENIX-saldo. Zal ik doorgaan?
>
> *[na je bevestiging]*
>
> De flow is klaar; alles staat in je studiobibliotheek.

Zet diezelfde opdracht in een [geplande taak](../handleiding/geplande-taken.md) en je
maandelijkse beeldronde gebeurt vanzelf, elke maandag om acht uur.

## Combineren met andere skills

Alles wat GENI in je studio maakt, komt ook in je dGENIX-bestanden te staan. Daardoor is het
resultaat geen eindpunt maar een schakel:

- **Kennisbank → SEO Blog Schrijver → deze skill → CMS Publisher**, een artikel met een
  passend beeld, als concept klaargezet
- **Geplande taak → deze skill → Social Media Manager**, elke maandag verse beelden met de
  posts erbij ingepland
- **Google Bedrijfsprofiel → deze skill → LinkedIn**, een goede review wordt een beeldcitaat
- **Google Sheets → deze skill → Google Drive**, elke rij zonder beeld krijgt er een

⚠️ Wil je een **bestaand** bestand gebruiken, laat GENI het dan eerst ophalen. De link uit
`visualstudio_bibliotheek` is tijdelijk; een opgehaald bestand blijft werken.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** dGEN Visual Studio, met een eigen studio-account
- **Saldo in de studio:** de generatie wordt daar afgerekend

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **dGEN Visual Studio**
2. Koppel je account via **Dashboard → Connectors**
3. Vraag GENI wat er in je studio klaarstaat

## Wat het kost

Twee saldo's, en dat is met opzet:

| Wat | Waar het van af gaat |
|---|---|
| Iets opvragen (flows, modellen, bibliotheek, saldo) | **5 credits** bij dGENIX |
| Iets laten maken (beeld, video, flow) | **25 credits** bij dGENIX |
| De generatie zelf | **Je studio-credits**, hetzelfde bedrag als wanneer je daar op Run drukt |

Alles wat iets maakt vraagt eerst om je bevestiging, met het bedrag erbij. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **GENI bouwt geen flows.** Hij leest en draait ze; het canvas blijft jouw werk
- **Video duurt minuten.** Je krijgt een bevestiging dat het loopt, het resultaat komt in
  je bibliotheek te staan
- **Modelnamen niet verzinnen.** Vraag eerst de catalogus op; een onbekend id weigert de studio
- **Geen studio-credits, geen beeld.** Bijkopen kan alleen in de studio zelf
- **Er wordt niets verwijderd.** De skill heeft geen recht om iets uit je bibliotheek te halen

## Problemen oplossen

**"Je dGEN Visual Studio is nog niet gekoppeld."** Kijk bij **Dashboard → Connectors** of de
connector op Verbonden staat. Trek je de toestemming in de studio in, dan stopt de koppeling
zonder waarschuwing.

**Er komt een id terug in plaats van een beeld.** De generatie loopt nog. Vraag er later naar
met dat id, of kijk in je bibliotheek.

**"De studio kon dit niet uitvoeren."** Dat is de melding van de studio zelf, meestal over een
model dat de meegestuurde invoer niet aanneemt. Vraag de catalogus op.

**De stijl klopt niet.** Noem je LoRA of gebruik een flow; los gevraagd beeld valt terug op het
standaardmodel van de studio.

## Veelgestelde vragen

**Wat is het verschil met AI Beeldgeneratie?**
Die maakt snel een los beeld op onze modellen en rekent dGENIX-credits. Deze skill werkt in
jouw studio-account, met jouw modellen, en rekent daar af.

**Kan GENI dit op een schema doen?**
Ja. Dat is de belangrijkste reden dat deze skill bestaat; zie
[Geplande taken](../handleiding/geplande-taken.md).

**Wat gebeurt er met wat hij maakt?**
Het komt op twee plekken te staan: in je studiobibliotheek, net als werk dat je zelf op het canvas maakt, en in je dGENIX-bestanden. Dat laatste maakt het bruikbaar in een volgende stap.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [dGEN Visual Studio koppelen](../connectors/dgen-visual-studio.md) · [AI Beeldgeneratie](ai-beeldgeneratie.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle skills](https://dgenix.nl/skills)
→ Over het product zelf: [dGEN Visual Studio](https://dgenvisual.com)

*dGENIX Docs, dGEN Visual Studio, bijgewerkt augustus 2026*
