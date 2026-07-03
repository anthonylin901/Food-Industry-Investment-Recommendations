# Food Industry Investment Recommendations

Is there still room to enter the food industry? This Power BI report analyzes 2024 sales data across 100 major U.S. food chains to answer that question — walking from market-wide landscape, down to a competitive deep-dive, and finally to a data-driven investment recommendation.

Originally built as coursework for Creating Effective Data Visualizations at the University of Leeds, then extended into a full portfolio project.


## 1. Overview — Market Landscape

![PowerBI](images/Overview.png)

Sets the scene for the entire industry: **$263,406M** in total 2024 sales across 100 chains, but -8.99% YoY, signaling an industry in contraction. With a median chain size of just **$808M** against a long tail of much larger players, the market is confirmed as highly fragmented.


* Sales by Segment shows Quick Service dominating at **$193,350M** nearly 73% of total industry sales.
* Sales Distribution by Segment (box plot) shows Quick Service also has the widest spread, meaning it hosts both giants and small players.
* Market Concentration (Top 30) applies Pareto analysis: McDonald's alone captures ~15.4% of total sales, and even the top 30 chains combined don't reach the 80% mark — reinforcing just how fragmented this market really is.

## 2. "A Great Sandwich Chain Isn't Born, It's Breaded" — Competitive Deep-Dive

![PowerBI](images/Investment_Insight.png)

Zooms into the sandwich sub-segment to study competitive dynamics up close, using Firehouse Subs ($840M sales, +1% YoY vs. prior year) as the benchmark chain.


* Market Concentration (Pareto) shows Subway alone commands 33.8% of the sandwich segment, with the cumulative share crossing the 80% line by the 6th-ranked chain (Firehouse Subs).
* Sandwich Chain Distribution (pie) visualizes the same concentration: Subway 33.8%, Panera Bread 21.8%, Arby's 17.1%, with the remaining 8 chains splitting the rest.
* The Chain Rank table adds a growth lens: despite its dominant share, Subway is actually shrinking (Growth YoY: -0.19), while smaller players like Jersey Mike's are growing (+0.20) — share and growth tell two different stories.

## 3. "Is There Room for More in the Food Industry?" — Weighted Scoring Model (WSM)

![PowerBI](images/Market_Structure.png)

The centerpiece of the report: an interactive Weighted Scoring Model (WSM) — a Multi-Criteria Decision-Making (MCDM) method — that scores each segment on four dimensions: Revenue, Market Concentration, Unit Economics, and Growth.


* Live weight sliders (Power BI What-if parameters) let users set their own priorities across the four criteria, with a validator confirming the weights sum to 1.
* Under the default weighting (Concentration-heavy: 0.30 / 0.60 / 0.05 / 0.05), Quick Service ranks #1 with a score of 0.918, well ahead of Casual Dining (0.700), Fast Casual (0.602), Midscale (0.217), and Fine Dining (0.050).
* The WSM Score Breakdown shows exactly which criteria drive each segment's score, and the Competitive Concentration heatmap cross-references segment vs. cuisine to spot where competition is lightest.


> The ranking isn't fixed, it's designed to shift as priorities change, which is the point: "best segment to enter" depends on what an investor actually values.

# Key Techniques Used

* Exploratory Data Analysis (EDA) to understand market distribution and outliers 
* Descriptive statistics: median, concentration ratio, histogram binning
* Weighted Scoring Model (WSM / MCDM) with interactive weight sliders for dynamic segment ranking
* DAX measures for YoY growth, cumulative sales %, and dynamic KPI logic
* Pareto (80/20) analysis via calculated cumulative-share line

# Try It Yourself

Download **Food Industry Investment Recommendations.pbix** from this repo and open in Power BI Desktop.

Feedback welcome, especially from anyone in F&B, investment, or data analytics.