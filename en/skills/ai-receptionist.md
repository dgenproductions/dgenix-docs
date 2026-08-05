# AI Receptionist

With the AI Receptionist you record your frequently asked questions once, after which GENI answers customer questions from them in the tone you set.

Available from **Pro**. No connection needed.

## What can GENI do with it?

- **Configure your FAQ** , company name, question-and-answer pairs, tone of voice and extra business information such as opening hours and address
- **Answer a customer question** from that FAQ
- **Summarise a customer conversation** with the action items pulled out

The difference with simply asking: it answers from **your** answers, not from
general knowledge.

## Example: what you ask, what you get

First configuring:

```
Set up my FAQ for De Krent Bakery, tone: friendly

Q: Are you open on Sundays?
A: Yes, from 8:00 to 13:00.

Q: Can I order a cake?
A: Yes, at least 3 days ahead, by phone or at the counter.
```

> FAQ configured for **De Krent Bakery**, 2 items, friendly tone.
> I do not have opening hours or an address yet; customers usually ask those
> first.

Then answering:

```
A customer asks: do you have gluten-free bread?
```

> Nothing in your FAQ covers that, so I am not inventing an answer.
>
> A suggestion if it is accurate:
> > "Yes, we have gluten-free bread daily. Availability is limited, so if you
> > order ahead we will set some aside for you."
>
> Shall I add it to your FAQ?

## Requirements

- **Plan:** Pro and up
- **Connection:** none

## Activating

1. Go to **Dashboard -> Skills** and activate **AI Receptionist**
2. Configure your FAQ with your frequently asked questions and tone
3. Ask a customer question to test it

## What it costs

| Action | Credits |
|---|---|
| Configure or update the FAQ | 5 |
| Answer a question | 3 |
| Summarise a conversation | 5 |

See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **It does not answer the phone.** There is no telephony connection; this is a text layer for you and your team.
- **It does not talk to customers itself.** There is no chat widget on your site; you paste the answer, or connect [WhatsApp Business](whatsapp-business.md).
- **Outside your FAQ it invents nothing.** That is deliberate: a guess aimed at a customer is worse than no answer.
- **No appointment booking.** Connect [Google Calendar](google-calendar.md) or [Calendly](calendly.md) for that.
- **Updating is yours.** If your opening hours change, you change the FAQ.

## Troubleshooting

**It says the answer is not there.** Correct, and that is the intent. Add the question to your FAQ.

**The tone is off.** Configure it again with a clear description, for example "short and businesslike" or "warm and informal".

**The FAQ does not parse.** Use the `Q:` and `A:` format with a blank line between items.

**Customers keep asking things that are not in it.** Analyse a week of questions and add the top five; that saves the most time.

## Frequently asked questions

**Can it answer on my website itself?**
No, there is no widget. You can have it read along on your business WhatsApp
through [WhatsApp Business](whatsapp-business.md).

**What is the difference with the Support Knowledge Base?**
[That one](knowledge-base.md) searches your whole documentation and names the
source. The AI Receptionist works from a short, manually configured FAQ with a
fixed tone.

**Can I configure several businesses?**
One FAQ at a time. If you work for several clients, use a
[project](../functies/projecten.md) per client.

**Can it summarise conversations from WhatsApp?**
Yes, paste the conversation and ask for a summary with action items.

---

Back to [Skills marketplace](README.md)
See also: [Support Knowledge Base](knowledge-base.md) · [WhatsApp Business](whatsapp-business.md) · [Projects](../functies/projecten.md)
On the site: [all skills](https://dgenix.com/skills)

*dGENIX Docs, AI Receptionist, updated August 2026*
