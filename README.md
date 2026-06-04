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

### Missing Data Assessment

Several variables contained missing values represented by the symbol "?".

- Weight had approximately 97% missing values.
- Medical Specialty had approximately 49% missing values.
- Payer Code had approximately 40% missing values.

Due to the extremely high proportion of missing data, Weight will likely be excluded from further analysis. Variables with moderate missingness will be evaluated on a case-by-case basis.
