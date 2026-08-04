# How it all fits together

dGENIX is made of five parts that build on each other: your assistant GENI, skills, connectors, credits and the channels you talk to it in. This page shows how they interlock.

Each part is explained on its own elsewhere in this documentation. Here it is
about the relationship, because that is exactly what people miss when something
does not work the way they expected.

## The layers, bottom to top

| Layer | What it does | Without this layer |
|---|---|---|
| **Connectors** | Grant access to your own accounts | GENI can reach nothing |
| **Skills** | Give GENI the ability to actually *do* something | Access without actions |
| **GENI** | Picks the right skill for your request | You would pick commands yourself |
| **Context** | Knowledge document, memory, knowledge base, projects | Every conversation starts from zero |
| **Credits** | Settle the work | , |

The key rule: **a skill and a connector are two different things.** The connector
decides whether GENI is *allowed* somewhere; the skill decides what it can *do*
there. That is the single most common source of confusion.

## Why skill and connector are separate

Say you switch on the Gmail skill but connect no Google account. GENI knows how
to read and write mail, but there is no mailbox. The other way round: connect
Google without switching on the skill and it has access but no actions.

That sounds roundabout and is not. You connect Google once and then decide per
skill what to switch on. And if you revoke the connection, every skill that
depends on it is out of play immediately , one button, no loose ends.

## What happens on a single request

You type:

```
Summarise my unread mail and put the action items in my calendar
```

Then this happens, in this order:

1. **GENI reads your context.** Knowledge document, relevant memories and, if you
   are inside a project, that project's context.
2. **It picks the skills.** This needs Gmail *and* Google Calendar. You do not
   have to name them.
3. **It checks access.** Is Google connected? If not, it says so rather than
   failing.
4. **It fetches the mail** and summarises.
5. **It proposes the calendar entries** and asks for confirmation, because that
   changes something.
6. **After your approval it executes** and deducts the credits.
7. **It remembers what matters**, for example that you like action items as
   separate calendar entries.

Step 5 is the pattern that runs through the whole platform: **reading is always
allowed, changing asks for approval.**

## What you see when something is missing

If the connection is missing you do not get an error but an explanation:

> I cannot read your inbox yet, because your Google account is not connected.
> Go to **Dashboard -> Connectors** and click Connect next to Gmail. After that
> I will pick this up right away.

## From one-off request to automatic

Anything you can ask by hand you can also schedule. A request that works in chat
works as a recurring task too: a daily overview every weekday at 08:00, a weekly
report every Monday.

How many recurring tasks you get depends on your plan: Starter 1, Growth 5,
Pro 10, Business 20. Execution is identical to a manual request, including the
confirmation on irreversible steps.

See [Scheduled tasks](../handleiding/geplande-taken.md).

## The Growth Tools sit on top

The five engines (SEO, GEO, Authority, Reputation and AI Content) are not
separate skills but heavier machines running on the same layers. They measure
something about your website or your reputation and deliver a report plus
concrete improvements.

What makes them special: GENI can combine them with ordinary skills. Running an
audit, putting the results in a document and emailing it is one request, not
three.

See [The five Growth Engines](../engines/README.md).

## The same assistant in every channel

Dashboard, Telegram and voice are three doors to the same assistant. Your
conversation history, your memory and your skills are identical everywhere. You
start a conversation on your laptop and finish it on your phone.

The dashboard is the only place where you configure: switching on skills,
connecting accounts, checking usage.

## Limits

- **No connector, no access.** There is no back door; GENI only goes where you
  let it in.
- **A skill does not work halfway.** If the connection is missing, GENI says so
  rather than delivering half a result.
- **Irreversible actions always ask for approval**, including inside a recurring
  task.
- **Credits go on execution**, not on thinking. If a paid action fails, they come
  back.
- **Projects share nothing with each other.** That is by design, but it means
  context does not carry over by itself.

## Frequently asked questions

**Do I have to say which skill it should use?**
No, GENI picks. If you want to steer it you can: *"use the Social Media Manager
to..."*.

**Why does a skill not work while it is switched on?**
Almost always because the matching connector is missing or expired. Check
**Dashboard -> Connectors** to see whether the account still shows as Connected.

**Can GENI combine several skills in one request?**
Yes, and that is the point. Reading mail, summarising, creating a calendar entry
and putting the result in a document can be a single sentence.

**What happens when my credits run out?**
Paid actions stop until your monthly balance refills or you top up. Topping up is
available from Starter; on Free there is a hard limit.

---

Next: [What is dGENIX](wat-is-dgenix.md) · [Context storage compared](context-opslag-vergeleken.md)
In depth: [Skills explained](../handleiding/skills-uitgelegd.md) · [Connectors](../connectors/README.md) · [The credit system](../hoe-het-werkt/credits.md)
On the site: [all skills](https://dgenix.com/skills) · [the five Growth Engines](https://dgenix.com/engines) · [pricing](https://dgenix.com/pricing)

*dGENIX Docs, How it all fits together, updated August 2026*
