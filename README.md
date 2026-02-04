# HR-Workforce-Analytics-EDA
An end-to-end Python analysis of workforce data, focusing on compensation equity and remote work trends.
# HR Analytics: Bridging the Gap Between Performance and Pay

##  Project Overview
This project involves a comprehensive audit of a workforce dataset (1,000+ records) to identify compensation trends and operational efficiency. The project was divided into two critical phases: **Data Engineering/Cleaning** and **Multivariate Exploratory Analysis**.

---

##  Phase 1: Data Cleaning & Integrity (The "Hidden" Work)
Before analysis, the raw data required significant restructuring to ensure accuracy:
* **Scientific Notation Correction:** Fixed corrupted phone number data caused by integer overflow using RegEx.
* **Smart Imputation:** Handled missing Age values using **Grouped Median Imputation** (by Department and Gender) to preserve demographic variance.
* **Type Conversion:** Standardized date objects and numerical floats to optimize memory usage and processing speed.
* **Feature Engineering:** Developed a dynamic `Tenure_Years` metric and `Salary_Tiers` to allow for deeper categorical investigation.

---

##  Phase 2: Key Analysis & Insights
The analysis revealed a "Performance-Agnostic" compensation model within the organization:
* **The Merit Gap:** Discovered a near-zero correlation (0.01) between employee performance and annual salary.
* **Remote Equity:** Confirmed **zero proximity bias**, with Remote and In-Office employees showing identical pay distributions.
* **Regional Hubs:** Identified California as the primary headcount driver, while Nevada operates as the most efficient remote-first satellite hub.

---

##  Recommendations
1. **Merit-Based Incentives:** Shift the compensation model to reward 'Excellent' performers who currently earn the departmental median.
2. **Tenure Retention:** Implement seniority-based pay bands to reduce the risk of institutional knowledge loss.

---

##  Tech Stack
* **Language:** Python 3.10
* **Libraries:** Pandas (Data Manipulation), NumPy (Numerical Logic), Seaborn/Matplotlib (Visualization)
* **Environment:** Kaggle / Jupyter Notebooks
