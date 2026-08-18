# Aggregate data — State of the Community 2026

Aggregate results from the 2026 survey. **No row-level response data is published here**.

Every number in the published report can be checked against these files. `findings-figures.csv` says which file to check each one in.

## Files

| File | Contents | Rows |
|---|---|---|
| `findings-figures.csv` | Every figure cited in the report, with the file and lookup keys needed to check it | 341 |
| `aggregates/per-question-tallies.csv` | Response counts and percentages for every closed question and option | 566 |
| `aggregates/derived-variables.csv` | Distribution of every variable the report uses that is not a single survey question | 114 |
| `aggregates/ordinal-item-summary.csv` | Every 1–5 item: n, mean, share negative, share positive, top box, net | 54 |
| `aggregates/ordinal-items-by-segment.csv` | Every 1–5 item broken out by every segment group | 5,640 |
| `aggregates/net-sentiment-by-segment.csv` | Net sentiment on six measures by segment, with significance tests | 498 |
| `aggregates/community-issues-by-segment.csv` | Experience of seven kinds of community problem, by segment | 455 |
| `crosstabs/crosstabs.csv` | Seventeen key questions × every segment group, long format | 4,798 |
| `significance-register.csv` | All 499 statistically significant subgroup differences found across 1,374 tests | 499 |
| `free-written-responses.md` | Every free-written response from every respondent who granted full permission, verbatim | 850 |

## Checking a figure in the report

Start with `findings-figures.csv`. Each row carries the section or finding, the sentence or chart row the figure appears in, the file to look in, and the lookup keys. Most figures resolve to one of three places:

- a **share of all respondents** — `per-question-tallies.csv`, or `derived-variables.csv` if the base is derived
- a **share rating an item 4–5** ("important+", "agree+", "positive") — `ordinal-item-summary.csv` overall, `ordinal-items-by-segment.csv` by group
- a **share of one group giving one answer** — `crosstabs.csv`

A small number of figures in the findings come from a two-way cross of variables — for example, respondents who both stopped attending events *and* no longer consider themselves community members. The finding states the cross it is using, and both variables are published separately.

## Free-written responses

`free-written-responses.md` publishes all 850 free-written responses from the 280 respondents who granted full permission, grouped by question and reproduced exactly as written.

Responses are sorted alphabetically within each question, so the ordering differs from question to question and **answers cannot be linked to a single respondent across questions**. No respondent identifier or demographic attribute is attached to any response. In a community this size, a linked set of free-written answers would be identifying even without a name.

## Joining to the survey instrument

Every file carries a **`question_number`** column keyed to the question numbering in [`../SURVEY-INSTRUMENT.md`](../SURVEY-INSTRUMENT.md). Join on that rather than on question text to avoid issues where a question and a label are not byte-identical.

## Columns Reference

### `per-question-tallies.csv`

| Column | Meaning |
|---|---|
| `question_number` | The question in `SURVEY-INSTRUMENT.md` this column belongs to |
| `column_role` | `question` for the question's own column, `option` for one option of a multi-select, `matrix row` for one statement in a matrix |
| `export_column` | The column header as it appears in the survey platform's export |
| `response` | The answer given, or a parenthetical marker (see below) |
| `pct_of_431` | Percentage of all respondents |
| `pct_of_answered` | Percentage of those who answered that question. Blank for free-text and never-displayed rows |
| `note` | Routing faults and export artefacts affecting that column |

Three parenthetical markers appear in `response`:

- `(free text - not published)` — an open-ended question. The count is the number of people who wrote something; the text itself is published only in `free-written-responses.md`, and only for respondents who granted permission.
- `(never displayed - see note)` — the question was never shown to anyone because of a conditional logic fault. The `note` column names the fault. See `../LIMITATIONS.md` §5a.
- `(no respondent selected this option)` — the option was shown and nobody chose it. This is not a fault, and is marked differently from the row above so the two are not confused.

**Country is published grouped.** Countries answered by fewer than ten respondents are combined into a single row. Naming a country answered by a handful of people would be identifying in a sample this size. 43 countries are represented in total.

**Survey-platform metadata columns are excluded entirely** — entry id, source URL, user agent, IP address, submission timing. They are not survey questions and several are identifying.

### `derived-variables.csv`

Six of the report's segments are constructed rather than asked: work role, pay status, tenure (combined), event relationship, contribution type, and personal experience of community issues. This file publishes each one's distribution so that any figure computed on a derived base can be checked. `../METHODOLOGY.md` describes how each is built.

It also carries the **gate-consistent change-in-sentiment base** — the 333 respondents whose gate answer and direction answer agree, of whom 318 feel worse and 15 feel better — and the 23 responses excluded from it. See `../LIMITATIONS.md` §5b.

`used_in_significance_register` marks which variables are tested. Five views slice respondents by what they told us they feel rather than by who they are; testing those against the sentiment items would be close to circular, so they appear in the breakdown files only.

### `significance-register.csv`

`test_type` distinguishes ordinal comparisons (Kruskal–Wallis) from categorical ones (chi-square). `statistic` is H or χ² accordingly. `spread_in_group_means` is blank for categorical tests, which have no group means.

A variable is never tested against itself, and neither is a variable against one it is derived from.

## Reading the numbers

- Five-point scales are treated as **ordinal**. Means are given for readability; all significance testing is non-parametric.
- **Net score = percentage rating 4–5, minus percentage rating 1–2.** Neutral answers count toward the group's size but do not move the number.
- Ordinal comparisons use the **Kruskal–Wallis H test**; categorical comparisons use **chi-square**.
- **Subgroups with fewer than 15 respondents are excluded** from every comparison.
- **No multiple-comparison correction has been applied.** With 1,374 tests, roughly 69 of the 499 significant results would be expected by chance. Treat any single result close to p = .05 as suggestive rather than established. The large effects the report leans on — contribution type, contributor self-identification, participation level, event relationship, AI use, pay status, and the belonging-versus-money gap — clear p < .001 by wide margins.

The full register is published rather than only the results the report highlights, so that this judgment is available to everyone.

## Licence

Aggregate data in this directory is published under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See [`../../LICENSE.md`](../../LICENSE.md).

We ask, separately from the licence, that you **do not attempt to re-identify respondents**, including by combining these aggregates with other sources.
