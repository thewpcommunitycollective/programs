# Limitations of the State of the Community Survey 2026


## 1. The sample is representative of the WordPress open source project community, not WordPress users

Findings about the WordPress *community* and *contributor core* are well supported. This sample is heavily weighted toward long-tenured, professionally invested participants: **of the 364 respondents who gave a tenure answer, 70.6% have been in the community for a decade or more, and 22 have been there under two years.**

**Tenure is measured by two questions.** Current community members were asked how long they *have been* part of the community; respondents who once considered themselves members and no longer do were asked how long they *were*. Both use the same six answer options and we combine them. The 67 respondents who have never considered themselves members were not asked. Anyone reanalysing this data should combine both questions. 

Findings about the WordPress software's broader user base are not available from this instrument, and it should not be described as such by us or by anyone citing it.

## 2. Self-selection during a period of public conflict

A community survey fielded while that community is being affected by public conflict will attract engaged respondents on all sides. We cannot rule this out.

However, response patterns vary sensibly across items and do not show uniform negativity: the same respondents reporting the most negative WordPress sentiment also report +78 net positivity toward open source and 95.1% agreement that Security in WordPress matters.

## 3. The "AI in WordPress" importance item is bimodal

**Do not quote this item on its own.**

Of the 55 respondents who rated "AI in WordPress" *very important*, **13 are negative or very negative about AI in WordPress**, 11 of them *very* negative. They rated "AI in WordPress" as important because they consider it an important **problem**.

Two respondents identified this flaw independently in their comments. The more accurate measure of attitude toward AI in WordPress is the separate AI sentiment item, _net −33_, not the importance item.

**This item is being rewritten for 2027.**

## 4. No correction has been applied for multiple comparisons

The published significance register contains **499 statistically significant subgroup differences, found across 1,374 tests — 916 ordinal comparisons and 458 categorical ones. With that many tests, roughly 69 of the 499 would be expected by chance alone.**

Treat any single result close to p = .05 as suggestive rather than established. The large effects the report leans on — contribution type and contributor self-identification, participation level, event relationship, AI use, pay status, and the belonging-versus-money gap — clear p < .001 by wide margins and survive any reasonable correction.

We publish the full register rather than only the results the report highlights, so that this judgment is available to readers rather than made silently on their behalf.

## 5. Instrument and data faults

### 5a. Questions that returned no data

| Item | Status |
|---|---|
| "Have you personally experienced any of the following when contributing to the WordPress community?" and all seven of its options plus its free-text follow-up | **Entirely empty.** Conditional routing failure. Primary question erroneously set as conditional. Not displayed for any respondent. |
| "What made you uncomfortable asking for help?" and follow-up question "What else made you uncomfortable asking for help?" | **Empty.** Conditional routing failure. Secondary question. Condition set to empty. Not displayed for any respondent. |
| "Are you currently being paid for any of your time spent participating in the WordPress open source project?" | **Empty.** Conditional routing failure. Secondary question. Meant to distinguish current paid contributors from former paid contributors. Not displayed for any respondent. All pay-status analysis therefore uses the "have you ever been paid" item, which did collect data. |
| "Describe how you are using AI in your work" | **Empty.** Layout issue. Free-write text option to expand on the "Other" answer for "How are you using AI in your work" appeared above the primary question. |

### 5b. Data irregularities

**The sentiment-change question leaked.** 333 respondents answered "yes, my sentiment toward WordPress changed," but 356 supplied a direction of change — 23 people gave a direction after indicating no change. This is a conditional routing gap.

**All published figures use the gate-consistent base**: the 333 respondents whose gate answer and direction answer agree. On that base, 318 (95.5%) feel more negatively and 15 (4.5%) more positively. We do not use the larger direction-item base of 356, because we cannot tell whether those 23 responses reflect a changed mind, a misread question, or a form error.

The parallel question about sentiment toward open source software shows **no leakage at all** — 139 gate answers, 139 directions. That is what makes the WordPress-versus-open-source comparison in Finding 01 a fair one: the two items are structurally identical and only one of them misbehaved.

**Three columns in the AI use-case question are unreliable.** One duplicates the "Internal / external communications" column; one mixes two separate options; one is labelled "Other" but is in fact the agentic site development option. All published figures are deduplicated and relabelled, and the affected columns are flagged in `data/aggregates/per-question-tallies.csv`.

