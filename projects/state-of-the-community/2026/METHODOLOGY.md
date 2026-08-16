# State of the Community Survey 2026 Methodology

## Fielding

The State of the Community Survey 2026 was open from **27 May to 17 July 2026**. Anyone who works with, builds on, contributes to, or cares about the WordPress open source project was invited to respond. It was distributed publicly and openly; there was no sampling frame.

The survey was **anonymous**. No email addresses or names were collected and no IP-based identities or account identifiers are used in analysis.

The survey was available in **English, Spanish, French, Japanese, Hindi and Portuguese**. Most respondents completed the survey in English, and less than 20 minutes.

**431 people completed the 2026 survey**, across 231 items in seven sections: sentiment toward the project, participation and contribution, community experience, events, open source values, AI, and demographics.

The survey instrument design drew on GitHub's Open Source Survey and various wellbeing measurement instruments.

## Sample composition

The 2026 sample composition was as follows:

| Dimension | Composition |
|---|---|
| Gender | 69.6% male · 18.6% female · 3.5% non-binary · 8.1% declined to state |
| Age | 37.4% 35–44 · 31.3% 45–54 · 15.1% 55–64 · 9.0% 25–34 · 4.6% 65–74 · 2.6% declined |
| Location | 40.4% United States · 57.1% elsewhere · 2.6% declined |
| Tenure | 55.0% 10+ years in the community · 1.4% under two years |
| Payment | 57.5% unpaid for their participation · 26.9% paid directly · 15.5% paid indirectly |

**This sample is not representative of WordPress users and must not be described as such.** It is heavily weighted toward long-tenured, professionally invested participants. See `LIMITATIONS.md`.

## Coding

- Five-point sentiment scales are coded `Very negative = 1 … Very positive = 5`.
- Five-point importance scales are coded `Not Important = 1, Somewhat unimportant = 2, Neutral = 3, Important = 4, Very Important = 5`.
- Five-point agreement scales are coded `Strongly disagree = 1 … Strongly agree = 5`.
- **Net sentiment = percentage rating 4–5, minus percentage rating 1–2.**
- Work-role segments are derived from the multi-select work-type item: *Owner/Exec* = selected business owner or executive and not employee; *Employee only* = employee and neither owner nor freelancer; *Freelancer only* = freelancer and neither; plus *Employee+Freelance*, *Employee+Owner*, and *Other/Non-working* for the remainder.

## Analysis

- Five-point scales are treated as **ordinal**, not interval. Means are reported for readability, but all significance testing is non-parametric.
- Group comparisons on ordinal outcomes use the **Kruskal–Wallis H test**. Comparisons on categorical or binary outcomes use **chi-square** tests of independence.
- **Subgroups with fewer than 15 respondents are excluded from comparisons.** Where such a group is shown at all — this applies to non-binary respondents, n=15 — it is labelled directional and excluded from inference.
- 728 ordinal tests and 348 categorical tests were run. 282 ordinal tests reached p < .05; 126 reached p < .001. 
- The predictive model reported in the report (Finding 06) is **ordinary least squares on standardized predictors**, n=431, R² = 0.353. It is descriptive, not causal.

### Multiple comparisons

**No multiple-comparison correction has been applied.** With 728 tests, roughly 36 of the 282 significant results would be expected by chance alone at p < .05.

Any single result close to p = .05 should be treated as **suggestive rather than established**. The large effects — participation level, event relationship, AI use, pay status, and the gender findings on psychological safety — survive any reasonable correction, which is reflected in the report.

We publish the full register so that this data is available for further analysis.

## Quotations

Quotations in the published report are drawn **exclusively from the 280 respondents (65.0%) who explicitly granted permission to publish their free-written comments**. Free-write responses from people who declined full permission were excluded, as were comments that implied legal culpability or speculation.

Quotes are reproduced **exactly as written**: spelling, punctuation, capitalization, emphasis, implications, and profanity are the respondents'. Trims within a longer response are marked `[…]`. Attributions use only demographic and role attributes the respondent themselves supplied.

## Reproducibility

All of the findings in the published report are computed from the aggregate data represented available in `data/`. 

Please open an issue for any concerns, questions, or comments.
