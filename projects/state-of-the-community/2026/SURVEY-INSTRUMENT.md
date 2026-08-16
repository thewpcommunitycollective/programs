#  State of the Community Survey 2026 - Survey Instrument

The complete instrument as fielded, reformatted for reading. **This file contains no response data.** Counts and percentages for every closed question are in [`data/aggregates/per-question-tallies.csv`](data/aggregates/per-question-tallies.csv).

Version 1.0 · fielded May 27 - July 17, 2026 · English, Spanish, French, Japanese, Hindi, Portuguese

**Provenance:** This is the authoritative instrument, generated from the platform export. Question order, option order, required flags and display conditions are all as fielded.

## Survey description shown to respondents

> The State of the Community Survey is an open survey from The WP Community Collective inviting anyone who works with, builds on, contributes to, or cares about WordPress to share how they are feeling about the community and its ecosystem. The survey covers topics including overall sentiment toward the WordPress open source project, community participation, open source sustainability, and the impact of AI. All responses are anonymous. The survey takes 10-15 minutes to complete.

---

## How to read this file

| | |
|---|---|
| **Question numbers** | Ours, applied in display order. Respondents did not see numbers. |
| `single` | One choice from a list |
| `multi` | Check all that apply |
| `scale` | One statement rated on a shared scale |
| `matrix` | Several statements, each rated on the same scale |
| `text` | Free text |
| **Required** | Marked on each question. The survey used forced-response validation on required items. |
| **Shown if …** | Display condition. Questions without this line were shown to everyone. |
| ⚠ | A display condition that cannot evaluate true as written — see the note at the end of this file. |

Option lists give the text respondents saw. The stored value is not shown here.

---

## Section 1: About You

### Q1. What is your age?

*Type: single* · *Required*

Options:

- Prefer not to answer
- 17 or younger
- 18-24
- 25-34
- 35-44
- 45-54
- 55-64
- 65-74
- 75 or older

### Q2. What is your gender?

*Type: single* · *Required*

Options:

- Prefer not to answer
- Male
- Female
- Non-binary
- Other

### Q3. Please indicate your gender identification:

*Type: text* · *Optional*

**Shown if Q2 = “Other”**

### Q4. What country do you primarily work from?

*Type: single* · *Required*

Options:

