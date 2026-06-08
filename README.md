# 🔐 Global Cybersecurity Threats (2015–2024)

An advanced analytics project analyzing global cybersecurity incidents to surface hidden patterns in financial loss, attack behavior, and organizational response — delivered as an executive dashboard for a healthcare audience.

---

## 📊 Tableau Storyboard

👉 [**View the Executive Dashboard**](https://public.tableau.com/app/profile/ryan.wick4013/viz/Global_Cybersecurity_Threats_2015-2024_Final/GlobalCybersecurityThreats20152024?publish=yes)

> The storyboard presents final insights only. Intermediate analysis steps are documented in the notebooks.

---

## 🎯 Objective

Explore large-scale cybersecurity threat data and deliver actionable insights via an executive-friendly dashboard highlighting trends, clusters, and strategic recommendations for healthcare organizations.

---

## 📌 Key Findings

- **Finance and healthcare** report the highest average financial losses across industries.
- **Proactive defense mechanisms** correlate with faster incident resolution times.
- **No strong linear relationship** exists between resolution time and financial loss.
- **User exposure** is an unreliable predictor of financial damage.
- **Cluster analysis** reveals distinct risk profiles — enabling tailored response strategies.

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Data Analysis | Python (pandas, matplotlib, seaborn) |
| Machine Learning | scikit-learn (K-Means, Regression) |
| Visualization | Tableau Public |
| IDE | Jupyter Notebook |
| Version Control | GitHub |

---

## 📊 Visualizations

Created in Tableau for a C-suite healthcare audience:

- Avg. Financial Loss by Industry (Bar Chart)
- Defense Mechanism vs Resolution Time (Box Plot)
- Resolution Time vs Financial Loss (Scatterplot)
- Global Trends Over Time (Line Chart)
- Incident Map by Country (Choropleth)
- Cluster Comparisons: Financial Loss, Resolution Time, and User Exposure

---

## 📁 File Structure

Global-Cybersecurity-Threats-Dashboard/
├── 01_Project_Management/
│   └── Project_Brief.pdf
├── 02_Data/
│   ├── raw/
│   │   ├── countries.geojson.json
│   │   └── Global_Cybersecurity_Threats_2015-2024.csv
│   └── cleaned/
│       └── Global_Cybersecurity_Threats_2015-2024-Cleaned.csv
├── 03_Scripts/
│   ├── 01_Clean_and_Explore.ipynb
│   ├── 02_Exploratory_Visual_Analysis.ipynb
│   ├── 03_Geographical_Visualizations.ipynb
│   ├── 04_Supervised_ML_Regression.ipynb
│   ├── 05_Unsupervised_ML_Clustering.ipynb
│   ├── 06_Time_Series_Analysis.ipynb
│   └── choropleth_avg_financial_loss.html
├── 04_Analysis/
│   ├── Reports/
│   └── Visualizations/
├── 05_Deliverables/
│   └── Global_Cybersecurity_Threats_Executive_Report.pdf
└── README.md

---

## 🧪 Data Sources & Ethics

- [Kaggle: Global Cybersecurity Threats Dataset (2015–2024)](https://www.kaggle.com/datasets/victorsoeiro/global-cybersecurity-threats)

Caveats:
- Data may reflect **self-reporting bias**
- Financial loss values may be **estimated or incomplete**
- Resolution times vary significantly across organizations
- No private or sensitive data was used

---

## ✅ Recommendations

- **Invest in proactive defenses** (e.g., intrusion detection) to reduce average response time.
- **Use cluster-based risk profiles** to drive strategic planning and resource allocation.
- **Don't assume faster resolution = less financial loss** — investigate contextual factors before acting on resolution metrics alone.

---

## 📌 Summary

Traditional metrics like user count and response time don't reliably predict financial damage from cyberattacks. A combination of clustering, regression, and visualization provides a clearer risk picture — empowering healthcare leaders to act more decisively.
