# A/B Test Analysis — Recommender System Test

**Business question:** Did the new recommendation system, rolled out via an improved payment funnel, actually lift conversion at each stage of the funnel (product page → cart → purchase)?

**Context:** A/B test ("recommender_system_test") run Dec 7, 2020 – Jan 4, 2021, targeting a 10%+ improvement in conversion rate at each funnel stage within 14 days of registration.

## Tools

`Python` · `pandas` · `numpy` · `scipy` (z-test, Bonferroni correction) · `matplotlib` · `seaborn` · `plotly`

## Approach

1. Data exploration and preprocessing across four source tables (events, marketing calendar, new users, test participants)
2. Test-design validation: group balance, sample overlap with other tests/marketing events, audience size vs. spec
3. Exploratory analysis of event volume, activity trends, and funnel conversion by group
4. Statistical evaluation of proportions (z-test with Bonferroni correction for multiple comparisons)
5. Conclusion and recommendations

## Key Findings

- The test **failed several validity checks**: data collection ran past the planned cutoff (through Dec 23 instead of Dec 21), included non-EU users, was missing the final 5 days of the intended window, overlapped with a "Christmas & New Year Promo" marketing campaign, and shared 25% of its users with a competing test.
- Group split was uneven (57% A / 43% B) rather than balanced.
- Purchase conversion was 23% in Group A vs. 9% in Group B — a large, statistically significant difference (z-test, Bonferroni-corrected) — but in the **opposite direction** of what a "successful" test would need, and not attributable to the recommender change alone given the design flaws above.

## Conclusion

Because of the test-execution issues (audience contamination, timeline overrun, uncontrolled marketing overlap, unbalanced groups), the results are **not reliable enough to attribute the observed difference to the new recommendation system**. The analysis recommends a clean re-run with stricter isolation, balanced group assignment, and full adherence to the planned test window.

## Deliverables

- `AB Test Analysis.ipynb` — full analysis notebook (data validation, EDA, statistical testing, conclusions)
