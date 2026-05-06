# Hospital Readmission Analysis

## Overview
This project analyzes hospital readmission patterns using the UCI Diabetes 130-US Hospitals dataset (101,745 patients). The goal: identify which patients are likely to be readmitted within 30 days.

## Tools Used
| Tool | Purpose |
|------|---------|
| Excel | Data audit & missing value documentation |
| SQL (SQLite) | Business queries & patient segmentation |
| Python | EDA, visualization & ML modeling |
| Power BI | Interactive dashboard |

## Dataset
- **Source:** UCI ML Repository — Diabetes 130-US Hospitals
- **Link:** https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008
- **Size:** 101,745 rows, 50 columns

## Key Findings
1. **11.16%** patients readmitted within 30 days
2. **20-30 age group** has highest readmission rate — 14.25%
3. **V58 diagnosis** has 41.7% readmission rate — highest risk
4. Patients with **16+ medications** have 67% higher readmission risk
5. **8-10 hospital days** = peak readmission risk zone
6. **Discharge destination** is strongest predictor of readmission

## ML Model — XGBoost
- **Algorithm:** XGBoost Classifier
- **Recall:** 60%
- **ROC-AUC:** 63.12%
- **Key insight:** discharge_disposition_id is most important feature (SHAP)

## Business Recommendations
- 48-hour callback system for V58 patients after discharge
- Special follow-up protocol for 20-30 age group
- Mandatory medication review for 15+ medications patients
- Strengthen discharge planning team — nursing facility patients pe focus

## Author
**Avinash** | Aspiring Data Analyst
Tools: Excel • SQL • Python • Power BI
