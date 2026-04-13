# 💳 Fintech Credit Risk & Data Integrity Audit

## 📌 Project Overview
This project performs a **Root Cause Analysis (RCA)** on a lending dataset to identify high-risk applicant profiles and audit data integrity. By identifying "red flags" and impossible data points, this analysis provides actionable recommendations for a Fintech lending product.

## 🔍 Key Findings (Root Cause Analysis)
* **Data Integrity Red Flags:** Discovered and neutralized ~3% of the dataset containing impossible values, such as applicant ages of **144 years** and employment lengths of **123 years**.
* **Risk Inflection Point:** Identified that the **Loan-to-Income (LTI) ratio** is the primary predictor of default. Risk remains stable until the **30% threshold**, after which default rates spike significantly.

## 💡 Business & Product Recommendations
Based on the data audit, I recommend the following product guardrails:
* **Automated Hard-Stop:** Implement a rejection filter for any applicant whose loan request exceeds **40% of their annual income**.
* **Manual Review Trigger:** Applications with an LTI between **30%–40%** should be flagged for manual credit officer oversight.
* **Front-end Validation:** Update the user application UI to prevent "impossible" age and employment inputs at the source.

## 🛠️ Tools Used
* **Python (Pandas):** Data Sanitization and Audit
* **Seaborn:** Statistical Data Visualization
* **Jupyter Notebook:** Exploratory Data Analysis (EDA)

---
*Created as part of a Data Science Portfolio focusing on Fintech and Product Management.*
