# State of the Community Survey 2026 Methodology

## Fielding

The State of the Community Survey 2026 was open from **27 May to 17 July 2026**. Anyone who works with, builds on, contributes to, or cares about the WordPress open source project was invited to respond. It was distributed publicly and openly; there was no sampling frame.

The survey was **anonymous**. No email addresses or names were collected and no IP-based identities or account identifiers are used in analysis.

The survey was available in **English, Spanish, French, Japanese, Hindi and Portuguese**. Most respondents completed the survey in English, and in less than 20 minutes.

**431 people completed the 2026 survey**, across 231 items in seven sections: sentiment toward the project, participation and contribution, community experience, events, open source values, AI, and demographics.

The survey instrument design drew on GitHub's Open Source Survey and various wellbeing measurement instruments.

## Sample composition

| Dimension | Composition |
|---|---|
| Gender | 69.6% male · 18.6% female · 3.5% non-binary · 8.1% declined to state · one respondent selected "Other" |
| Age | 37.4% 35–44 · 31.3% 45–54 · 15.1% 55–64 · 9.0% 25–34 · 4.6% 65–74 · 2.6% declined |
| Location | 40.4% United States · 57.1% elsewhere · 2.6% declined. 43 countries in total |
| Tenure | Of the 364 respondents with a tenure answer: 70.6% ten or more years in the community · 6.0% under two years |
| Payment | 57.5% unpaid for their participation · 26.9% paid directly · 15.5% paid indirectly |

**This sample is not representative of WordPress users and must not be described as such.** It is heavily weighted toward long-tenured, professionally invested participants. See `LIMITATIONS.md`.

## Coding

- Five-point sentiment scales are coded `Very negative = 1 … Very positive = 5`.
- Five-point importance scales are coded `Not Important = 1, Somewhat unimportant = 2, Neutral = 3, Important = 4, Very Important = 5`.
- Five-point agreement scales are coded `Strongly disagree = 1 … Strongly agree = 5`.
- **Mean scores (e.g. 4.64, 2.43)** are the arithmetic mean of those 1–5 codes for the group cited.
- **Net score = percentage of a group rating 4–5, minus percentage rating 1–2.** Neutral answers count toward the group's size but do not move the number. Net scores run from +100 to −100. Differences between two net scores are expressed in points.
- **"Important+"** means the share rating an item 4 or 5.

### Tenure

Tenure is measured by two questions, not one. Respondents who currently consider themselves community members were asked how long they *have been* part of it. Respondents who once considered themselves members and no longer do were asked how long they *were*. Both offer the same six answer options, and **we combine them**. The 67 respondents who say they have never considered themselves community members were not asked and have no tenure value, giving a tenure base of 364.

Any reanalysis that uses only the present-tense question silently excludes everyone who has left the community, which biases every question about disengagement. See `LIMITATIONS.md` §1.

### Change in sentiment

Change in feeling toward WordPress is measured by a gate question ("has your sentiment changed?") followed by a direction question. The two items disagree for 23 respondents, who supplied a direction after indicating no change.

**All published figures use the gate-consistent base**: the 333 respondents (77.3%) whose gate answer and direction answer agree. Of those, 318 (95.5%) report feeling more negatively and 15 (4.5%) more positively — 73.8% and 3.5% of all respondents respectively. The parallel question about open source software shows no such leakage. See `LIMITATIONS.md` §5b.

### Segment variables

Every published breakdown uses one of seventeen segment variables: gender, age, location, work role, pay status, tenure (combined), participation level, participation change, event relationship, contribution type, contributor identity, community membership, AI use at work, contributing to open source elsewhere, volunteering outside WordPress and open source, whether income depends on WordPress, and whether the respondent personally experienced any of the community issues the survey listed.

Six of those are derived rather than asked directly — work role, pay status, tenure (combined), event relationship, contribution type, and personal experience of community issues. Their construction is described in this file. The rest are single survey items.

### Work-role segments

Derived from the multi-select work-type item: *Owner/Exec* = selected business owner or executive and not employee; *Employee only* = employee and neither owner nor freelancer; *Freelancer only* = freelancer and neither; plus *Employee+Freelance*, *Employee+Owner*, and *Other/Non-working* for the remainder.

### Contribution type

Derived from the work-type items rather than from self-description. Respondents are classed as doing *code / project work* if they report software or WordPress development work, and *community work* if they report community-directed or WordCamp work. The four resulting groups are **Community and code work**, **Code / project work only**, **Community work only**, and **No contribution work**. Finding 06 turns on the gap between this variable and the contributor self-identification item.

### Event relationship

The single official-events item, relabelled to five groups: *attend, multiple times a year*; *attend, annually or occasionally*; *stopped attending*; *never attended, would like to*; *never attended, not interested*. "Ever attended" in Finding 10 means the first three groups combined.

## Analysis

- Five-point scales are treated as **ordinal**, not interval. Means are reported for readability, but all significance testing is non-parametric.
- Group comparisons on ordinal outcomes use the **Kruskal–Wallis H test**. Comparisons on categorical or binary outcomes use **chi-square** tests of independence.
- **Subgroups with fewer than 15 respondents are excluded from comparisons.** Where such a group is shown at all — this applies to non-binary respondents, n=15 — it is labelled directional and excluded from inference.
- **1,374 subgroup tests were run** across seventeen segment variables: 916 ordinal comparisons and 458 categorical ones. **499 reached p < .05 and 270 reached p < .001.** A variable is never tested against itself, and platform metadata columns are excluded. The full register is published at `data/significance-register.csv`.
- The model reported in Finding 06 is a **logistic regression** predicting contributor self-identification among respondents who report doing contribution work, with code-based work, participation venue, pay status and participation level as predictors. It is descriptive, not causal.
- Finding 10 reports a second logistic regression, predicting who stopped attending events among everyone who ever attended, controlling for gender, pay status, tenure and current sentiment.

### Multiple comparisons

**No multiple-comparison correction has been applied.** With 1,374 tests, roughly 69 of the 499 significant results would be expected by chance alone at p < .05.

Any single result close to p = .05 should be treated as **suggestive rather than established**. The large effects the report leans on — the effect of contribution type on contributor self-identification, participation level, event relationship, AI use, pay status, and the belonging-versus-money gap — clear p < .001 by wide margins and survive any reasonable correction.

We publish the full register so that this judgment is available to readers rather than made silently on their behalf.

### Self-reported attribution

Several findings rest on respondents saying why they did something: why they stopped attending events, why they reduced their participation, what they weigh when deciding whether to take part. Self-reported attribution is evidence of what people believe about their own behaviour. It is not a measurement of cause, and the report does not treat it as one.

## Quotations

Quotations in the published report are drawn **exclusively from the 280 respondents (65.0%) who explicitly granted permission to publish their free-written comments**. A further 14 respondents granted partial permission and are excluded from publication entirely, along with the 131 who declined. Comments implying legal culpability or unsubstantiated allegation were also excluded.

Quotes are reproduced **exactly as written**: spelling, punctuation, capitalization, emphasis and profanity are the respondents'. Trims within a longer response are marked `[…]`. No demographic or role attributes are attached to any quotation in the report.

## Reproducibility

Every figure in the published report can be checked against the aggregate data in `data/`. `data/findings-figures.csv` lists each figure the report cites, the sentence or chart row it appears in, and the file and lookup keys needed to verify it. `data/README.md` describes each file.

No row-level response data is published. Country is published grouped, and survey-platform metadata columns — entry id, source URL, user agent, IP address, submission timing — are excluded from every file.

Please open an issue for any concerns, questions, or comments.
