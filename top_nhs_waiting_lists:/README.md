# Finding NHS Organisations with the Largest Waiting Lists

## Problem
The NHS publishes waiting list sizes for each trust. We want to identify the **three organisations with the highest total waiting list** at the end of September 2025.

## Data
File: `data/nhs_waiting_lists.csv`

## Method
1. Load the CSV into a pandas DataFrame.
2. Sort by `total_waiting_list` in descending order.
3. Select the top 3 rows.
4. Display organisation name and total waiting list.