- Prefer not to answer
- Afghanistan
- Albania
- Algeria
- American Samoa
- Andorra
- Angola
- Anguilla
- Antarctica
- Antigua and Barbuda
- Argentina
- Armenia
- Aruba
- Australia
- Austria
- Azerbaijan
- Bahamas
- Bahrain
- Bangladesh
- Barbados
- Belarus
- Belgium
- Belize
- Benin
- Bermuda
- Bhutan
- Bolivia
- Bonaire, Sint Eustatius and Saba
- Bosnia and Herzegovina
- Botswana
- Bouvet Island
- Brazil
- British Indian Ocean Territory
- Brunei Darussalam
- Bulgaria
- Burkina Faso
- Burundi
- Cabo Verde
- Cambodia
- Cameroon
- Canada
- Cayman Islands
- Central African Republic
- Chad
- Chile
- China
- Christmas Island
- Cocos Islands
- Colombia
- Comoros
- Congo
- Congo, Democratic Republic of the
- Cook Islands
- Costa Rica
- Croatia
- Cuba
- Curaçao
- Cyprus
- Czechia
- Côte d'Ivoire
- Denmark
- Djibouti
- Dominica
- Dominican Republic
- Ecuador
- Egypt
- El Salvador
- Equatorial Guinea
- Eritrea
- Estonia
- Eswatini
- Ethiopia
- Falkland Islands
- Faroe Islands
- Fiji
- Finland
- France
- French Guiana
- French Polynesia
- French Southern Territories
- Gabon
- Gambia
- Georgia
- Germany
- Ghana
- Gibraltar
- Greece
- Greenland
- Grenada
- Guadeloupe
- Guam
- Guatemala
- Guernsey
- Guinea
- Guinea-Bissau
- Guyana
- Haiti
- Heard Island and McDonald Islands
- Holy See
- Honduras
- Hong Kong
- Hungary
- Iceland
- India
- Indonesia
- Iran
- Iraq
- Ireland
- Isle of Man
- Israel
- Italy
- Jamaica
- Japan
- Jersey
- Jordan
- Kazakhstan
- Kenya
- Kiribati
- Korea, Democratic People's Republic of
- Korea, Republic of
- Kuwait
- Kyrgyzstan
- Lao People's Democratic Republic
- Latvia
- Lebanon
- Lesotho
- Liberia
- Libya
- Liechtenstein
- Lithuania
- Luxembourg
- Macao
- Madagascar
- Malawi
- Malaysia
- Maldives
- Mali
- Malta
- Marshall Islands
- Martinique
- Mauritania
- Mauritius
- Mayotte
- Mexico
- Micronesia
- Moldova
- Monaco
- Mongolia
- Montenegro
- Montserrat
- Morocco
- Mozambique
- Myanmar
- Namibia
- Nauru
- Nepal
- Netherlands
- New Caledonia
- New Zealand
- Nicaragua
- Niger
- Nigeria
- Niue
- Norfolk Island
- North Macedonia
- Northern Mariana Islands
- Norway
- Oman
- Pakistan
- Palau
- Palestine, State of
- Panama
- Papua New Guinea
- Paraguay
- Peru
- Philippines
- Pitcairn
- Poland
- Portugal
- Puerto Rico
- Qatar
- Romania
- Russian Federation
- Rwanda
- Réunion
- Saint Barthélemy
- Saint Helena, Ascension and Tristan da Cunha
- Saint Kitts and Nevis
- Saint Lucia
- Saint Martin
- Saint Pierre and Miquelon
- Saint Vincent and the Grenadines
- Samoa
- San Marino
- Sao Tome and Principe
- Saudi Arabia
- Senegal
- Serbia
- Seychelles
- Sierra Leone
- Singapore
- Sint Maarten
- Slovakia
- Slovenia
- Solomon Islands
- Somalia
- South Africa
- South Georgia and the South Sandwich Islands
- South Sudan
- Spain
- Sri Lanka
- Sudan
- Suriname
- Svalbard and Jan Mayen
- Sweden
- Switzerland
- Syria Arab Republic
- Taiwan
- Tajikistan
- Tanzania, the United Republic of
- Thailand
- Timor-Leste
- Togo
- Tokelau
- Tonga
- Trinidad and Tobago
- Tunisia
- Turkmenistan
- Turks and Caicos Islands
- Tuvalu
- Türkiye
- US Minor Outlying Islands
- Uganda
- Ukraine
- United Arab Emirates
- United Kingdom
- United States
- Uruguay
- Uzbekistan
- Vanuatu
- Venezuela
- Viet Nam
- Virgin Islands, British
- Virgin Islands, U.S.
- Wallis and Futuna
- Western Sahara
- Yemen
- Zambia
- Zimbabwe
- Åland Islands

### Q5. Which best describes your current work type?

*Type: multi* · *Required*

Select all that apply.

Options:

- Employee
- Freelancer / Contractor
- Executive
- Business owner
- Non-working, looking for work
- Non-working, not looking for work
- Student
- Other

### Q6. What size is the company you work for?

*Type: single* · *Required*

**Shown if Q5 = “Employee” OR Q5 = “Executive”**

Options:

- 1-20 employees
- 20-50 employees
- 50-100 employees
- 100+ employees

### Q7. What size is your company?

*Type: single* · *Required*

**Shown if Q5 = “Business owner”**

Options:

- No employees (other than you)
- 1-10 employees
- 11-20 employees
- 21-50 employees
- 50+ employees

### Q8. Describe your work type:

*Type: text* · *Optional*

