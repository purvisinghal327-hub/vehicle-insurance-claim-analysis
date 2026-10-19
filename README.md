# Vehicle Insurance Claim Risk Analysis & Prediction

## Project Overview

This project analyses vehicle insurance policy data to understand claim patterns and explore whether machine learning can help predict claim occurrence.

Using R for data analysis and modelling and Excel for reporting, the project examines how claim rates vary across customer age, vehicle age, vehicle segment, and fuel type.

## Objectives

- Explore the characteristics of insurance policies with and without claims.
- Identify patterns and relationships between policy characteristics and claim occurrence.
- Compare Logistic Regression and Random Forest classification models.
- Present key findings through an Excel dashboard.

## Tools & Technologies

- **R:** Data cleaning, exploratory data analysis, statistical testing, and predictive modelling.
- **Excel:** KPI reporting, charts, and dashboard creation.
- **Statistical analysis:** Hypothesis testing and examination of claim-rate differences.
- **Machine learning:** Logistic Regression and Random Forest.

## Dataset

The analysis covers **58,592 insurance policy records**, including 3,748 claims.

The original dataset is not included in this repository. To reproduce the analysis, obtain the dataset from its authorised source and update the file path in the R script as needed.

## Key Findings

- **Overall claim rate:** 6.40%.
- **Total policies analysed:** 58,592.
- **Total claims observed:** 3,748.
- Claim rates varied across customer age groups and vehicle characteristics.
- The 65–69 customer age group had an observed claim rate of approximately 13.57%; this finding should be interpreted alongside the group's sample size.
- The 10+ years vehicle-age group contained only six policies, so its observed 0% claim rate is not a reliable general conclusion.

## Model Comparison

Two classification models were evaluated using the Area Under the ROC Curve (AUC).

| Model | AUC |
|---|---:|
| Logistic Regression | 0.607 |
| Random Forest | 0.625 |

Random Forest achieved a slightly higher AUC. However, both models showed limited ability to distinguish policies with claims from those without claims. Further feature engineering, model tuning, and evaluation would be needed before considering practical deployment.

## Excel Dashboard

The dashboard presents key metrics and visual comparisons through five charts:

1. Claim rate by vehicle age
2. Claim rate by customer age
3. Claim rate by vehicle segment
4. Claim rate by fuel type
5. Model comparison using AUC

Supporting worksheets provide the underlying KPI and segment-level summaries.

![Vehicle Insurance Claim Analysis Dashboard](dashboard.png)

## Repository Contents

- `Insurance_Claim_Dashboard_Final_v2.xlsx` — Excel dashboard and supporting worksheets.
- 01_data_exploration.R — data analysis and modelling code.
- `Insurance Claim Risk Analysis.Rproj` — RStudio project file.
- `.gitignore` — files and folders excluded from version control.

## Limitations

- The models have modest predictive performance.
- Some age groups have small sample sizes.
- Observed associations do not establish causation.
- Model performance should be assessed using additional evaluation metrics and appropriate validation before real-world use.

## Conclusion

This project demonstrates an end-to-end workflow combining data exploration, statistical analysis, classification modelling, and Excel-based reporting to investigate vehicle insurance claim patterns.

**Skills demonstrated:** R, exploratory data analysis, statistical testing, machine learning, Excel dashboards, and analytical communication.

