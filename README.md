# Hospital Readmission Risk Prediction

### Overview
Hospital readmissions represent a major cost and quality challenge in healthcare systems. This project develops a machine learning model to predict patient readmission risk using administrative and clinical data available during hospitalization.

### Goal: 
To identify high-risk patients early and support preventive interventions.

### Problem Statement:
Can we predict whether a patient will be readmitted based on available hospitalization and prior utilization data?

### Dataset:

The dataset contains 10 years of hospitalization data, including:

- Patient age group
- Length of stay
- Number of lab procedures
- Number of medications
- Prior inpatient, outpatient, and emergency visits
- Primary and secondary diagnoses
- Diabetes management indicators
- Readmission outcome (yes/no)

Each row represents a single hospital encounter

### Exploratory Data Analysis:

**Key insights:**

1. Prior inpatient visits are the strongest predictor of readmission.
2. Readmission risk increases with age (up to 80–90 years).
3. Patients with chronic conditions (e.g., diabetes, circulatory diseases) show higher readmission rates.
4. Hospital stay complexity shows moderate impact compared to prior utilization.

### Models Implemented:
- Logistic Regression
- Random Forest

Threshold optimization was performed to prioritize recall

### Limitations:

- No socioeconomic variables
- No post-discharge data
- Limited diagnostic granularity
- No mortality information
