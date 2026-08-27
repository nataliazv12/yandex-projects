# Bank Customer Churn — Segmentation Analysis

**Business question:** Which customer segments are most at risk of churning, and what are their defining characteristics?

**Client:** Regional bank "Metanprom" (anonymized dataset, 10k+ records)

## Tools

`Python` · `pandas` · `scipy` · `matplotlib` · `seaborn` · `plotly` · `Tableau`

## Approach

1. Exploratory data analysis across 12 customer attributes (demographics, financial behavior, product usage)
2. Statistical comparison of churn vs. retained customers
3. Segmentation by 2–3 combined features with highest churn lift

## Key Findings

- **Overall churn rate:** concentrated in specific behavioral and demographic intersections
- Male clients churn more than female across all branches
- Highest churn: Yaroslavl branch; lowest: Rybinsk
- Customers with 3+ products and high credit scores (830–900) show elevated churn risk
- Two age groups stand out: **25–35** and **50–60**

## Identified Churn Segments

**Segment 1 — High-Score Active Clients Without Credit Cards**
- Credit score 830–900 + no credit card + active usage → high churn risk despite engagement

**Segment 2 — Older Male Property Owners**
- Age 50+ + male + property score > 3 → lifecycle transition churn

**Segment 3 — Young High-Scorers With Cards**
- Age 25–35 + credit score 830–900 + credit card + active → competitive offer churn

## Deliverables

- [Tableau Dashboard](https://public.tableau.com/app/profile/natalia.zvereva/viz/_16938672598280/sheet1)
- [Executive Presentation](https://docs.google.com/presentation/d/1W4GetguhFQclC6S0341AQju2JuNPbk0lrixbSwGb2Ps/edit?usp=sharing)
- `Bank Customer Churn.ipynb` — full analysis notebook