**Shown if Q5 = “Other”**

### Q9. Which of the following WordPress-related activities do you engage in?

*Type: multi* · *Required*

Please indicate both previous and/or current participation. Select all that apply.

Options:

- I use the WordPress open source software
- I follow updates and discussions about the WordPress open source project
- I participate in WordPress-related events
- I contribute to the software development of the WordPress open source
- I contribute to the community development of the WordPress open source project community development
- I generate income using the WordPress open source software
- I work for a company that operates in the WordPress ecosystem
- I use WordPress as part of my job or professional work, but my company is not directly involved in the WordPress ecosystem
- I use WordPress personally or for my own organization/project
- I do not currently participate in WordPress-related activities
- Other (please describe)

### Q10. Describe the WordPress-related activities you engage in:

*Type: text* · *Required*

**Shown if Q9 = “Other (please describe)”**

### Q11. Where do you participate in the WordPress open source project?

*Type: multi* · *Required*

Please indicate both previous and/or current participation. Select all that apply.

Options:

- Make WordPress (WordPress Slack)
- WordPress.org (forums, posts, etc.)
- Official WordPress events (WordCamps, etc.)
- WordPress-adjacent events (PressConf, WordSesh, etc.)
- Membership-based communities (Post Status, The Repository, etc.)
- Product-related communities
- WordPress communities on social media (Discord, Reddit, etc.)
- I do not participate in the WordPress open source project.
- Other (please describe)

### Q12. Describe where you participate in the WordPress open source project:

*Type: text* · *Required*

**Shown if Q11 = “Other (please describe)”**

### Q13. Which of the following describe the type of work you do with regard to the WordPress open source project?

*Type: multi* · *Required*

Please indicate both previous and/or current participation. Select all that apply.

Options:

- Building or developing with WordPress (sites, applications, etc.)
- Creating products to use with WordPress (plugins, themes, tools, etc.)
- Providing services to WordPress users or businesses
- Contributing to the WordPress open source project
- Contributing to the WordPress community
- Using WordPress personally or for your organization
- Working adjacent to WordPress (not directly building or using it)
- Not currently using WordPress
- Other (please describe)

### Q14. Describe your working situation with regard to the WordPress open source project.

*Type: text* · *Required*

**Shown if Q13 = “Other (please describe)”**

### Q15. Are you or have you ever been paid for any of your time spent participating in the WordPress open source project?

*Type: single* · *Required*

Options:

- Yes, directly - Some or all of my work duties include participating in WordPress
- Yes, indirectly - I participate in WordPress for work, but am not required to do so
- No - I am not paid for any of my participation in WordPress

### Q16. Are you currently being paid for any of your time spent participating in the WordPress open source project?

*Type: single* · *Required*

**Shown if Q15 = “Yes, directly - Some or all of my work duties include participating in WordPress” AND Q15 = “Yes, indirectly - I participate in WordPress for work, but am not required to do so”**

Options:

- Yes
- No

### Q17. Does the WordPress open source project affect your income?

*Type: single* · *Required*

Options:

- Yes
- Partially
- No
- Other

### Q18. How does the WordPress open source project affect your income?

*Type: text* · *Optional*

**Shown if Q17 = “Yes” OR Q17 = “Partially” OR Q17 = “Other”**

### Q19. I consider myself to be a contributor to the WordPress open source project.

*Type: scale* · *Required*

Scale: Strongly disagree · Disagree · Neutral · Agree · Strongly agree

### Q20. Which forms of contribution describe your participation in the WordPress open source project?

*Type: multi* · *Required*

Please indicate both previous and/or current participation. Select all that apply.

**Shown if Q19 = “Agree” OR Q19 = “Strongly agree”**

Options:

