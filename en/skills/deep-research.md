# Deep Research

## What does this skill do?

Deep Research runs in-depth, multi-iteration research. You give one research topic, and your assistant splits it into 4 to 8 sub-questions, does a focused web search for each, and synthesises a final report with a TLDR, findings per theme and a numbered source list. Ideal for market, industry and competitor analysis without doing ten searches yourself.

## Requirements

- **Plan:** Growth+
- **Integrations:** none, the skill uses built-in web search

## How do you activate the skill?

1. Go to **Skills** in the dashboard
2. Find **Deep Research** and click **Activate**
3. Open the **Assistant** and click **Tools** at the bottom, choose **Deep Research**
4. Type your research question and press Enter

You can also trigger it via a suggestion like "In-depth market research" on the empty chat screen, or by starting your question with "Deep research ...", the assistant then picks the right model and skill automatically.

## What can you do with it?

### Market research
"Run in-depth market research into Dutch e-commerce platforms for SMBs in 2026, focus on pricing and feature set."

### Competitor analysis
"Make a competitor analysis with cited sources for [company] versus [competitor 1] and [competitor 2]."

### Trend report
"Research the key trends in generative AI for healthcare providers, with practical examples and sources."

### Due diligence
"Do background research on [partner or client], including recent activity, leadership and press."

## Output

Every Deep Research report contains:

- **TLDR**, a 3-sentence summary for management
- **Findings**, grouped per theme, with inline citations like `[1]` and `[2]`
- **Sources**, a numbered list with title + URL

No speculation without a source. Anything not from the sources is explicitly flagged as such.

## Credit cost

| Type | Sub-questions | Expected credits | Hard cap |
|---|---|---|---|
| Standard | 4 | ~3,500 cr | 4,500 cr |
| Deep | 8 | ~7,500 cr | 8,500 cr |

The skill uses the Sonnet model (more powerful and more expensive) because decomposition and synthesis with sources require more reasoning.

## Tips

- Be specific. "Trends in marketing" is too broad, "Trends in B2B SaaS marketing for SMBs in the Netherlands 2026" yields better sources.
- Add context with `focus` ("mainly B2B", "Dutch market", "open data only").
- Use **deep** only for large questions. For most questions **standard** is fast enough and half the price.
- Save reports in a project folder, Deep Research reports are valuable later as reference.
