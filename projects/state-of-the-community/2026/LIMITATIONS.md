# Limitations of the State of the Community Survey 2026


## 1. The sample is representative of the WordPress open source project community, not WordPress users

Findings about the WordPress *community* and *contributor core* are well supported. This sample is heavily weighted toward long-tenured, professionally invested participants: **55.0% have been in the community for a decade or more.** Conversely, only six respondents have been around less than two years. 

Findings about the WordPress software's broader user base are not available from this instrument, and it should not be described as such by us or by anyone citing it.

## 2. Self-selection during a period of public conflict

A community survey fielded while that community is being affected by public conflict will attract engaged respondents on all sides. We cannot rule this out.

However, response patterns vary sensibly across items and do not show uniform negativity: the same respondents reporting the most negative WordPress sentiment also report +78 net positivity toward open source and 95.1% agreement that Security in WordPress matters.

## 3. The "AI in WordPress" importance item is bimodal

**Do not quote this item on its own.**

Of the 55 respondents who rated "AI in WordPress" *very important*, **13 are negative or very negative about AI in WordPress**, 11 of them *very* negative. They rated "AI in WordPress" as important because they consider it an important **problem**.

Two respondents identified this flaw independently in their comments. The more accurate measure of attitude toward AI in WordPress is the separate AI sentiment item, _net −33_, not the importance item.

**This item is being rewritten for 2027.**

## 4. Questions that returned no data

| Item | Status |
|---|---|
| "Have you personally experienced any of the following when contributing to the WordPress community?" and all seven of its options plus its free-text follow-up  | **Entirely empty.** Conditional routing failure. Primary question erroneously set as conditional. Not displayed for any respondent.|
| "What made you uncomfortable asking for help?" and followup question "What else made you uncomfortable asking for help?" | **Empty.** Conditional routing failure. Secondary question. Condition set to empty. Not displayed for any respondent. |
| "Are you currently being paid for any of your time spent participating in the WordPress open source project?" | **Empty.** Conditional routing failure. Secondary question. Meant to establish current paid contributors from former paid contributors. Not displayed for any respondent.|
| "Describe how you are using AI in your work" | **Empty.** Layout issue. Free-write text option to expand on "Other" answer for "How are you using AI in your work" appeared above the primary question. |

## 5. Data irregularities

- **333 respondents answered "yes, my sentiment changed" but 356 supplied a direction of change for their sentiment.** Conditional routing gap. All published figures use the direction item, which has the larger base: 331 negative, 25 positive.
- **Three columns in the AI use-case question are unreliable.** One duplicates the "Internal / external communications" column; one mixes two separate options; one is labelled "Other" but is in fact the agentic site development option. All published figures are deduplicated and relabelled, and the affected columns are flagged in data/aggregates/per-question-tallies.csv

## 6. Question design faults

- **Accessibility, health and safety precautions, and destination-country safety were not offered as options with regard to event attendance** This omission was raised unprompted in multiple respondents' free-written comments.
- **Some questions were forced-response when they should not have been.** This was primarily a platform limitation.
- The gender question offered "Other" with a free-text follow-up that only one person used. That answer cannot be published without risking respondent identification.

## 7. Group sizes

Non-binary respondents number 15, exactly at our minimum threshold for inclusion. This group is included in significance testing, but a group at the threshold cannot carry a finding on its own: it is reported as directional throughout, is never the sole basis for a claim, and is labelled as such wherever it appears in a chart or table. Excluding it entirely would change none of the conclusions — the gender effect on sentiment holds either way — but would be its own form of erasure.

Several country-level and role-level cells are similarly small and are not reported as groups at all.

## 8. What we deliberately did not publish

We did not publish row-level response data, nor any free-text responses from respondents who did not grant explicit and full permission. We also did not publish free-written text that included unsubstantiated allegations.

---

*If you find a limitation we have not listed, please open an issue here.*
