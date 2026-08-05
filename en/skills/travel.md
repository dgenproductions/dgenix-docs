# Travel Planner

With the Travel Planner GENI helps you plan a trip: it looks up real places on the map, works out routes and turns that into a day-by-day programme.

Available from **Growth**. No connection needed, the map data comes from dGENIX
itself.

## What can GENI do with it?

- **Look up places on the map** , hotels, restaurants, museums, beaches and attractions at your destination, with rating, address and opening hours
- **Work out a route** between two points, with distance and travel time
- **Build a day programme** that accounts for what sits where
- **Think along about the trip itself** , when to go, what to arrange before departure, how to split the days

The first two fetch real data. The rest comes from what GENI knows, and that
matters for your credits (see below).

## Example: what you ask, what you get

```
We are going to Porto for 4 days in October, what should we see?
```

> **Porto , 4 days in October**
>
> October is a good month: around 20 degrees, far quieter than summer.
>
> **Day 1 , Ribeira and the river**
> - Livraria Lello (book ahead, or you queue for an hour)
> - Cross Ponte Luís I on foot at sunset
>
> **Day 2 , Vila Nova de Gaia**
> - Port cellars across the river, two is plenty
> - Teleférico back up, saves a steep climb
>
> **Day 3 , Bolhão and Cedofeita**
> - Mercado do Bolhão in the morning
> - Rua de Miguel Bombarda for galleries
>
> **Day 4 , the coast**
> - Matosinhos, 20 minutes on the metro, seafood by the sea
>
> Shall I look up hotels in Ribeira or Cedofeita?

And if you say yes:

```
Yes, hotels in Cedofeita
```

> Three options within walking distance of Rua de Miguel Bombarda:
>
> | Name | Rating | Address |
> |---|---|---|
> | Example Hotel A | 4.5 (820 reviews) | R. de Cedofeita 120 |
> | Example Guesthouse B | 4.7 (310 reviews) | R. do Rosário 48 |
> | Example Hotel C | 4.2 (1,140 reviews) | Praça de Carlos Alberto 3 |
>
> From here it is a 14 minute walk to Ribeira.

## Requirements

- **Plan:** Growth and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **Travel Planner**
2. Say where you are going and for how long

## What it costs

| Action | Credits |
|---|---|
| Travel advice and day programme without a map lookup | 5 |
| Look up places on the map | 300 |
| Work out a route | 75 |

A map lookup is the expensive step, because real data sits behind it. So ask
specifically: "find three hotels in Cedofeita" is one lookup, "find hotels,
restaurants and museums" quickly becomes three. See
[The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI books nothing.** No flights, no hotels, no tickets , you get the options and book yourself.
- **There are no live prices or availability.** Map data gives place, rating and opening hours, not a room rate for your dates.
- **Flights are not included.** GENI can think along about routes and connections, but does not pull flight schedules.
- **Opening hours and ratings can be out of date.** Check them before you travel, especially around public holidays.
- **Travel documents and visas are not advice.** It can build a checklist; verify the official requirement with the authority.

## Troubleshooting

**It names places without addresses.** Then the answer comes from its knowledge, not the map. Ask explicitly to "look this up" for real data.

**It costs more credits than expected.** Every map lookup is 300 credits. Bundle your question: one search per category.

**The route does not match my transport.** Say so: on foot, by car or by public transport gives a different answer.

**A place turns out to be closed.** The data sometimes lags. Call or check the site before you go.

## Frequently asked questions

**Do I need to connect Google Maps?**
No. The map data runs through dGENIX, you connect nothing.

**Can it put my trip in my calendar?**
Yes, with [Google Calendar](google-calendar.md) connected. Ask it to schedule
the day programme as appointments.

**What is the difference with Smart Shopping?**
Both use the same map data. [Smart Shopping](shopping.md) targets shops and
groceries, Travel Planner targets trips.

**Can it remember my travel preferences?**
Yes, put them in your [memory](../functies/geheugen.md), for example that you
prefer not to fly or always want to stay central.

---

Back to [Skills marketplace](README.md)
See also: [Smart Shopping](shopping.md) · [Google Calendar](google-calendar.md) · [Memory](../functies/geheugen.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Travel Planner, updated August 2026*
