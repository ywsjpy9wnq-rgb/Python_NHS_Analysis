# Logistic Regression: Predicting Long Waits (>52 weeks) from Staffing Levels

## Research Question
Is there an association between the number of doctors, nurses, ambulance staff, or midwives and whether an organisation has **any patient waiting more than 52 weeks**?

## Data Preparation
- Outcome variable: `long_wait` = 1 if `over_52_and_up_to_65_weeks` > 0, else 0.
- Predictors: `doctors`, `nurses`, `ambulance_staff`, `midwives` (columns from `nhs_staffing_info.csv`).

## Method
- Merge waiting list and staffing data.
- Fit a logistic regression model using `statsmodels.api.Logit`.
- Report odds ratios and p‑values.

## Interpretation
Coefficients > 0 mean higher staffing is associated with **higher odds** of long waits (possibly because larger trusts have both more staff and more long‑wait patients).