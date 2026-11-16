# CareGap Kenya: Predicting Household Health Insurance Exclusion & Healthcare Access Barriers Across Kenya’s 47 Counties

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Status](https://img.shields.io/badge/Status-In%20Progress-green)
![Domain](https://img.shields.io/badge/Domain-Public%20Health%20%26%20Policy-teal)

## Project Overview
Despite Universal Health Coverage (UHC) reforms and Kenya’s transition from the National Health Insurance Fund (NHIF) to the **Social Health Authority (SHA)**, millions of registered Kenyans remain without active insurance coverage due to financial constraints, informal employment, and geographic barriers.

**CareGap Kenya** analyzes data from the **2022 Kenya Demographic and Health Survey (KDHS)** across all 47 counties—covering men, women, and children—to map regional coverage disparities, segment vulnerable household archetypes via clustering, and build explainable machine learning classifiers that predict health insurance exclusion risk to guide targeted SHA enrollment and subsidy allocation.

---

## Key Research Questions
* **County & Geospatial Disparities:** Which of Kenya’s 47 counties experience the steepest combined burden of uninsured households and financial or distance barriers to healthcare?
* **Demographic & Intra-Household Gaps:** How does health insurance coverage vary across gender (men vs. women), age cohorts (children under 18, youth, working-age adults, and the elderly), and rural vs. urban residences?
* **Top Socioeconomic Predictors:** Which factors (wealth quintile, education attainment, employment type, household size, and county of residence) most strongly predict being uninsured?
* **Barriers & SHA Policy Implications:** How closely does lack of insurance correlate with delayed care-seeking due to cost or facility distance, and which demographic groups require priority SHA means-testing and subsidies?

---

## Repository Structure
```text
caregap-kenya-capstone/
├── app/                     # Streamlit interactive policy & risk prediction web app
├── data/
│   └── public/              # Open-access HDX county-level benchmark CSVs
│       ├── access-to-health-care_subnational_ken.csv
│       └── health-insurance_subnational_ken.csv
├── notebooks/               # Jupyter / Google Colab notebooks (EDA, Clustering, Modeling, SHAP)
├── src/                     # Reusable data cleaning, feature engineering, and modeling scripts
├── .gitignore               # Excludes restricted DHS microdata (.DTA / .ZIP)
└── README.md                # Project documentation
