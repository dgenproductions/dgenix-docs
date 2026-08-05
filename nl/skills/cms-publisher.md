# CMS Publisher

Met de CMS Publisher zet GENI een artikel rechtstreeks in je WordPress of Webflow, standaard als concept zodat jij het laatste woord houdt.

Beschikbaar vanaf **Growth**. Je hebt een gekoppelde WordPress- of
Webflow-site nodig.

## Wat kan GENI hiermee?

- **Publiceren naar WordPress** , titel, inhoud, categorieën en tags, als concept of direct live
- **Publiceren naar Webflow** , een item in je CMS-collectie, als concept of gepubliceerd

Beide staan standaard op **concept**. Live zetten kan, maar dan moet je het
expliciet vragen.

## Voorbeeld: wat je vraagt, wat je terugkrijgt

```
Zet het artikel over onderhoudscontracten als concept op mijn WordPress
```

> **Concept aangemaakt , "Waarom een onderhoudscontract je meer oplevert dan het kost"**
>
> - 1.180 woorden, 6 tussenkoppen
> - Categorie: Onderhoud · Tags: contract, planning, kosten
> - Status: **concept**, dus nog niet zichtbaar voor bezoekers
>
> Bewerken en publiceren doe je hier:
> `jouwsite.nl/wp-admin/post.php?post=412&action=edit`
>
> Ik heb geen uitgelichte afbeelding gezet, die kies je zelf.

## Vereisten

- **Plan:** Growth en hoger
- **Koppeling:** WordPress (met een applicatiewachtwoord) of Webflow. Zie [Connectors](../connectors/README.md)

## Activeren

1. Ga naar **Dashboard → Skills** en activeer **CMS Publisher**
2. Koppel je WordPress- of Webflow-site via **Dashboard → Connectors**
3. Vraag GENI een artikel als concept te plaatsen

## Wat het kost

| Actie | Credits |
|---|---|
| Publiceren naar WordPress | 25 |
| Publiceren naar Webflow | 25 |

Het schrijven van het artikel kost apart; zie
[SEO Blog Schrijver](seo-blog.md) of
[Het creditsysteem](../hoe-het-werkt/credits.md).

## Grenzen en limieten

- **Alleen WordPress en Webflow.** De [Authority Engine](authority-engine.md) publiceert naar meer systemen; deze skill niet.
- **Concept is de standaard, en dat is opzet.** Direct live zetten kan, maar vraagt een expliciete opdracht.
- **Geen afbeeldingen.** Uitgelichte afbeeldingen en beeld in de tekst zet je zelf; genereren kan wel met [AI Beeldgeneratie](ai-beeldgeneratie.md).
- **Geen bestaande artikelen bijwerken.** Hij maakt een nieuw item aan.
- **Opmaak beperkt zich tot koppen, alinea's en lijsten.** Blokken, shortcodes en pagebuilder-elementen komen niet mee.
- **Webflow publiceert niet je site.** Een gepubliceerd item verschijnt pas na een site-publish in Webflow.

## Problemen oplossen

**"Geen toegang".** Bij WordPress is het applicatiewachtwoord verlopen of ingetrokken. Maak een nieuw aan en koppel opnieuw.

**Het artikel staat er zonder opmaak.** De inhoud kwam als platte tekst binnen. Vraag GENI om markdown-opmaak met koppen.

**Verkeerde collectie in Webflow.** Noem de collectie expliciet, of stel de standaard in bij de koppeling.

**Het item staat in Webflow maar is niet zichtbaar.** Publiceer je site in Webflow; een CMS-item alleen is niet genoeg.

## Veelgestelde vragen

**Wordt het direct live gezet?**
Nee, standaard niet. Je krijgt een concept en publiceert zelf, tenzij je
expliciet om live vraagt.

**Wat is het verschil met de Authority Engine?**
[Die](authority-engine.md) schrijft een hele contentstrategie en publiceert naar
acht systemen. De CMS Publisher is de losse stap "zet dit artikel erin".

**Kan ik dit inplannen?**
Ja, via [Geplande taken](../handleiding/geplande-taken.md), bijvoorbeeld elke
week een concept klaarzetten.

**Werkt het met WooCommerce?**
Voor blogartikelen wel, dat is gewoon WordPress. Producten aanmaken kan niet.

---

→ Terug naar [Skills marktplaats](README.md)
→ Zie ook: [SEO Blog Schrijver](seo-blog.md) · [Authority Engine](authority-engine.md) · [Connectors](../connectors/README.md)
→ Op de site: [alle skills](https://dgenix.nl/skills) · [alle koppelingen](https://dgenix.nl/integrations)

*dGENIX Docs, CMS Publisher, bijgewerkt augustus 2026*
