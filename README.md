# Global Cybersecurity Threats (2015–2024)

Python and Tableau analysis of a decade of simulated global cyberattack data: what drives financial loss, which industries and attack types carry the most risk, and how incidents group into risk profiles. Delivered as an executive Tableau storyboard for a healthcare C-suite audience.

**Live dashboard:** [Tableau Public storyboard](https://public.tableau.com/app/profile/ryan.wick4013/viz/Global_Cybersecurity_Threats_2015-2024_Final/GlobalCybersecurityThreats20152024) · **PDF export:** [Global Cybersecurity Threats (2015–2024).pdf](<05_Sent to Client/Global Cybersecurity Threats (2015–2024).pdf>)

**Skills demonstrated:** data cleaning, exploratory analysis, geospatial mapping, linear regression, K-means clustering, time-series stationarity testing, dashboard design, executive communication.

## Key Findings

- **Resolution time does not predict financial loss.** Linear regression (resolution time → loss) gave R² ≈ −0.0003; the correlation is about −0.01.
- **Affected-user count is not a reliable predictor of loss** either (near-zero correlation).
- **Government and Telecommunications show the highest median financial losses** in the exploratory analysis; the dashboard's average-loss chart ranks Government, IT, and Banking highest. Differences between industries are modest.
- **No defense mechanism clearly stands out.** Firewall and Antivirus show slightly lower median resolution times, but all five mechanisms overlap heavily.
- **K-means (k = 3) found three incident profiles:** moderate (~$53M loss, ~200K users), major (~$76M, ~707K users), and high exposure but low loss (~$22M, ~666K users). Financial loss separates the clusters more than resolution time does.
- **Annual losses plateau** at roughly $13–16B per year with no seasonality; the series is not stationary until differenced (Dickey-Fuller p = 0.095 before, 0.0006 after).

## Objective

Explore a large cybersecurity incident dataset, test common assumptions about what makes incidents costly, and present curated results to an executive audience through an interactive Tableau storyboard.

## Research Questions

1. How effective are different defense mechanisms in reducing resolution time or financial damage?
2. How many millions are lost per hour of incident resolution, and has this changed since 2015?
3. Are specific vulnerability types commonly exploited in high-impact attacks, and which result in the highest losses?
4. Which industries face the highest losses?

Working hypothesis tested with regression: *longer incident resolution times are associated with higher financial losses* (not supported by the data).

## Dataset

- **Source:** Kaggle, [Global Cybersecurity Threats 2015–2024](https://www.kaggle.com/datasets/victorsoeiro/global-cybersecurity-threats). The dataset is simulated, so findings illustrate method, not real-world incident rates.
- **Size:** 3,000 records, 10 variables: Country, Year, Attack Type, Target Industry, Financial Loss (in Million $), Number of Affected Users, Attack Source, Security Vulnerability Type, Defense Mechanism Used, Incident Resolution Time (in Hours).
- **Geography:** a countries GeoJSON file supports the choropleth map.

### Cleaning procedures

| Column | Change | Reason |
|---|---|---|
| Country | `UK` → `United Kingdom`, `USA` → `United States` | Standardize the only two abbreviated names |
| Financial Loss (in Million $) | Formatted as dollar values | Readability |
| Number of Affected Users | Added thousands separators | Readability |

No missing values or duplicate rows were found.

## Approach

| Notebook | What it does |
|---|---|
| 6.1 Clean and Understand | Profile the data, document cleaning, define research questions |
| 6.2 Exploratory Visual Analysis | Correlation matrix, scatterplots, pair plot, categorical plots; refine hypotheses |
| 6.3 Geographical Visualizations | Choropleth of average financial loss by country |
| 6.4 Supervised ML: Regression | Test whether resolution time predicts financial loss |
| 6.5 Unsupervised ML: Clustering | Elbow method, K-means with k = 3, cluster profiles |
| 6.6 Time Series | Annual loss trend, decomposition, Dickey-Fuller test, differencing, ACF |

## Screenshots

![Global financial loss by country](<04_Analysis/04.03_Visualizations/Global Financial Loss from Cybersecurity Incidents (2015-2024).png>)

![Clusters by resolution time and financial loss](<04_Analysis/04.03_Visualizations/Clusters by Resolution Time and Financial Loss.png>)

![Financial loss by target industry](<04_Analysis/04.03_Visualizations/Financial Loss by Target Industry.png>)

## Recommendations (from the dashboard)

- **Invest in proactive defenses** tailored to industry-specific threats.
- **Prioritize resolution speed**: fast handling does not always reduce cost, but builds long-term resilience.
- **Use cluster-based monitoring** to improve resource allocation and triage.

## Limitations

- The dataset is simulated; real incident data would behave differently.
- Self-reporting bias, estimated losses, and varying resolution-time definitions would affect real-world data.
- Findings are exploratory; the regression uses a single predictor.

## Tools

Python (pandas, matplotlib, seaborn, scikit-learn) · Jupyter Notebook · Tableau Public · GitHub

## Folder Structure

```
.
├── README.md
├── 01_Project Management/    (project brief, project documentation)
├── 02_Data/
│   ├── 02.01_Data Raw/       (original CSV, GeoJSON)
│   └── 02.02_Data Cleaned/   (first-pass cleaned CSV)
├── 03_Scripts/               (notebooks 6.1 to 6.6, choropleth HTML files)
├── 04_Analysis/
│   └── 04.03_Visualizations/ (exported charts)
└── 05_Sent to Client/        (PDF export of the Tableau storyboard)
```

## Author

Ryan Wick · [LinkedIn](https://www.linkedin.com/in/ryanwick-data-analyst/) · [Portfolio](https://sincere-dance-bac.notion.site/Ryan-Wick-242ccf8114f68059ba2ef00bd573f150)
