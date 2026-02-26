# Hospital Readmission Risk Prediction

This project presents a machine learning–based analysis of hospital administrative and clinical data to identify key predictors of patient readmission, supporting data-driven healthcare intervention strategies.

## Industry

Healthcare / Health Tech / Hospital Operations

## Business Problem

Hospital readmissions represent a major cost and quality challenge for healthcare systems.
Healthcare providers need a way to identify high-risk patients at discharge in order to implement preventive interventions and reduce avoidable readmissions.

## Objective

Develop a predictive model to estimate the probability of 30-day hospital readmission using structured hospitalization and prior utilization data.

## Data Description

Dataset containing 10 years of hospital encounter data (20K+ records), including:

- Patient age group
- Length of hospital stay
- Number of lab procedures
- Number of medications administered
- Prior inpatient, outpatient, and emergency visits
- Primary and secondary diagnoses
- Diabetes management indicators
- Readmission outcome (Yes/No)

Each row represents a single hospital encounter.

## Tools Used

- Python (Pandas, NumPy)
- Scikit-learn
- Logistic Regression
- Random Forest
- Data Cleaning & Feature Engineering
- Classification Metrics (Recall, Precision, ROC-AUC)

## Methodology

1. Performed data cleaning, preprocessing, and categorical encoding.
2. Conducted structured Exploratory Data Analysis (EDA) by demographic, clinical complexity, prior utilization, and diagnosis categories.
3. Built baseline classification models.
4. Trained and evaluated Logistic Regression and Random Forest models.
5. Optimized the decision threshold to prioritize recall in a healthcare context.
6. Compared model performance using ROC-AUC, Recall, Precision, and confusion matrix analysis.

## Key Findings

- Prior inpatient visits were the strongest predictor of readmission (patients with previous admissions showed more than 2x higher risk).
- Readmission risk increased progressively with age up to the 80–90 group.
- Chronic conditions (especially Diabetes) showed higher readmission rates than acute conditions.
- Adjusting the classification threshold increased recall from 41% to 75%, improving early identification of high-risk patients.

## Business Impact

The model enables healthcare providers to:

- Identify high-risk patients before discharge
- Prioritize follow-up interventions
- Improve resource allocation
- Potentially reduce readmission-related costs

By prioritizing recall, the model supports preventive healthcare strategies.

## Challenges & Learnings

- Observed limited predictive improvement from non-linear models, suggesting predominantly linear relationships in structured hospital data.
- Learned to balance precision vs recall based on real-world healthcare priorities.
- Reinforced understanding of model interpretability in clinical contexts.
- Recognized limitations of administrative-only datasets without socioeconomic or post-discharge variables.
