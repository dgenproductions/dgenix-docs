# Smart Shopping

With Smart Shopping GENI finds shops near you on the map, thinks along about what you need to buy and keeps your shopping list.

Available from **Growth**. No connection needed, the map data comes from dGENIX
itself.

## What can GENI do with it?

- **Look up shops on the map** , supermarkets, DIY stores, clothing shops or a specialist, with address, rating and opening hours
- **Work out the route to a shop**, with distance and travel time
- **Build and maintain shopping lists**, grouped by aisle
- **Think along about a purchase** , what to watch for, which size or variant you need, where it is usually sold

Only the first two fetch real data, and that is also where the credits sit.

## Example: what you ask, what you get

```
Where can I still get paint and brushes this evening in Eindhoven?
```

> Three DIY stores still open now:
>
> | Shop | Open until | Address |
> |---|---|---|
> | Example DIY North | 21:00 | Voorbeeldweg 12 |
> | Example Hardware | 20:00 | Voorbeeldlaan 340 |
> | Example Paint Specialist | 18:00 | Voorbeeldstraat 7 |
>
> The first is 9 minutes by car. If you are after wall paint: reckon on roughly
> 1 litre per 10 square metres per coat, so two 2.5 litre tins for an average
> room.

And for a list:

```
Add to my list: coffee, toilet paper, toothpaste, and something for Sunday evening
```

> **Shopping list**
>
> **Coffee & tea:** coffee beans
> **Household:** toilet paper, toothpaste
> **Sunday evening:** you had a bake last week, so I am adding salmon,
> potatoes and broccoli , 25 minutes of work.
>
> Say the word if you want something else for Sunday.

## Requirements

- **Plan:** Growth and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **Smart Shopping**
2. Say where you live, so you do not have to repeat it every time

## What it costs

| Action | Credits |
|---|---|
| Shopping list or buying advice without a map lookup | 3 |
| Look up shops on the map | 300 |
| Work out a route | 75 |

A map lookup is the expensive step. Keeping a list or asking for advice costs
almost nothing; only when you ask to "find shops nearby" is real data fetched.
See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI orders and buys nothing.** No web shops, no payments , you get the list and the shops.
- **There are no current prices or stock levels.** It does not know whether that product is on the shelf today.
- **Offers and leaflets are not included.**
- **Opening hours can be out of date**, especially around public holidays. Check them if you are driving somewhere specially.
- **The list lives in the conversation.** To really keep it, save it as a note in your [Workspace](../functies/werkruimte.md).

## Troubleshooting

**It finds no shops.** Name the town or the neighbourhood. Without a location it cannot look anything up on the map.

**It costs more credits than expected.** Every map lookup is 300 credits. Ask once, specifically, instead of three times, broadly.

**The list is gone the next day.** A conversation is not storage. Ask GENI to keep the list as a note.

**The opening hours were wrong.** That data sometimes lags behind the shop itself; call if in doubt.

## Frequently asked questions

**Do I need to connect Google Maps?**
No. The map data runs through dGENIX, you connect nothing.

**Can it compare prices between shops?**
Not with live prices. It can think along about where something is usually
cheaper and what to watch out for.

**Does this work with the Meal Planner?**
Yes, and that is the handiest combination: the
[Meal Planner](meal-planner.md) makes the menu and the list, Smart Shopping
finds the shop to go with it.

**Can I get a list automatically every week?**
Yes, through [Scheduled tasks](../handleiding/geplande-taken.md).

---

Back to [Skills marketplace](README.md)
See also: [Meal Planner](meal-planner.md) · [Travel Planner](travel.md) · [Workspace](../functies/werkruimte.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Smart Shopping, updated August 2026*
