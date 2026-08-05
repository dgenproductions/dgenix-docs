# Typeform

With the Typeform skill GENI fetches the responses to your forms and summarises what comes out, so you do not have to scroll through a hundred answers yourself.

Available from **Growth**. You need a connected Typeform account.

## What can GENI do with Typeform?

- **List your forms**
- **Fetch recent responses** for a specific form
- **Analyse the responses** and produce a summary

That third one is the point. Reading individual answers takes time; pulling the
patterns out is the work that never gets done.

## Example: what you ask, what you get

```
What is coming out of our customer satisfaction form?
```

> **Customer satisfaction , 87 responses, last 30 days**
>
> **Average score:** 8.1 *(was 7.6 last period)*
>
> **Frequently mentioned in the positive**
> - Fast response to questions (34 times)
> - Thinking along when problems come up (21 times)
>
> **Frequently mentioned in the negative**
> - Reachability by phone (19 times)
> - Unclear lead times (11 times)
>
> **Worth noting:** the lead-time complaints come almost entirely from customers
> who ordered in June. That looks like a one-off, not structural.

## Requirements

- **Plan:** Growth and up
- **Connection:** a Typeform account via **Dashboard -> Connectors**

## Activating

1. Go to **Dashboard -> Skills** and activate **Typeform**
2. Go to **Dashboard -> Connectors** and click **Connect**
3. Ask for a form or for an analysis

## What it costs

Fetching forms and responses are light actions; an analysis costs more because
things are actually read and summarised. The amount shows on the button before
you start. See [The credit system](../hoe-het-werkt/credits.md).

## Limits

- **Read only.** GENI does not create or modify forms.
- **No deleting responses.**
- **Recent responses**, not your full history. For a yearly overview export from Typeform.
- **Personal data stays personal data.** What people enter in a form falls under the GDPR; handle it carefully.
- **The analysis is a summary, not statistics.** For significance and cross-sections use an analytics tool.

## Troubleshooting

**A form is missing.** Check that it belongs to the connected account; a colleague's forms fall outside.

**No responses come through.** The form has none yet, or they fall outside the fetched period.

**The summary misses what matters to you.** Say what to look for ("what do they say about price") and it focuses the analysis there.

**Open answers are summarised where you wanted quotes.** Ask explicitly for verbatim quotes.

## Frequently asked questions

**Can I run this monthly?**
Yes, and that is the best use: a summary every month instead of a form filling up
without anyone looking. See [Scheduled tasks](../handleiding/geplande-taken.md).

**Can it put the responses in a spreadsheet?**
With [Google Sheets](google-sheets.md) connected you can ask it to write the
results out.

**What is the difference with the Reputation Engine?**
[That one](reputation-engine.md) actively asks for Google reviews. Typeform is
about your own forms and stays inside your organisation.

**Does this work with a free Typeform account?**
Yes, within the response limits Typeform itself applies.

---

Back to [Skills marketplace](README.md)
See also: [Airtable](airtable.md) · [Google Sheets](google-sheets.md) · [Reputation Engine](reputation-engine.md)
On the site: [all skills](https://dgenix.com/skills) · [all integrations](https://dgenix.com/integrations)

*dGENIX Docs, Typeform, updated August 2026*
