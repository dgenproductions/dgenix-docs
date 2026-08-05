# Workflow Builder

Met de Workflow Builder importeer je een bestaande n8n-workflow als JSON in dGENIX en laat je GENI hem uitvoeren, zonder dat je een eigen n8n-server nodig hebt.

Beschikbaar vanaf **Pro**. Pro bevat **3 import-slots**; meer slots koop je erbij.

## Wat kan GENI hiermee?

- **Een workflow importeren** vanaf n8n-JSON die je plakt of aanlevert
- **Een workflow uitvoeren**, met de parameters die je meegeeft
- **Je geïmporteerde workflows tonen**
- **Een workflow verwijderen** (en daarmee het slot vrijmaken)

Je bouwt de workflow dus elders (in n8n, of vanuit een template) en draait hem
hier.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Importeer deze workflow
[n8n JSON geplakt]
```

> **Geïmporteerd: Lead-verrijking**
>
> 6 stappen herkend:
> 1. Webhook , ontvangt bedrijfsnaam
> 2. HTTP , KvK-gegevens ophalen
> 3. Filter , alleen actieve inschrijvingen
> 4. HTTP , website ophalen
> 5. AI , bedrijfsomschrijving samenvatten
> 6. Google Sheets , regel toevoegen
>
> Je gebruikt nu **2 van je 3 slots**.
> Uitvoeren kost ongeveer 25 credits, afhankelijk van het aantal stappen.

En bij uitvoeren:

```
Draai de lead-verrijking voor "Voorbeeld BV"
```

> Klaar in 8 seconden. KvK-nummer gevonden, website opgehaald, samenvatting
> geschreven en als regel 47 in je sheet gezet.
>
> Eén stap gaf een waarschuwing: het handelsregister gaf twee inschrijvingen
> terug, ik heb de actieve gebruikt.

## Vereisten

- **Plan:** Pro en hoger
- **Koppeling:** hangt af van je workflow. Gebruikt hij Gmail of Sheets, dan moet die connector verbonden zijn

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **Workflow Builder**
2. Plak je n8n-JSON in de chat of importeer via het dashboard
3. Draai hem met "voer workflow X uit"

## Wat het kost

| Actie | Credits |
|---|---|
| Workflow importeren | 0 |
| Workflow uitvoeren | vanaf 25 |
| Workflows tonen | 3 |
| Workflow verwijderen | 0 |

De 25 credits zijn de basis; een workflow met veel stappen of AI-stappen kost
meer, omdat elke stap zijn eigen werk doet. Zie
[Het creditsysteem](../hoe-het-werkt/credits.md).

**Extra slots:** +1 voor € 6,99, +5 voor € 29,99, +10 voor € 59,99 per maand,
maandelijks opzegbaar.

## Grenzen en limieten

- **Niet elke n8n-node wordt ondersteund.** dGENIX voert de stappen zelf uit; nodes die een eigen n8n-omgeving vereisen doen het niet.
- **Geen visuele editor.** Je bouwt en wijzigt in n8n en importeert de JSON opnieuw.
- **Slots zijn per geïmporteerde workflow**, niet per uitvoering. Verwijder een oude om ruimte te maken.
- **Wijzig je de workflow in n8n, dan verandert hier niets.** Importeer hem opnieuw.
- **Credentials komen uit je dGENIX-connectors**, niet uit de JSON. Een workflow met een Gmail-stap werkt pas als Gmail gekoppeld is.

## Problemen oplossen

**"Import mislukt".** De JSON is onvolledig of komt uit een export van alleen een deel van de canvas. Exporteer de hele workflow.

**Een stap wordt overgeslagen.** Die node wordt niet ondersteund. Vraag welke stappen herkend zijn, dan zie je precies waar het misgaat.

**"Geen slots meer".** Verwijder een workflow die je niet meer gebruikt, of koop extra slots bij via **Account → Facturering**.

**De workflow draait maar doet niets.** Meestal ontbreekt de koppeling die een stap nodig heeft. Controleer je Connectors.

## Veelgestelde vragen

**Heb ik een eigen n8n-server nodig?**
Nee. Je gebruikt n8n alleen om te bouwen; het draaien gebeurt bij dGENIX.

**Wat is het verschil met Automations?**
[Automations](../functies/workflow-automations.md) zijn taken die GENI op een
tijdstip uitvoert. De Workflow Builder draait een geïmporteerde keten van
stappen. Je kunt ze combineren: een automation die je workflow start.

**Wat is het verschil met Eigen Workflows?**
[Eigen Workflows](custom-workflows.md) roept een webhook aan op jouw eigen
server. De Workflow Builder voert de stappen hier uit.

**Kan GENI zelf een workflow bouwen?**
Hij kan meedenken over de opzet, maar de JSON bouw je in n8n.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [Eigen Workflows](custom-workflows.md) · [Automations](../functies/workflow-automations.md) · [Geplande taken](../handleiding/geplande-taken.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [prijzen](https://dgenix.nl/pricing)

*dGENIX Docs, Workflow Builder, bijgewerkt augustus 2026*
