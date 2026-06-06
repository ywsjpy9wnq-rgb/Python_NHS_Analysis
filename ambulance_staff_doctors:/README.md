# Do Organisations with Ambulance Staff Have More Doctors?

## Objective
Compare the average number of doctors between two groups:
- Organisations that employ ambulance staff
- Organisations that do not

## Data
File: `data/nhs_staffing_info.csv`

## Method
1. Create a boolean mask for rows where `ambulance_staff > 0`.
2. Count the number of organisations with ambulance staff.
3. Compute the mean of `doctors` for each group.

## Interpretation
The result shows whether ambulance‑staffed organisations tend to be larger (more doctors) or not.