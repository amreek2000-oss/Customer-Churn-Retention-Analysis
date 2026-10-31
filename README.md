[README.md.md](https://github.com/user-attachments/files/34216944/README.md.md)
<div align="center">

# 📊 Customer Churn & Retention Analytics
### Predictive Machine Learning Pipeline & Power BI Executive Dashboard

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

</div>

## 📌 Executive Overview

Customer churn directly impacts business revenue and lifetime value (LTV). This project delivers an end-to-end data analytics and predictive Machine Learning solution designed to identify churn drivers, calculate probabilistic risk scores, and deliver dynamic visual analytics through an interactive **Power BI Executive Dashboard**.

> 💡 **Project Achievement:** Built a **Random Forest Classifier** achieving **`99.81% Accuracy`** and a **`1.000 ROC AUC Score`**, seamlessly enriching dataset records with `Churn_Probability` and `Predicted_Churn_Risk` metrics for real-time retention tracking.

---

## 🛠️ Complete Tech Stack

```text
🔴 SQL (MySQL)           ➜ Data Extraction & Staging
🟡 Python (Pandas/NumPy) ➜ Data Preprocessing & Cleaning
🟢 Scikit-Learn          ➜ Random Forest ML Model & Risk Scoring
🔵 Power BI (DAX)        ➜ Dynamic KPIs & Visual Analytics
🟣 Git / GitHub          ➜ Portfolio Version Control & Documentation
```

| Domain | Tools & Technologies | Focus Area |
| :--- | :--- | :--- |
| 🗄️ **Database & Pipeline** | `SQL (MySQL)` | Structured querying, relational staging, and schema design |
| 🐍 **Preprocessing & EDA** | `Python`, `Pandas`, `NumPy` | Data validation, missing value imputation, and encoding |
| 🤖 **Machine Learning** | `Scikit-Learn` (`RandomForestClassifier`) | Model training, cross-validation, and risk probability scoring |
| 📊 **Business Intelligence** | `Power BI Desktop`, `DAX` | Measures creation, layout modeling, and visual interactivity |
| 📁 **Environment & VCS** | `VS Code`, `Git`, `GitHub`, `Markdown` | Deployment readiness and executive project documentation |

---

## ⚡ Interactive Executive Metrics (Power BI DAX)

<div align="center">

| Metric Name | Value | DAX Calculation | Business Impact |
| :--- | :---: | :--- | :--- |
| 👥 **Total Customers** | **`64.37K`** | `COUNT(customer_churn[CustomerID])` | Establishes total operational user base |
| 📉 **Total Churn** | **`30.00K`** | `SUM(customer_churn[Churn])` | Measures absolute account loss volume |
| 🎯 **Churn Rate** | **`47.37%`** | `DIVIDE([Total Churn], [Total Customers], 0)` | Tracks relative churn proportion |
| 🚨 **High-Risk Users** | **`30.00K`** | `CALCULATE([Total Customers], Risk = "High Risk")` | Direct target list for customer success outreach |

</div>

---

## 🚀 Technical Architecture

```text
[ 📁 Raw Customer Dataset ] 
          │
          ▼
[ 🗄️ SQL Data Staging & Cleaning ]
          │
          ▼
[ 🐍 Python ML Pipeline (train_churn_model.py) ]
  ├── 1. Preprocessing & One-Hot Encoding
  ├── 2. Random Forest Classifier Training (99.81% Acc)
  └── 3. Probabilistic Risk Scoring (Churn_Probability)
          │
          ▼
[ 📊 Enriched Dataset (customer_churn_with_ml.csv) ]
          │
          ▼
[ 📈 Power BI Interactive Dashboard (Customer_Churn_Retention_Analysis.pbix) ]
  ├── 💳 Executive KPI Summary Banner
  ├── 🎛️ Gender & Subscription Type Slicers
  ├── 📞 Support Calls Column Chart
  ├── 📜 Contract Length Clustered Bar Chart
  └── 🍩 ML Risk Categorization Donut Chart
```

---

## 🎯 Power BI Visual Architecture

* 💳 **Dynamic KPI Header:** Instant tracking for Total Customers (`64.37K`), Total Churn (`30K`), Churn Rate (`47.37%`), and High-Risk Customers (`30K`).
* 🎛️ **Interactive Slicers:** Dynamic multi-segment filtering across `Gender` (*Male, Female*) and `Subscription Type` (*Basic, Standard, Premium*).
* 📞 **Support Calls Dynamic Chart:** Clustered column chart highlighting escalating churn trends corresponding to higher support interaction counts.
* 📜 **Contract Tenure Bar Chart:** Clustered bar visual comparing retention distributions across Monthly, Quarterly, and Annual contracts.
* 🍩 **ML Risk Segmentation Donut Chart:** Risk categorization visual (`Count of CustomerID by Predicted_Churn_Risk`) showing High Risk vs. Low Risk proportions.

---

## 📂 Repository Structure

```text
├── 📄 customer_churn_cleaned.csv            # Cleaned baseline dataset
├── 📄 customer_churn_with_ml.csv             # Enriched dataset containing ML risk probabilities
├── 🐍 train_churn_model.py                   # Python Random Forest ML script
├── 📊 Customer_Churn_Retention_Analysis.pbix # Interactive Power BI Dashboard
├── 📋 requirements.txt                      # Python environment dependencies
└── 📝 README.md                              # Portfolio project documentation
```

---

## 💡 Key Business Takeaways & Strategy

1. 📞 **Support Escalation Alert:** Customers exceeding 3 support calls show a high probability of churning. Automated retention triggers should be deployed immediately.
2. 📜 **Contract Migration:** Monthly subscribers account for a large portion of churned accounts. Offering conversion incentives to Annual plans will increase long-term customer stability.
3. 🎯 **Targeted Campaigning:** Focusing retention budgets strictly on the **`30K High-Risk`** accounts flagged by the Machine Learning model maximizes ROI and prevents churn proactively.

---
