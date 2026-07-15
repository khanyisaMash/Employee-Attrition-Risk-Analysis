
# Employees Leaving Risk Analysis

A data analytics project identifying where risk of employees leaving is heavily concentrated, using Python for statistical validation and Power BI for interactive reporting.

## Use Case: To reduce the number of employees leaving, what actions should be taken by HR?**

The findings show that: **employees working overtime in the lowest salary quartile leave at 58.5%, 3.6x the company average and new hires (under 2 years tenure) working overtime are leaving at roughly 3x the company average and within that tenure group, three job roles carry the highest risk:**

1. **Laboratory Technician** - 64.3% attrition rate among new hires working overtime
2. **Sales Executive** - 62.5% attrition rate among new hires working overtime
3. **Research Scientist** - 48.3% attrition rate among new hires working overtime

**Recommended action:** review overtime policy and compensation for employees working overtime in the lowest salary quartile, and extend that review to new hires in the three roles above.

*(A fourth job role, Sales Representative, showed 80% attrition but on a sample of only 10 — too small to act on, worth monitoring only.)*

## Key Findings

| Finding | Result |
|---|---|
| Overall attrition rate | 16.1% |
| Overtime workers | 30.5% (vs. 10.4% non-overtime) |
| Overtime + lowest salary quartile (top validated segment) | 58.5% — 3.6* baseline |
| New hires (0-2 yrs) + overtime | 51.0% — ~3* baseline |
| Highest-risk roles within new-hire + overtime group | Laboratory Technician, Sales Executive, Research Scientist |


### 4. Reporting (Power BI)
- Two-page report:
  - **Page 1 — Overview:** KPI cards (headcount, attrition count, attrition rate) and four driver charts (Overtime, Salary Band, Job Satisfaction, and Tenure Group)
  - **Page 2 — Segments:** heatmap matrix, Overtime × Salary Band  and Overtime × Tenure Group, with a red text fill to flag at risk groups
             -chart showing at rest job roles for new hires.


## Repository Structure
```
data/           Cleaned fact table and dimension tables (CSV)
scripts/        Python data cleaning and dimension-modeling pipeline
dashboard/      Power BI report file (.pbix) and screenshots
docs/           Written business recommendations (Word doc)
```

## Tools Used
Python (pandas, scipy, scikit-learn), Power BI (Power Query, DAX, star-schema modeling)

## Data Source
[IBM HR Analytics Employee Attrition & Performance dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) (Kaggle)

## How We Got There: Methodology
