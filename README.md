# hospital-readmission-analysis
Exploratory analysis of hospital readmission patterns using healthcare encounter data.

## Project Goal

This project explores factors associated with hospital readmissions using healthcare encounter data from U.S. hospitals.

## Research Questions

1. What factors are associated with hospital readmissions?
2. How does age affect readmission rates?
3. Do certain diagnoses have higher readmission frequencies?
4. Does length of stay influence readmission outcomes?

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

### Initial exploration
Initial exploration showed that the dataset contains 101,766 records and 50 variables. The main outcome variable is readmission status, while predictors include demographic characteristics, hospital utilization measures, diagnoses, medications, and lab result indicators.

### Data Cleaning
The goal of this phase was to prepare the diabetes dataset for exploratory data analysis and modeling by addressing missing values, removing unnecessary variables, and ensuring data quality.

Data Cleaning Procedures
-Replaced placeholder values (?) with missing values (NaN).
-Removed identifier variables (encounter_id, patient_nbr).
-Removed variables with excessive missingness (weight, payer_code, medical_specialty).
-Removed observations with invalid gender, race and medical diagnodid classifications.
-Checked for duplicate records and removed them
-Retained variables relevant to the research questions on readmission

| Dataset Stage    |    Rows | Columns |
| ---------------- | ------: | ------: |
| Original Dataset | 101,766 |      50 |
| Cleaned Dataset  |  71,518 |     44 |

After data cleaning, the dataset was reduced from 101,766 observations to 71,518 observations. Records were removed due to duplicate patient encounters and the exclusion of variables with excessive missing values.

| Readmission Status | Percentage |
| ------------------ | ---------: |
| NO                 |     60.10% |
| >30                |     31.10% |
| <30                |      8.80% |

The majority of patients (60.10%) were not readmitted after discharge. Approximately 31.10% were readmitted after 30 days, while only 8.80% were readmitted within 30 days. This indicates that the dataset is somewhat imbalanced.




Due to the extremely high proportion of missing data, Weight will likely be excluded from further analysis. Variables with moderate missingness will be evaluated on a case-by-case basis.
