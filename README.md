# Insurance Fraud Analytics

## Overview
An academic project combining exploratory data analysis in Power BI with predictive modeling in RapidMiner to analyze genuine and fraudulent motor insurance claims.

The project explores claim patterns and compares classification models to support fraud screening and claims review.

## Tools
- **Power BI:** Data transformation and interactive dashboards
- **RapidMiner:** Predictive modeling and model evaluation

## Data Preparation
- Cleaned currency fields and converted them to numeric types.
- Standardized date formats and categorical variables.
- Created a feature measuring the days between an accident and its claim.
- Reviewed missing values before analysis.

## Dashboard Analysis
Developed separate dashboards for genuine and fraudulent claims, exploring:
- Accident reasons and collision types
- Vehicle age, style, and price
- Driver characteristics
- Claim trends over time
- Repair costs

## Predictive Modeling
Compared Decision Tree and Random Forest models using cross-validation. Logistic Regression was also explored during development.

Evaluated model performance using accuracy, fraud recall, and precision, with particular attention to identifying fraudulent claims.

## Reported Results
| Model | Accuracy | Fraud Recall |
|---|---:|---:|
| Decision Tree | 54.02% | 0.02% |
| Random Forest | 52.00% | 19.47% |

Random Forest identified more fraudulent claims than Decision Tree, although its low recall indicates that substantial improvement would be needed before practical use.

## Repository Contents
- **Insurance Fraud Analytics.pdf:** Project report with dashboard screenshots, modeling processes, results, and recommendations.
- **Insurance_fraud_detection_powerbi.pbix:** Power BI dashboard file.
- **insurance_fraud_dt_rf .rmp:** RapidMiner workflow for Decision Tree and Random Forest.
- **insurance_fraud_dt_rf_with_disabled_lr.RMP:** Alternative workflow retaining a disabled Logistic Regression operator.

## Skills Demonstrated
Data cleaning, feature engineering, exploratory data analysis, dashboard design, classification modeling, cross-validation, and business interpretation.

## Limitations and Reproducibility
This is an academic analysis, not a production fraud detection system. Reported metrics are taken from the project report and have not been independently rerun.

The source dataset is not included. The RapidMiner workflows reference a local repository dataset, so users must supply the data and update the retrieval configuration to run them.
