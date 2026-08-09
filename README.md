# BNPL Credit Risk & Conversion Analytics

A Business Analytics and Machine Learning project focused on **Buy Now, Pay Later (BNPL)** customer risk, default prediction, and conversion analysis.

The project combines **Python, SQL, Excel, Power BI, and machine learning** to transform customer and transaction data into business insights that can support credit-risk and checkout decisions.

## Business Problem

BNPL platforms need to balance two objectives:

- Increase customer conversion and successful checkout completion.
- Control credit losses by identifying customers who are likely to default.

The objective of this project is to analyze customer characteristics and behavioral data, identify the major drivers of default risk, and build a predictive model that can help prioritize risk-sensitive decisions.

## Project Objectives

1. Clean and prepare BNPL customer data.
2. Perform exploratory and business-focused data analysis.
3. Use SQL for structured data analysis and querying.
4. Identify factors associated with customer default.
5. Build a classification model for default prediction.
6. Evaluate the model using precision, recall, F1-score, and accuracy.
7. Develop a Power BI dashboard for business reporting and decision support.
8. Document the requirements and process using BRD/FRD documentation.

## Technology Stack

| Area | Tools |
|---|---|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Power BI |
| Database / Querying | SQL, SQLite |
| Machine Learning | Scikit-learn |
| Data Preparation | Excel, Python |
| Documentation | BRD / FRD |
| Development | Jupyter Notebook, Git, GitHub |

## Project Workflow

```text
Raw BNPL Dataset
       |
       v
Data Cleaning & Validation
       |
       v
Exploratory Data Analysis
       |
       +------> SQL / SQLite Analysis
       |
       v
Feature Engineering
       |
       v
Default Prediction Model
       |
       v
Model Evaluation
       |
       +------> Risk Driver Analysis
       |
       v
Power BI Dashboard
       |
       v
Business Recommendations
```

## Key Risk Drivers

The analysis identified several variables with strong influence on predicted default risk, including:

- **Credit score**
- **Monthly income**
- **Debt-to-income ratio**
- **App usage frequency**
- **Age**

These variables can be used as inputs for risk segmentation and targeted credit-policy decisions.

## Model Evaluation

The classification model achieved approximately **60.13% accuracy** in the reported evaluation.

For credit-risk applications, accuracy alone is not sufficient. The model was therefore evaluated using a full classification report, with particular attention to **recall for the default class**.

A higher default recall helps reduce the number of customers who are actually likely to default but are incorrectly classified as low risk. This is important because missed high-risk customers can directly contribute to credit losses.

Reported default-class performance included approximately:

- **Precision:** 50%
- **Recall:** 88%
- **F1-score:** 64%

The model should therefore be interpreted as a risk-screening tool rather than as a standalone approval/rejection mechanism.

## Business Insights

### 1. Credit score is a major risk indicator
Customers with weaker credit profiles generally require stronger risk controls and potentially lower exposure limits.

### 2. Income and debt burden matter together
Monthly income provides an indication of repayment capacity, while the debt-to-income ratio provides additional context about existing financial obligations.

### 3. Behavioral data can add predictive value
App usage frequency and other behavioral variables can complement traditional financial variables when building customer risk segments.

### 4. Recall is important for default detection
In a BNPL risk setting, failing to identify a potential defaulter can be more costly than incorrectly flagging a low-risk customer. Therefore, recall should be considered alongside precision, F1-score, and the business cost of each type of error.

## Power BI Dashboard

The project includes a Power BI-oriented dataset and dashboard deliverables for presenting:

- Customer demographics
- Credit-risk distribution
- Default patterns
- Income and debt indicators
- Customer behavior
- Risk-driver analysis
- Business KPIs

The dashboard is intended to help business stakeholders move from raw model output to actionable risk and customer insights.

## Business Analyst Deliverables

This project demonstrates Business Analyst skills in addition to technical analytics:

- Business problem definition
- Requirement analysis
- BRD / FRD documentation
- Data analysis and KPI identification
- SQL-based analysis
- Dashboard development
- Statistical and ML model interpretation
- Risk and business-impact analysis
- Converting analytical findings into recommendations

## Repository Contents

The repository contains the project notebook, datasets, dashboard-related files, and project documentation.

## Future Improvements

- Perform hyperparameter tuning and cross-validation.
- Compare multiple classification algorithms.
- Apply cost-sensitive learning for default detection.
- Calibrate predicted probabilities for better risk scoring.
- Add customer risk bands such as Low, Medium, and High Risk.
- Integrate model outputs into an automated decision workflow.
- Add monitoring for model drift and changes in default behavior.

## Author

**Sharath C**  
Business Analyst / Engineering Student

GitHub: [06SharXD](https://github.com/06SharXD)

---

**Project:** BNPL Credit Risk & Conversion Analytics  
**Focus:** Business Analytics • Credit Risk • Machine Learning • SQL • Power BI