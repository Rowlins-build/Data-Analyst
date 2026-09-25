# Data Analysis Project

## Overview
This project involves cleaning and analyzing shelter outcome records from the Austin Animal Center (25 Feb 2025 – 5 May 2025, 2,003 raw rows) using Microsoft Excel to identify adoption trends, whether age or naming affects an animal's outcome, and data-quality issues hidden in the raw records. The goal was to transform raw, messy data into a clean, structured format and extract meaningful insights.

## Objectives
- Clean and prepare raw shelter data for analysis
- Identify adoption rate patterns across animal types, and whether age or naming correlates with outcome
- Present findings through clear summary tables and written analysis

## Tools Used
- Microsoft Excel
- COUNTIF, VLOOKUP, IF, TEXT, DATEVALUE, TRIM, FIND/RIGHT/LEFT, SEARCH
- Summary tables built with live formulas against the cleaned dataset

## Process
1. **Data Cleaning**: Removed 2 exact duplicate rows, deleted a redundant column, standardized names and ages, fixed broken date formatting, and split combined fields (sex/sterilization status) into separate columns
2. **Data Exploration**: Reviewed the dataset structure, identified 42 distinct age formats and inconsistent text fields needing standardization
3. **Analysis**: Calculated adoption rate by animal type, compared mean vs. median age across outcome types, compared named vs. unnamed animal outcomes, and cross-tabulated outcome type by animal type
4. **Visualization**: Built summary tables showing outcome counts, percentages, and rates by category (see `Summary_Analysis` sheet)

## Key Findings
- Adoption rate depends heavily on species: Dogs ~62%, Cats ~53%, "Other" (wildlife/exotics) ~16%, Birds ~11%
- Reclaimed (Return to Owner) animals are ~2.7x older on average than adopted animals — lost adult pets get reclaimed, while young strays get adopted
- Named animals are adopted 69.5% of the time vs. 24.5% for unnamed animals, but this reflects shelter triage decisions made before naming, not naming itself causing the outcome
- 2,001 outcome rows represent only 1,958 distinct animals — 41 animals exited the shelter more than once during the period
- One record showed an animal "adopted" three years before its recorded birth date, revealing that ages in the source system are stored without validation

## Files in this Repository
- `ShelterFiles_outcomes.xlsx` — The main Excel file containing raw data, cleaning steps, and analysis (sheets: Raw, Clean, Summary_Analysis, Data_Quality_Log)

## How to Use
1. Download the `.xlsx` file
2. Open in Microsoft Excel (or compatible spreadsheet software)
3. Navigate through the sheets: "Raw" (original data), "Clean" (standardized dataset), "Summary_Analysis" (findings), "Data_Quality_Log" (audit trail of every change)

## Author
Eng. Ekumi Rowlins Iseri