- Code/programming
- Documentation
- Maintenance (beta testing, reviewing contributions, reporting bugs, etc.)
- Training/education
- Translation
- Testing
- Standards (accessibility, web standards, etc.)
- Compliance (privacy, regulatory, etc.)
- Administrative/management (release leads, team reps, etc.)
- Community development (program development, mentorship, community care, etc.)
- Events (organizing events, volunteering at events, speaking at events, etc.)
- Marketing (content, communications, etc.)
- Sponsorship
- Project governance and policy
- Community participation
- Community leadership
- Unofficial WordPress events and groups
- Other

### Q21. What other form of contribution describes your participation in the WordPress open source project?

*Type: text* · *Required*

**Shown if Q20 = “Other”**

### Q22. I consider myself to be a member of the WordPress community.

*Type: scale* · *Required*

Scale: Strongly disagree · Disagree · Neutral · Agree · Strongly agree

### Q23. How long have you been part of the WordPress community?

*Type: single* · *Required*

**Shown if Q22 = “Agree” OR Q22 = “Strongly agree”**

Options:

- Less than 1 year
- 1-2 years
- 3-6 years
- 6-10 years
- 10-15 years
- 15+ years

### Q24. Have you ever considered yourself a member of the WordPress community?

*Type: single* · *Required*

**Shown if Q22 = “Strongly disagree” OR Q22 = “Disagree” OR Q22 = “Neutral”**

Options:

- Yes
- No

### Q25. How long were you a part of the WordPress community?

*Type: single* · *Required*

(Whatever that means to you!)

**Shown if Q24 = “Yes”**

Options:

- Less than 1 year
- 1-2 years
- 3-6 years
- 6-10 years
- 10-15 years
- 15+ years

### Q26. Why do you not consider yourself to be a member of the WordPress community?

*Type: text* · *Optional*

**Shown if Q24 = “No”**

### Q27. Why do you no longer consider yourself to be a member of the WordPress community?

*Type: text* · *Optional*

**Shown if Q24 = “Yes”**

## Section 2: Sentiment about the WordPress Open Source Project

### Q28. Right now, how do you feel overall about the WordPress open source project?

*Type: single* · *Required*

Options:

- Very positive
- Positive
- Neutral / Unsure
- Negative
- Very negative

### Q29. Has your sentiment toward the WordPress open source project changed over the past 24 months?

*Type: single* · *Required*

Options:

- Yes
- No

### Q30. How has your sentiment toward the WordPress open source project changed over the past 24 months?

*Type: single* · *Required*

**Shown if Q29 = “Yes”**

Options:

- I feel more positively about the WordPress open source project than I did 24 months ago
- I feel more negatively about the WordPress open source project than I did 24 months ago

### Q31. How do you feel about the future of the WordPress open source project?

*Type: single* · *Required*

Options:

- Very positive
- Positive
- Neutral / Unsure
- Negative
- Very negative

### Q32. What is supporting your positive feelings about the future of the WordPress open source project?

*Type: text* · *Optional*

**Shown if Q31 = “Very positive” OR Q31 = “Positive”**

### Q33. What is affecting your negative feelings about the future of the WordPress open source project?

*Type: text* · *Optional*

**Shown if Q31 = “Negative” OR Q31 = “Very negative”**

### Q34. How important are each of the following aspects of the WordPress open source project to you?

*Type: matrix* · *Required*

Statements:

- WordPress open source software
- The WordPress community
- WordPress events and meetups
- Contributing to WordPress
- Open source values
- AI in WordPress
- Security in WordPress
- Web standards and compliance
- WordPress leadership
- WordPress governance
- Business issues (mergers & acquisitions, product ecosystem, private equity investment, etc.)
- Enterprise/scale issues
- Collaboration with the greater open source ecosystem

Scale: Not Important · Somewhat unimportant · Neutral · Important · Very Important

### Q35. What other aspects of the WordPress open source project are important to you?

*Type: text* · *Optional*

## Section 3: Community Participation

### Q36. How would you describe your current level of community participation in the WordPress open source project?

*Type: single* · *Required*

Options:

