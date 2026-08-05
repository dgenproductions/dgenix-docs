# Meal Planner

With the Meal Planner GENI puts together a weekly menu around your diet, household size and budget, and adds the shopping list to go with it.

Available from **Growth**. No connection needed.

## What can GENI do with it?

- **Generate a weekly menu** based on your preferences, diet, allergies, cuisine and budget
- **Build a shopping list** for that menu, grouped so you do not walk the aisles three times

GENI first checks your [memory](../functies/geheugen.md) for what it already
knows (diet, allergies, number of people) and only asks for what is missing. Set
that up once and you never have to repeat it.

## Example: what you ask, what you get

```
Make a weekly menu for 2 people, vegetarian, no nuts
```

> **Weekly menu , 2 people, vegetarian, nut-free**
>
> | Day | Dinner | Prep time |
> |---|---|---|
> | Mon | Lentil stew with roasted carrot | 35 min |
> | Tue | Shakshuka with feta | 25 min |
> | Wed | Pasta with roasted pepper and ricotta | 30 min |
> | Thu | Chickpea and spinach curry | 40 min |
> | Fri | Vegetable tart with salad | 45 min |
> | Sat | Gnocchi with sage butter and squash | 25 min |
> | Sun | Aubergine bake | 55 min |
>
> Two dishes share their base (pepper, onion), so you buy that in one go.
> Shall I add the shopping list?

And then:

```
Yes, shopping list please
```

> **Shopping , week 32**
>
> **Fruit & veg:** 3 peppers, 1 aubergine, 400 g spinach, 1 squash, 4 carrots,
> 2 onions, garlic, fresh sage
> **Dairy:** feta 200 g, ricotta 250 g, 6 eggs
> **Store cupboard:** 400 g lentils, 2 tins chickpeas, pasta 500 g, gnocchi 500 g
>
> Flour, olive oil and spices are not listed, you usually have those in.

## Requirements

- **Plan:** Growth and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **Meal Planner**
2. Tell it once what your diet, allergies and household size are
3. Ask for a weekly menu

## What it costs

| Action | Credits |
|---|---|
| Generate a weekly menu | 15 |
| Build a shopping list | 8 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **GENI orders nothing.** You get a list; the shopping stays yours.
- **Prices are estimates.** It does not know the current shelf price at your supermarket.
- **Food safety is not medical advice.** With an allergy or a medical diet, check the labels yourself.
- **It does not know what you already have** unless you say so. Mention it and it takes that into account.
- **Menus are weekly.** A month in one go becomes unmanageably long.

## Troubleshooting

**The menu ignores my allergy.** Put the allergy in your [memory](../functies/geheugen.md) rather than in a single message, so it applies every time.

**The portions are off.** State the number of people explicitly, and whether children are eating along.

**Too many separate ingredients.** Ask for a menu that shares ingredients, or cap the number of products.

**Too expensive.** Give it a weekly budget and it steers towards cheaper base ingredients.

## Frequently asked questions

**Can I combine dietary requirements?**
Yes. Vegetarian plus gluten-free plus a budget in one request works fine.

**Can it take last week into account?**
If you ask. Say "no pasta again" or ask for variation against last week.

**Can I get this weekly on a schedule?**
Yes, through [Scheduled tasks](../handleiding/geplande-taken.md), for example a
menu and list every Saturday morning.

**Do I get recipes too?**
You get dishes with prep times. Ask about one dish for the full method.

---

Back to [Skills marketplace](README.md)
See also: [Smart Shopping](shopping.md) · [Memory](../functies/geheugen.md) · [Scheduled tasks](../handleiding/geplande-taken.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, Meal Planner, updated August 2026*
