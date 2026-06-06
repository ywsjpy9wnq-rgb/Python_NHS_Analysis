# Cross‑tabulation: Patient Wait Groups vs. Doctor Count Groups

## Goal
Create a summary table showing how many NHS organisations fall into each combination of:
- Number of patients waiting ≤18 weeks (4 categories)
- Number of doctors (4 categories)

## Data Sources
- `nhs_waiting_lists.csv` – contains `organisation_code` and `up_to_18_weeks`
- `nhs_staffing_info.csv` – contains `organisation_code` and `doctors`

## Steps
1. Merge the two datasets on `organisation_code`.
2. Use `pd.cut()` to create categorical groups for patients and for doctors.
3. Build a contingency table with `pd.crosstab()`.
4. Display the table with row and column totals.