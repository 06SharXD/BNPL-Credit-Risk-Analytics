# BNPL Credit Risk & Conversion Analytics

This project looks at **Buy Now, Pay Later (BNPL)** customer data to understand two things: who is more likely to default and what customer factors are related to that risk.

I worked on the project from both a **data/ML** and **business analysis** perspective, using Python, SQL, Excel and Power BI.

## What was the problem?

A BNPL company wants to grow its customer base without taking on unnecessary credit risk.

So the main questions I wanted to answer were:

- Which customer factors are related to default?
- Can we build a model to identify customers who may be at higher risk?
- Which metrics should be used to judge the model?
- How can the results be presented clearly to a business team?

## What I did

1. Cleaned and prepared the BNPL dataset.
2. Explored the data to understand customer and default patterns.
3. Used SQL/SQLite to perform structured analysis.
4. Prepared features for a classification model.
5. Built and evaluated a default prediction model.
6. Looked at the main factors contributing to predicted risk.
7. Prepared data for a Power BI dashboard.
8. Documented the business requirements using BRD/FRD documentation.

## Tools used

- **Python** – Pandas, NumPy, Matplotlib, Scikit-learn
- **SQL / SQLite** – data querying and analysis
- **Excel** – data preparation and supporting analysis
- **Power BI** – dashboard and business reporting
- **Jupyter Notebook** – analysis and model development
- **Git / GitHub** – version control and project documentation

## Project flow

```text
BNPL Dataset
    ↓
Data Cleaning
    ↓
Exploratory Analysis
    ↓
SQL Analysis
    ↓
Feature Preparation
    ↓
Default Prediction Model
    ↓
Model Evaluation
    ↓
Risk Driver Analysis
    ↓
Power BI Dashboard
    ↓
Business Insights
```

## Some of the findings

The variables that stood out in the analysis included:

- Credit score
- Monthly income
- Debt-to-income ratio
- App usage frequency
- Age

These factors were useful for understanding differences in default risk across customers.

## Model results

The model had an overall accuracy of about **60.13%** in the reported evaluation.

However, accuracy was not the main metric I focused on. Since the goal is to identify customers who may default, **recall for the default class** is particularly important.

The reported results for the default class were approximately:

| Metric | Result |
|---|---:|
| Precision | 50% |
| Recall | 88% |
| F1-score | 64% |

The high recall means the model was able to identify a large proportion of the customers who actually defaulted. At the same time, the precision shows that some customers predicted as high risk did not actually default.

So, the model is better viewed as a **risk-screening aid** rather than something that should make a credit decision on its own.

## Power BI dashboard

The dashboard is designed to give a business-level view of the data, including:

- Customer profile and demographics
- Default rate
- Credit-risk patterns
- Income and debt information
- Customer behaviour
- Key risk factors
- Relevant KPIs

The idea is to make the analysis easier for someone who does not need to look through the Python notebook or model output.

## Business Analyst work

Along with the technical analysis, I worked on:

- Defining the business problem
- Identifying requirements
- Preparing BRD and FRD documentation
- Identifying useful KPIs
- SQL-based data analysis
- Dashboard planning
- Interpreting model results from a business perspective
- Converting the findings into practical recommendations

## Files in this repository

The repository contains the analysis notebook, datasets, dashboard-related files and project documentation.

## What I would improve next

If I continue working on this project, I would like to:

- Test a few more classification models.
- Tune the model and compare cross-validation results.
- Look at the cost of false positives vs. false negatives.
- Create clear Low / Medium / High risk segments.
- Calibrate the model's probability scores.
- Add model monitoring if this were used with real BNPL data.

## Author

**Sharath C**

Business Analyst / Engineering Student

GitHub: [06SharXD](https://github.com/06SharXD)