- Very active participation
- Moderately active participation
- Occasional participation
- Observational only
- Inactive
- Do not participate / Not applicable

### Q37. Has your level of community participation in the WordPress open source project changed in the last 24 months?

*Type: single* · *Required*

Options:

- Significantly increased
- Increased
- No change / About the same
- Decreased
- Significantly decreased

### Q38. When deciding to participate in the WordPress open source project, how important are each of the following to you?

*Type: matrix* · *Required*

Statements:

- Personal capacity
- Financial incentives/restraints
- Impact of my contributions to the project
- Impact of my participation on my professional or personal life
- Understanding how to participate
- Mentorship or guidance
- Project roadmap
- Project leadership
- Project governance/policies
- Advocacy on behalf of web standards (accessibility, privacy, etc.)
- Participation in the WordPress community
- Feeling welcome/included
- Participating in a language other than English
- Working asynchronously

Scale: Not Important · Somewhat unimportant · Neutral · Important · Very Important

### Q39. What other factors are important to you when deciding how to participate in the WordPress open source project?

*Type: text* · *Optional*

### Q40. Have you ever sought or received help from others in the WordPress community related to participating or contributing?

*Type: multi* · *Required*

Select all that apply.

Options:

- I asked for help in a public forum (Slack, forums, GitHub, social media, etc.) and received a useful response
- I reached out directly to someone I know in the community and they helped me
- I found help through community documentation, guides, or onboarding resources
- I sought help, but did not receive a useful response
- I wanted help, but didn't feel comfortable asking
- I have not needed to seek this type of help
- Other (please describe)

### Q41. What type of help have you sought or received from others in the WordPress community related to participating or contributing?

*Type: text* · *Required*

**Shown if Q40 = “Other (please describe)”**

### Q42. What made you uncomfortable asking for help?

*Type: multi* · *Optional*

Select all that apply.

**Shown if Q40 = “I wanted help, but didn't feel comfortable asking.”** ⚠

Options:

- I didn't know who to ask
- I was concerned about how my question would be received
- I had experienced or witnessed negative interactions before
- I felt like an outsider or newcomer
- Other (please describe)

### Q43. What else made you uncomfortable asking for help?

*Type: text* · *Optional*

**Shown if Q42 = “Other (please describe)”**

### Q44. Have you personally experienced any of the following when contributing to the WordPress community?

*Type: multi* · *Required*

Select all that apply.

**Shown if Q46 [row: “Other (please describe)”] = *(empty)*** ⚠

Options:

- Lack of response to my contributions, questions, or requests for help
- Contributions or ideas rejected without explanation
- Dismissive or condescending responses to my contributions or questions
- Unclear, incomplete, or unwelcoming documentation or onboarding
- Difficulty finding where or how to get started
- I have not encountered any of the above
- Other (please describe)

### Q45. What issues have you personally encountered when contributing to the WordPress community?

*Type: text* · *Required*

**Shown if Q44 = “Other (please describe)”**

### Q46. Have you personally experienced or witnessed any of the following issues in the WordPress community?

*Type: matrix* · *Required*

Statements:

- Hostility or rudeness
- Dismissive or condescending responses to contributions or questions
- Name-calling or personal attacks
- Harassment or targeted negative behavior
- Conflict or ongoing interpersonal tension between community members
- Language or content that made me or others feel unwelcome or excluded
- Problems with project leadership or governance
- Other (please describe)

Scale: Myself · Others · Both myself and others · Have not experienced/witnessed

### Q47. What other issues have you personally experienced or witnessed in the WordPress community?

*Type: text* · *Required*

**Shown if Q46 [row: “Other (please describe)”] = “Myself” (row “Other (please describe)”) OR Q46 [row: “Other (please describe)”] = “Others” (row “Other (please describe)”) OR Q46 [row: “Other (please describe)”] = “Both myself and others” (row “Other (please describe)”)**

### Q48. As a result of experiencing any of the above, are any of the following true for you?

