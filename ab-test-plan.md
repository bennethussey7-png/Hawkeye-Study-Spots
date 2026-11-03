# A/B Test Plan — Hawkeye Study Spots

## 1. Experiment Overview

This experiment will test whether changing the main headline on the Hawkeye Study Spots homepage increases visitors' interest in exploring the website's study-space listings.

The experiment will compare two versions of the homepage. The only content change between the versions is the main headline.

**Version A (Control):**
"Find a study spot that fits your day."

**Version B (Treatment):**
"Find your perfect study spot at the University of Iowa."

Version A: https://bennethussey7-png.github.io/Hawkeye-Study-Spots/

Version B: https://bennethussey7-png.github.io/Hawkeye-Study-Spots/home-b.html

## 2. Hypothesis and Justification

**Hypothesis:** A more specific, benefit-focused homepage headline that explicitly mentions the University of Iowa will increase the proportion of visitors who indicate they would click to explore study-space listings compared with the original, more general headline.

**Justification:** Students searching for a place to study want to quickly determine whether a website offers relevant information. The revised headline emphasizes finding a suitable study spot and identifies the University of Iowa, making the website's purpose more immediately clear. This may encourage visitors to explore the listings rather than leave the homepage.

## 3. AI Visitor and Testing Procedure

The experiment will use AI-simulated visitors rather than real website traffic.

Each AI visitor will act as a University of Iowa student looking for a quiet place to study on campus.

The same AI model and settings will be used for every trial. Each trial will begin in a fresh conversation with memory disabled to prevent earlier responses from influencing later decisions.

The only difference between conditions will be whether the AI visitor reviews Version A or Version B.

**Exact prompt:**

"You are a University of Iowa student looking for a quiet place to study on campus. Review the following website homepage: [VERSION URL]. Based on this page, would you click to explore the study-space listings? Answer Yes or No, followed by one sentence explaining your decision."

The appropriate Version A or Version B URL will replace the placeholder. Before beginning the experiment, I will confirm that the AI model can access both pages. If it cannot, I will use the full homepage text consistently for both conditions and document that method.

## 4. Random Assignment

Before collecting responses, I will generate a randomized trial sequence containing 50 Version A assignments and 50 Version B assignments.

The assignments will be shuffled and saved before testing begins. Trials will be conducted in that randomized order so the two versions are interleaved rather than tested in separate blocks.

## 5. Primary Outcome

The primary outcome will be whether the AI visitor indicates that they would click to explore the study-space listings.

Responses beginning with "Yes" will receive a score of 1. All other responses will receive a score of 0.

The main measurement will be the percentage of Yes responses in each condition.

This measures stated click intention, not actual website clicks.

## 6. Sample Size and Stopping Rule

The experiment will include 100 total AI visitor trials:

- 50 trials reviewing Version A
- 50 trials reviewing Version B

All 100 trials will be completed before evaluating the results. Data collection will not stop early based on the observed responses.

The experiment is planned to launch no later than November 17, 2026.

## 7. Analysis and Success Criteria

After completing all trials, I will calculate the Yes response rate for each version and the difference in percentage points between Version B and Version A.

I will use a two-sided Fisher's exact test to assess the difference between the two proportions, using a significance level of 0.05.

Version B will be considered successful if it produces a higher Yes response rate than Version A and the difference is statistically significant at p < 0.05.

If the difference is not statistically significant, I will report the observed results without claiming that the revised headline improved performance.

## 8. Data Collection and Documentation

I will maintain a spreadsheet or CSV containing:

- Trial number and randomized assignment
- Homepage version and URL
- AI model and testing date
- Complete AI response
- Binary outcome (1 or 0)
- Notes about any technical issues or deviations

The final report will include the experiment setup, results, statistical comparison, screenshots of both homepage versions, links to the live pages, and a discussion of limitations.

## 9. SEO Protection

Version B includes a `noindex` robots meta tag to discourage search engines from indexing the experimental homepage. Version B will not be added to the website's XML sitemap.

This helps prevent the experimental page from competing with the original homepage in search results.