### 5c. Question design faults

- **Accessibility, health and safety precautions, and destination-country safety were not offered as options with regard to event attendance.** This omission was raised unprompted in multiple respondents' free-written comments. Respondents also raised employer budget and permission, whether remote or hybrid attendance is offered, speaker compensation, codes of conduct, who will be present, and whether AI is promoted at the event. All become closed options in 2027.
- **Some questions were forced-response when they should not have been.** This was primarily a platform limitation: the conditional logic did not work per item within matrix modules.
- The gender question offered "Other" with a free-text follow-up that only one person used. That answer cannot be published without risking respondent identification.
- **Two "open source values" items exist in the instrument** — one in the project-aspects matrix and one in the open source matrix — with slightly different wording and different results (4.48 and 4.51 overall). Findings citing this concept use the open source matrix item. The duplication is removed for 2027.

## 6. Follow-up and free-response questions were gated on the answers before them

Throughout the survey, "please describe," "what other…" and "why…" questions were shown only to respondents who gave a particular answer to the question above them. This was intentional. It keeps the survey short and avoids asking people to explain a position they do not hold.

It also means that **for most free-response questions, the population who could answer is narrower than the population who had something to say** — and that we drew that boundary in advance, on the basis of a closed question. Where a closed question and the concept behind it do not line up perfectly, the gate inherits the mismatch and the free text inherits it in turn.

The clearest example is contributor identity. "Which forms of contribution describe your participation in the WordPress open source project?" was shown only to respondents who agreed with the statement "I consider myself to be a contributor to the WordPress open source project." **69 respondents reported doing contribution work elsewhere in the survey but did not agree with that statement, and so were never asked what they contribute.** The survey applied the same filter that Finding 06 is about. Nothing was lost from the closed data, but the qualitative record of what non-identifying contributors actually do does not exist for 2026.

Other gates with the same shape:

| Free-response question | Shown only to respondents who |
|---|---|
| "Why do you no longer consider yourself to be a member of the WordPress community?" | had said they once did and no longer do |
| "What is affecting your negative feelings about the future…?" | had rated the future negatively — no parallel question was asked of neutral or unsure respondents |
| "What other issues have you personally experienced or witnessed…?" | had selected at least one closed issue option |
| "What type of help have you sought or received…?" | had said they sought or received help |

This is a design tradeoff rather than an error, and one we now think was set too tight in places. For 2027 we intend to offer at least one ungated "anything else?" free-response per section rather than only at the end of the survey; open identity-linked follow-ups to everyone whose *behaviour* qualifies them rather than only those whose *self-description* does; and ask the negative-sentiment follow-up of neutral and positive respondents too, so the qualitative record is not systematically one-sided.

## 7. Questions we did not ask

Two gaps became apparent only during analysis, and both limit findings in this report:

- **We did not ask respondents who currently attend events occasionally whether they used to attend more often.** Finding 10 can therefore describe the group who stopped entirely, but cannot say whether the contraction runs deeper than that.
- **We did not ask respondents who stopped attending whether they would attend a local event if one existed.** Respondents raise the disappearance of local events unprompted, but the survey cannot test whether restoring them would bring people back.

## 8. Respondents describing their own motives

Several findings rest on respondents saying why they did something — why they stopped attending events, why they reduced their participation, what they weigh when deciding whether to take part. Self-reported attribution is evidence of what people believe about their own behaviour. It is not the same as measuring cause, and we do not treat it as such.

Where the report says respondents attribute an outcome to something, that is the claim being made. Where a causal reading would be tempting but the data cannot support it, the finding says so.

## 9. Group sizes

Non-binary respondents number 15, exactly at our minimum threshold for inclusion. This group is included in significance testing, but a group at the threshold cannot carry a finding on its own: it is reported as directional throughout, is never the sole basis for a claim, and is labelled as such wherever it appears in a chart or table. Excluding it entirely would change none of the conclusions in this report, but would be its own form of erasure.

Several country-level and role-level cells are similarly small and are not reported as groups at all.

## 10. What we deliberately did not publish

We did not publish row-level response data, nor any free-text responses from respondents who did not grant explicit and full permission. Fourteen respondents granted *partial* permission; because the instrument did not ask which comments they meant, none of their free text is published. We also did not publish free-written text that included unsubstantiated allegations.

---
---

*If you find a limitation we have not listed, please open an issue here.*
