# Asset Rental Agreement Analytics Portfolio

## Project Overview

This portfolio project analyzes an active lease asset report for **Lexmark International Inc.** The goal is to understand asset rental costs, contract exposure, vendor patterns, missing data issues, and factors that help predict monthly asset rental amount.

This repository follows the same simple portfolio style as the sample GitHub project: a clear README plus a Jupyter Notebook organized into sections for data access, exploratory analysis, data preparation, modeling, evaluation, and final recommendations.

## Business Problem

A company has many leased assets across contracts, vendors, manufacturers, and locations. Without analytics, it is hard to identify expensive assets, rental anomalies, upcoming contract risks, and cost-saving opportunities.

**Main prediction target:** `Asset Rental Amount`

## Dataset Summary

| Metric | Value |
|---|---:|
| Rows | 1,727 |
| Columns | 33 |
| Total Asset Quantity | 1,751 |
| Unique Contracts | 29 |
| Unique Vendors | 1 |
| Unique Manufacturers | 1 |
| Total Asset Cost | $2,055,670.82 |
| Total Monthly Asset Rental Amount | $171,807.61 |

## Research Questions

1. Which vendors and manufacturers have the highest rental cost exposure?
2. Which asset types have the highest monthly rental amount?
3. Are there unusual rental amounts compared with asset cost?
4. Which features are most useful for predicting asset rental amount?
5. What business recommendations can reduce cost and improve lease management?

## Repository Structure

```text
Asset_Rental_Agreement_Analytics_Portfolio/
├── data/
│   └── Jan_LAR.xlsx
├── notebooks/
│   └── Asset_Rental_Analytics.ipynb
├── outputs/
│   └── generated charts and model files
├── src/
│   └── data_cleaning.py
├── README.md
├── requirements.txt
└── .gitignore
```

## Notebook Sections

### Section I: Accessing the Data
- Load the Excel file
- Review rows, columns, data types, and missing values
- Define the business goal and prediction target

### Section II: Exploratory Data Analysis
- Descriptive statistics
- Vendor and manufacturer cost analysis
- Rental amount distribution
- Asset cost vs rental amount relationship
- Missing data visualization

### Section III: Prepare Data for Training
- Clean column names
- Handle missing values
- Create useful features such as rental-to-cost ratio, lease age, and days until primary term end
- Encode categorical variables

### Section IV: Regression Modeling
- Train Linear Regression and Random Forest Regressor
- Compare model performance using MAE, RMSE, and R²

### Section V: Model Evaluation and Visualization
- Actual vs predicted rental amount plot
- Feature importance chart
- Residual error review

### Section VI: Business Recommendations
- Identify high-cost vendors/assets
- Monitor rental-to-cost anomalies
- Improve missing data quality
- Use model predictions to flag unusual lease pricing

## How to Run

1. Clone or download this repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook notebooks/Asset_Rental_Analytics.ipynb
```

4. Run all cells from top to bottom.

## Expected Outputs

- Cleaned dataset preview
- EDA charts using Plotly
- Regression model comparison table
- Feature importance results
- Business insights and recommendations

## Tools Used

- Python
- Pandas
- NumPy
- Plotly
- Scikit-learn
- Jupyter Notebook
- Joblib

## Author

Prakash Ghatani