*Type: multi* · *Required*

Select all that apply.

**Shown if Q46 [row: “Hostility or rudeness”] = “Myself” (row “Hostility or rudeness”) OR Q46 [row: “Dismissive or condescending responses to contributions or questions”] = “Myself” (row “Dismissive or condescending responses to contributions or questions”) OR Q46 [row: “Name-calling or personal attacks”] = “Myself” (row “Name-calling or personal attacks”) OR Q46 [row: “Harassment or targeted negative behavior”] = “Myself” (row “Harassment or targeted negative behavior”) OR Q46 [row: “Conflict or ongoing interpersonal tension between community members”] = “Myself” (row “Conflict or ongoing interpersonal tension between community members”) OR Q46 [row: “Language or content that made me or others feel unwelcome or excluded”] = “Myself” (row “Language or content that made me or others feel unwelcome or excluded”) OR Q46 [row: “Problems with project leadership or governance”] = “Myself” (row “Problems with project leadership or governance”) OR Q46 [row: “Other (please describe)”] = “Myself” (row “Other (please describe)”) OR Q46 [row: “Hostility or rudeness”] = “Others” (row “Hostility or rudeness”) OR Q46 [row: “Dismissive or condescending responses to contributions or questions”] = “Others” (row “Dismissive or condescending responses to contributions or questions”) OR Q46 [row: “Name-calling or personal attacks”] = “Others” (row “Name-calling or personal attacks”) OR Q46 [row: “Harassment or targeted negative behavior”] = “Others” (row “Harassment or targeted negative behavior”) OR Q46 [row: “Conflict or ongoing interpersonal tension between community members”] = “Others” (row “Conflict or ongoing interpersonal tension between community members”) OR Q46 [row: “Language or content that made me or others feel unwelcome or excluded”] = “Others” (row “Language or content that made me or others feel unwelcome or excluded”) OR Q46 [row: “Problems with project leadership or governance”] = “Others” (row “Problems with project leadership or governance”) OR Q46 [row: “Other (please describe)”] = “Others” (row “Other (please describe)”) OR Q46 [row: “Hostility or rudeness”] = “Both myself and others” (row “Hostility or rudeness”) OR Q46 [row: “Dismissive or condescending responses to contributions or questions”] = “Both myself and others” (row “Dismissive or condescending responses to contributions or questions”) OR Q46 [row: “Name-calling or personal attacks”] = “Both myself and others” (row “Name-calling or personal attacks”) OR Q46 [row: “Harassment or targeted negative behavior”] = “Both myself and others” (row “Harassment or targeted negative behavior”) OR Q46 [row: “Conflict or ongoing interpersonal tension between community members”] = “Both myself and others” (row “Conflict or ongoing interpersonal tension between community members”) OR Q46 [row: “Language or content that made me or others feel unwelcome or excluded”] = “Both myself and others” (row “Language or content that made me or others feel unwelcome or excluded”) OR Q46 [row: “Problems with project leadership or governance”] = “Both myself and others” (row “Problems with project leadership or governance”) OR Q46 [row: “Other (please describe)”] = “Both myself and others” (row “Other (please describe)”)**

Options:

- I stopped contributing to a project or team
- I stepped back from community participation generally
- I moved my activity to other channels
- I did not change my participation, but it affected how I feel about my participation
- I filed a code of conduct report and it was resolved
- I filed a code of conduct report and it was not resolved
- It did not change my participation
- Other (please describe)

### Q49. How did your experience above affect how you participate in the WordPress community?

*Type: text* · *Required*

**Shown if Q48 = “Other (please describe)”**

## Section 4: Event Participation

### Q50. Attending in-person WordPress-related events is important to me.

*Type: scale* · *Required*

Scale: Strongly disagree · Disagree · Neutral · Agree · Strongly agree

### Q51. Which best describes your participation in official WordPress open source project events (such as WordCamps and Meetups)?

*Type: single* · *Required*

