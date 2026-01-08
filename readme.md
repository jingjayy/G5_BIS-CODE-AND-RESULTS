# Telecom Customer Churn Prediction
### Comparative Machine Learning Analysis for Revenue Retention

**Subject:** BIS 3218 Business Intelligence Systems
**Institution:** Sunway University
**Year:** 2024/2025

---

## Group Members

| Student Name | Student ID | Contribution Focus |
| :--- | :--- | :--- |
| Hong Jing Jay | 22008338 | Methodology, Pipeline Architecture, Analysis |
| Vicky Leow Ming Fong | 22009591 | Literature Review, Report Synthesis |
| Wong Wei Ting | 24001869 | Data Preparation, Predictive Modelling |
| Geoi Ree Gyn | 22001952 | Business Insights & Recommendations |
| Chan Zheng Shao | 24020059 | Data Exploration & Performance Evaluation |
| Lau Wei Chen | 23125016 | Abstract, Conclusion, Documentation |

---

## Project Overview

This repository contains the source code, analysis reports, and evaluation results for the research project: **"Telecom Customer Churn Prediction."**

The project addresses the critical business challenge of **customer attrition** in the telecommunications sector. Instead of relying on traditional reactive measures, we implemented a **data-driven predictive pipeline** designed to identify high-risk churners before they exit the service.

The system was developed using **Python (Scikit-learn)** and **GPU-accelerated dataframes (cuDF)** to process over **100,000 customer records**. The goal was to solve the problem of **"Silent Attrition"**—where standard linear models overlook complex behavioral patterns. By deploying a **Random Forest ensemble model**, we achieved a significantly higher recall, capturing **351 additional churners** compared to the baseline, directly protecting **Customer Lifetime Value (CLV)**.

---

## Technical Performance

The analysis confirms the superiority of ensemble methods over traditional linear benchmarks for high-dimensional telecom data:

* **Baseline (Logistic Regression):** Accuracy 58.35% | AUC 0.6093
* **Optimized Model (Random Forest):** Accuracy **61.7%** | AUC **0.6655**
* **Business Impact:** Successfully reduced **False Negatives** to 1,779, providing a more robust "net" for proactive retention campaigns.

---

## Key Churn Drivers
The model identified the most influential predictors of churn to guide strategic decision-making:
1. **Equipment Age (eqpdays):** High correlation between aging hardware and service exit.
2. **Customer Tenure:** Critical risk windows identified post-contract expiration.
3. **Usage Behavior:** Sudden drops in 'minutes of use' serving as early warning signals.