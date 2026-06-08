# Global-Cybersecurity-Threats-Dashboard

---

# 🔐 Global Cybersecurity Threats (2015–2024)

---

## 📌 Overview

This project analyzes global cybersecurity incidents from 2015 to 2024 to identify hidden patterns in financial loss, user exposure, resolution time, and organizational response strategies. It is designed for a C-suite healthcare audience, with a focus on practical, high-level insights that inform risk mitigation strategies.

---

## 🎯 Objective

To explore large-scale cybersecurity threat data and deliver actionable insights via an executive-friendly dashboard that highlights trends, clusters, and strategic recommendations for healthcare organizations.

---

## 🧰 Tools Used

- **Python** (pandas, seaborn, scikit-learn, matplotlib)
- **Jupyter Notebooks**
- **Tableau Public**
- **GitHub**

---

## 📌 Key Findings

- **Finance and healthcare industries** report the highest average financial losses.
- **Proactive defense mechanisms** correlate with faster resolution times.
- **No strong linear relationship** was found between resolution time and financial loss.
- **User exposure** is an unreliable predictor of financial loss.
- **Cluster analysis** reveals distinct risk profiles across incidents — enabling tailored response strategies.

---

## 🛠️ Tools & Technologies

| Category        | Tools/Tech                               |
|----------------|-------------------------------------------|
| Data Analysis   | Python (pandas, matplotlib, seaborn)     |
| Machine Learning| scikit-learn (K-Means, Regression)       |
| Visualization   | Tableau Public                           |
| IDE             | Jupyter Notebook                         |
| Version Control | GitHub                                   |

---

## 📊 Visualizations

The following visualizations were created in Tableau to support storytelling for a healthcare executive audience:

- Avg. Financial Loss by Industry (Bar Chart)
- Defense Mechanism vs Resolution Time (Box Plot)
- Resolution Time vs Financial Loss (Scatterplot)
- Global Trends Over Time (Line Chart)
- Incident Map by Country (Choropleth)
- Cluster Comparisons: Financial Loss, Resolution Time, and User Exposure

---

## 📁 File Structure

```
Cybersecurity_Threats_2015-2024/
├── 01_Project Management/
│ ├──Data_Immersion_A6_Project_Brief.pdf
│ ├──Ryan_Wick_Data Immersion_Achievement 6_Project Documentation.docx
│ └── Ryan_Wick_Data Immersion_Achievement 6_Project Documentation.pdf
├── 02_Data/
│ ├──02.01_Data Raw/
│ │ ├──countries.geojson.json
│ │ ├──Global_Cybersecurity_Threats_2015-2024-Original.csv
│ │ └── Global_Cybersecurity_Threats_2015-2024-Raw.csv
│ ├──02.02_Data Cleaned/
│ │ └── Global_Cybersecurity_Threats_2015-2024-First_Pass.csv
├── 03_Scripts/
│ ├──Achievement 6.1_Clean and Understand.ipynb
│ ├──Achievement 6.2_Exploratory Visual Analysis.ipynb
│ ├──Achievement 6.3_Geographical Visualizations with Python.ipynb
│ ├──Achievement 6.4_Supervised Machine Learning_Regression.ipynb
│ ├──Achievement 6.5_Unsupervised Machine Learning_Clustering.ipynb
│ ├──Achievement 6.6_Sourcing & Analyzing Time Series Data.ipynb
│ ├──choropleth_avg_financial_loss.html
│ └── choropleth_avg_financial_loss_with_tooltip.html
├── 04_Analysis/
│ ├──04.01_Reports/
│ ├──04.02_Test Files/
│ ├──04.03_Visualizations/
│ │ ├──Autocorrelation of Differenced Financial Loss.png
│ │ ├──Boxplot of Average Financial Loss by Country.png
│ │ ├──Clusters by Affected Users and Financial Loss.png
│ │ ├──Clusters by Resolution Time and Affected Users.png
│ │ ├──Clusters by Resolution Time and Financial Loss.png
│ │ ├──Correlation Matrix of Numerical Features.png
│ │ ├──Decompse Time Series.png
│ │ ├──Differenced Financial Loss Time Series.png
│ │ ├──Elbow Method - Optimal Number of Clusters.png
│ │ ├──Financial Loss by Attack Type.png
│ │ ├──Financial Loss by Target Industry.png
│ │ ├──Financial Loss by Vulnerability Type.png
│ │ ├──Financial Loss vs Affected Users.png
│ │ ├──Financial Loss vs Incident Resolution Time.png
│ │ ├──Frequency of Financial Loss Categories by Attack Type.png
│ │ ├──Global Financial Loss from Cybersecurity Incidents (2015-2024).png
│ │ ├──Pair Plot of Numerical Features.png
│ │ ├──Regression FInancial Loss vs. Resolution Time.png
│ │ └── Resolution Time by Defense Mechanism.png
├── 05_Sent to Client/
│ └── Global Cybersecurity Threats (2015–2024).pdf
├── README.md
```

---

## 🧪 Data Sources & Ethics

This project uses openly available data on global cybersecurity threats. However, it's important to note:

- Some data may suffer from **self-reporting bias**
- Financial loss values may be **estimated or incomplete**
- Resolution time may vary significantly across organizations
- No private or sensitive data was used

---

## ✅ Recommendations

- **Invest in proactive defenses** (e.g., intrusion detection) to reduce average response time.
- **Use cluster-based risk profiles** to drive strategic planning and resource allocation.
- **Don’t assume faster resolution = less financial loss** — investigate contextual factors.

---

## 🌐 Data Sources

- [Kaggle: Global Cybersecurity Threats Dataset (2015–2024)](https://www.kaggle.com/datasets/victorsoeiro/global-cybersecurity-threats)

---

## 📊 Tableau Storyboard

Explore the final executive dashboard here:  
👉 [**Global Cybersecurity Threats (2015–2024) Tableau Dashboard**](https://public.tableau.com/app/profile/ryan.wick4013/viz/Global_Cybersecurity_Threats_2015-2024_Final/GlobalCybersecurityThreats20152024?publish=yes)

> _Note: The storyboard presents only the final insights. Intermediate steps are documented in the notebooks._

---

## 📌 Summary

This project reveals that traditional metrics like user count and response time don’t reliably predict financial damage from cyberattacks. Instead, leveraging a combination of clustering, regression, and visualization provides a clearer view of cyber risk, empowering healthcare leaders to act more decisively and effectively.