Options:

- I participate in WordPress events multiple times per year
- I participate in WordPress events annually or occasionally
- I used to participate in WordPress events, but I no longer do
- I have not attended any WordPress events, but I'd like to or am planning to
- I have not attended any WordPress events, and I'm not interested in attending
- Other (please describe)

### Q52. Describe your participation in official WordPress open source project events:

*Type: text* · *Optional*

**Shown if Q51 = “I participate in WordPress events multiple times per year” OR Q51 = “I participate in WordPress events annually or occasionally” OR Q51 = “I used to participate in WordPress events, but I no longer do”**

### Q53. Which best describes your participation in unofficial, WordPress-adjacent in-person events (such as PressConf or LoopConf)?

*Type: single* · *Required*

Options:

- I participate in WordPress-adjacent in-person events multiple times per year
- I participate in WordPress-adjacent in-person events annually or occasionally.
- I used to participate in WordPress-adjacent in-person events, but I no longer do
- I have not attended any WordPress-adjacent in-person events, but I'd like to or am planning to
- I have not attended any WordPress-adjacent in-person events, and I'm not interested in attending
- Other (please describe)

### Q54. Describe your participation in unofficial, WordPress-adjacent in-person events:

*Type: text* · *Optional*

**Shown if Q53 = “Other (please describe)”**

### Q55. Have you attended any other open source or tech-related in-person conferences or events in the past 24 months?

*Type: single* · *Required*

Options:

- Yes
- No

### Q56. What other open source or tech-related in-person conferences or events have you attended?

*Type: text* · *Optional*

**Shown if Q55 = “Yes”**

### Q57. When deciding to attend in-person conferences or events, how important are each of the following to you?

*Type: matrix* · *Required*

Statements:

- A location local to you
- A regional/destination location
- Events with smaller attendance
- Events with larger attendance
- Hard skill development (technical instruction, workshops, etc.)
- Soft skill development (business development, personal development, etc.)
- Topics of sessions / panels
- Particular speakers / keynotes
- Meeting professional development requirements
- Networking opportunities
- Community development/engagement
- Cost of ticket
- Cost of attendance (travel, housing, etc.)

Scale: Not Important · Somewhat unimportant · Neutral · Important · Very Important

### Q58. What else is important to you when deciding to attend in-person conferences or events?

*Type: text* · *Optional*

## Section 5: Open Source

### Q59. Right now, how do you generally feel about open source software?

*Type: single* · *Required*

Options:

- Very positive
- Positive
- Neutral / Unsure
- Negative
- Very negative

### Q60. Has your sentiment toward open source software changed over the past 24 months?

*Type: single* · *Required*

Options:

- Yes
- No

### Q61. How has your sentiment toward open source software changed over the past 24 months?

*Type: single* · *Required*

**Shown if Q60 = “Yes”**

Options:

- I feel more positively about open source software than I did 24 months ago
- I feel more negatively about open source software than I did 24 months ago

### Q62. How important are the following to you?

*Type: matrix* · *Required*

Statements:

- Open source software
- Open source values (whatever that means to you)
- The sustainability of open source projects
- Open source in WordPress
- Open source in AI

Scale: Not Important · Somewhat unimportant · Neutral · Important · Very Important

### Q63. Do you contribute to open source projects other than the WordPress open source project?

*Type: single* · *Required*

Options:

- Yes, regularly
- Yes, occasionally
- I'd like to in the future
- I used to, but have stopped
- No, and I don't plan to

### Q64. Do you contribute to or volunteer for organizations, projects or causes other than WordPress or open source projects?

*Type: single* · *Required*

Options:

- Yes, regularly
- Yes, occasionally
- I'd like to in the future
- I used to, but have stopped
- No, and I don't plan to

## Section 6: AI

### Q65. Are you currently using AI in your work?

*Type: single* · *Required*

Options:

- Yes
- No

### Q66. Describe how you are using AI in your work:

