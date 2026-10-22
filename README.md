# HR Workforce Analytics | Python, Jupyter Notebook & Power BI

## Project Overview

This project explores workforce characteristics, employee attrition, job satisfaction and other HR indicators using a public synthetic employee dataset.

The project combines Python-based data quality assessment and exploratory data analysis in Jupyter Notebook with interactive reporting in Power BI.


**Tools:** Python, pandas, NumPy, Jupyter Notebook, Power BI

## Project Objectives

- Assess dataset quality, consistency and suitability for analysis.
- Explore workforce composition and employee characteristics.
- Investigate attrition patterns across age groups, departments, job roles and other employee attributes.
- Examine job satisfaction and selected workforce indicators.
- Develop an interactive Power BI report for segmented analysis.
- Document KPI definitions, methodological choices and data limitations.

## Repository Structure

```text
hr-workforce-analytics/
├── README.md
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   └── HR_Data_Quality_and_Exploratory_Analysis.ipynb
└── powerbi/
    ├── HR_Workforce_Analytics.pbix
    └── screenshots/
        ├── executive_overview.png
        └── workforce_retention_insights.png
```

## Dataset

The project uses the IBM HR Analytics Employee Attrition & Performance dataset, publicly available through Kaggle.

The dataset contains 1,470 employee records and 35 original columns. Three constant columns were excluded during preparation, leaving 32 columns for analysis.

The data is synthetic and must not be interpreted as representing actual employees or the workforce of the European Parliament or any other institution.

## Methodology

### 1. Data Quality Assessment — Python

The Jupyter Notebook documents the data inspection and preparation process, including:

- Dataset structure and data types.
- Missing-value assessment.
- Duplicate-record and employee-identifier checks.
- Constant-column identification.
- Category and value-range checks.
- Consistency checks between selected employment-related fields.

### 2. Exploratory Data Analysis — Python

The notebook explores workforce characteristics and relationships between selected variables. The analysis is descriptive and aims to identify patterns worth investigating further, rather than establish causal relationships.

### 3. Interactive Reporting — Power BI

The Power BI report presents selected HR indicators through interactive visualisations and filters.

The report focuses on workforce composition, attrition patterns and employee-related indicators, with the aim of making comparisons across relevant employee groups easier to explore.

## KPI Definitions

- **Total Employees:** Number of distinct employee identifiers in the dataset.
- **Attrition Count:** Number of records where the attrition indicator is "Yes".
- **Attrition Rate:** Attrition count divided by the total number of employees in the analysed dataset.
- **Average Tenure:** Average number of years employees have spent at the company.
- **Average Monthly Income:** Mean value of the dataset's `MonthlyIncome` field.
- **Average Training Frequency:** Mean value of `TrainingTimesLastYear`, representing the recorded number of training occasions in the previous year.

These indicators describe the available dataset. The attrition rate is not an annual turnover rate because the dataset does not provide a time series of employee departures and workforce size.

The dataset does not specify the currency for `MonthlyIncome`; therefore, no currency symbol should be assumed.

## Limitations

- The dataset is synthetic and may not reflect the characteristics of a real organisation.
- The analysis is descriptive and does not establish causation.
- The available data does not support reliable conclusions about changes over time.
- Findings should be interpreted in the context of the dataset and its definitions.
- Employee-level indicators should not be treated as a basis for consequential HR decisions without appropriate validation, context and safeguards.

## Reproducibility

To explore the Python analysis, open the notebook in Jupyter Notebook or JupyterLab and run the cells in order after installing the required Python libraries.

To explore the dashboard, download `HR_Workforce_Analytics.pbix` and open it using Power BI Desktop.

Data source: IBM HR Analytics Employee Attrition & Performance dataset, available on Kaggle. Please refer to the original dataset page and its applicable licence for source and redistribution terms.

