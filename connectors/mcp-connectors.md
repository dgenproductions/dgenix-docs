# MCP-connectors

MCP-connectors koppelen je AI-assistent aan externe tools via **Model Context Protocol (MCP)** — een open standaard waarmee dGENIX kant-en-klare connectors uit het groeiende MCP-ecosysteem kan aansluiten. Voor jou werkt zo'n connector precies als een gewone skill: je activeert hem in de marketplace, koppelt je eigen account, en je assistent gebruikt de bijbehorende tools automatisch.

---

## Hoe het werkt

1. Ga naar **Dashboard → Skills** en zoek de connector
2. Klik op **Activeren** (de connector verschijnt als gewone skill-toggle)
3. Volg de stap-voor-stap instructie die direct na activatie verschijnt
4. Koppel je eigen account via **Dashboard → Connectors** (alleen als de connector dat vereist)
5. Vraag je assistent om de connector te gebruiken

Elke MCP-connector heeft zijn eigen instructie in het dashboard, net als bij Gmail of WhatsApp. Je hoeft niets technisch te doen.

---

## Je eigen account

MCP-connectors draaien standaard op **jouw eigen account** bij de externe dienst. Je koppelt het met één klik (OAuth) of door je eigen API-sleutel in te voeren. Voordelen:

- Je houdt zelf de controle over je account en je data
- Eventuele kosten van de externe dienst lopen via jouw account, niet via dGENIX
- Verbreken kan altijd via **Connectors → Verbinding verbreken**

---

## Credits

MCP-connectors gebruiken hetzelfde creditsysteem als alle andere skills. Per connector staat een vaste creditprijs per actie. Dure acties vragen eerst om bevestiging ("dit kost X credits, doorgaan?") voordat ze uitgevoerd worden — dus je komt nooit voor verrassingen te staan.

---

## Verbinden: OAuth of API-sleutel

- **OAuth (één klik):** je logt in bij de dienst en geeft toestemming. De voorkeursmethode.
- **API-sleutel:** je plakt een sleutel uit je account van de externe dienst, net als bij WhatsApp Business of Stripe.
- **Geen koppeling:** sommige open connectors vereisen geen account — activeren is genoeg.

Welke methode van toepassing is, staat in de instructie van de connector zelf.

---

→ Terug naar [Connectors](README.md)