*Type: text* · *Optional*

**Shown if Q70 = “Other”**

### Q67. Right now, how do you generally feel about AI in the tech industry?

*Type: single* · *Required*

Options:

- Very positive
- Positive
- Neutral / Unsure
- Negative
- Very negative

### Q68. Right now, how do you generally feel about AI in WordPress?

*Type: single* · *Required*

Options:

- Very positive
- Positive
- Neutral / Unsure
- Negative
- Very negative

### Q69. Right now, how do you generally feel about AI in web development (vibe coding, agentic development, etc.)?

*Type: single* · *Required*

Options:

- Very positive
- Positive
- Neutral / Unsure
- Negative
- Very negative

### Q70. How are you currently using AI in your work?

*Type: multi* · *Required*

Select all that apply

**Shown if Q65 = “Yes”**

Options:

- Internal / external communications
- Writing / editing content
- Writing / reviewing code
- Design or image generation
- Research or learning
- Project management
- Bespoke plugin/theme development for clients
- Bespoke plugin/theme development for yourself/your work
- Commercial product development -- plugins or themes
- Agentic site management
- Agentic site development
- Other

### Q71. With regard to AI's current impact on your work or income, which of the following are true for you?

*Type: single* · *Required*

Options:

- AI has had a positive impact on my work or income
- AI has had a negative impact on my work or income
- AI has not significantly impacted my work or income
- Other (please describe)

### Q72. Describe how AI has impacted your income, job security, or client base:

*Type: text* · *Optional*

**Shown if Q71 = “AI has had a positive impact on my work or income.” OR Q71 = “AI has had a negative impact on my work or income.” OR Q71 = “Other (please describe)”** ⚠

### Q73. With regard to AI's future impact on your work or income, which of the following are true for you?

*Type: single* · *Required*

Options:

- AI will probably positively impact my work or income in the future
- AI will probably negatively impact my work or income in the future
- AI will probably not impact my work or income in the future
- Other (please describe)

### Q74. How do you think AI will impact your work or income in the future?

*Type: text* · *Optional*

**Shown if Q73 = “AI will probably positively impact my work or income in the future.” OR Q73 = “AI will probably negatively impact my work or income in the future.” OR Q73 = “Other (please describe)”** ⚠

## Section 7: Closing

### Q75. Is there anything else you'd like to share about how you're feeling about WordPress, the community, open source, or the greater tech industry?

*Type: text* · *Optional*

Optional.

### Q76. May we publicly cite and/or publish your free-written comments?

*Type: single* · *Required*

The WPCC will collect and summarize the free-written comments. We may also publicly cite or publish free-written comments. Please indicate if you permit all, some, or none of your free-written comments to be publicly cited and/or published. Even with permissions, we will make every effort to remove any possibly identifying details from any comments we share.

Options:

- My free-written comments may be publicly cited and/or published
- Some of my free-written comments may be publicly cited and/or published
- My free-written comments may not be publicly cited and/or published

### Q77. Which of your free-written comments may we cite and/or publish?

*Type: text* · *Required*

Optional.

**Shown if Q76 = “Some of my free-written comments may be publicly cited and/or published”**

---

## Routing faults

Further details available in [`LIMITATIONS.md`](LIMITATIONS.md). 

### Never displayed

The following questions were not displayed to respondents and returned zero responses.

**Q42. What made you uncomfortable asking for help?**

- Condition as written: Shown if Q40 = “I wanted help, but didn't feel comfortable asking.”
- Fault: **A trailing full stop in the rule value** that is not present in the option text (`…comfortable asking.` against the option `…comfortable asking`). The comparison is exact, so the rule did not fire.

**Q44. Have you personally experienced any of the following when contributing to the WordPress community?**

- Condition as written: Shown if Q46 [row: “Other (please describe)”] = *(empty)*
- Fault: **This question was not conditional**, and the incorrectly applied condition is tied to subsequent question.

