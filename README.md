# Asset Rental Agreement Analytics Portfolio

## Project Overview

This project studies an active lease asset report for Lexmark International Inc.

The main goal of this portfolio is to identify ways to reduce costs, lower contract risks, and improve lease management. The analysis looks at asset rental costs, lease contracts, missing data, and the factors that affect monthly rental payments

Using data analysis, charts, and machine learning, the project turns raw lease data into useful business information that helps with financial and business decisions.

The project follows a simple data science process:

- Data Collection
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Predictive Modeling
- Model Evaluation
- Business Recommendations

## Business Problem

With this company has many leased assets across contracts, vendors, manufacturers, and locations. Without analytics, it is hard to identify expensive assets, rental anomalies, upcoming contract risks, and cost-saving opportunities.

- The company has many leased assets in different locations.
- These assets are managed under different contracts, vendors, and manufacturers.
- It is difficult to find expensive assets without data analysis.
- It is also hard to find unusual rental costs and contract risks. 
- Data analysis can help find ways to reduce costs and improve lease management

This project addresses these challenges by analyzing lease asset information and developing predictive models that estimate monthly rental amounts.

**Main prediction target:** `Asset Rental Expenses`

Reduce Monthly Asset Rental Expenses


The primary objective is to identify the key drivers of rental costs and build models capable of predicting monthly rental expenses.




## Dataset Summary

The analysis is based on an active lease asset report containing asset, contract, vendor, manufacturer, and financial information.

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

## Key Dataset Attributes
- Contract Number
- Vendor Name
- Manufacturer
- Asset Description
- Model Number
- Asset Quantity
- Asset Cost
- Asset Rental Amount
- Asset Rental Tax
- Commencement Date
- Primary Term End Date
- Geographic Location

## Research Questions
This project seeks to answer the following business questions:

1. Which vendors and manufacturers have the highest rental costs? 
2. Which asset types generate the highest monthly rental amounts? 

3. Are there any unusual rental amounts compared to asset costs? 

4. Which factors best predict asset rental amounts? 

5. How can lease costs be reduced and lease management improved?<


## The primary objectives of this project are:

Analyze lease asset financial performance
Identify cost-saving opportunities
Detect rental pricing anomalies
Improve lease data quality
Develop predictive models for rental expenses
Generate actionable business recommendations

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

## Methodology
## Method I: Data Access and Understanding

Activities:

- Load Excel lease asset dataset
- Review data structure
- Analyze column types
- Evaluate missing values
- Define business objectives

Deliverables:

- Dataset summary
- Data quality assessment
- Initial business understanding


### Method II: Exploratory Data Analysis(EDA)

The EDA phase investigates relationships, distributions, and patterns within the lease portfolio.

- Descriptive statistics
- Missing Values by Column
- Asset Distribution by State
- Distribution of Asset Rental Amount
- Asset cost vs Monthly Rental Amount

  
  <img width="1364" height="318" alt="image" src="https://github.com/user-attachments/assets/1586d031-26ae-45a5-94ae-51a5bcc1e1f1" />
  <img width="1930" height="690" alt="image" src="https://github.com/user-attachments/assets/a49b3d1b-5198-4baf-a8f4-631d218d2659" />
<img width="2068" height="818" alt="image" src="https://github.com/user-attachments/assets/a58f6caf-0e2e-417f-bc2e-05ddbe03d38d" />
<img width="2040" height="772" alt="image" src="https://github.com/user-attachments/assets/77434559-2a4f-4159-9e08-e1846e190372" />
<img width="2168" height="788" alt="image" src="https://github.com/user-attachments/assets/d1312fdb-1a2a-463f-bb89-36b5ba852d00" />










### Method III: Prepare Data 

- Clean column names
- Handle missing values
- Create useful features such as rental-to-cost ratio, lease age, and days until primary term end
- Encode categorical variables

  <img width="1330" height="264" alt="image" src="https://github.com/user-attachments/assets/4a9f6e8a-2729-49b2-a62a-da1375f542ca" />




### Method IV: Regression Modeling

Two regression algorithms are used to predict monthly rental amounts.
# Model Evaluated
1. Linear Regression
2. Random Forest Regressor

Used as a baseline model to understand linear regression relationships between features and rental amount.

Random Forest Regressor

Used to capture complex nonlinear relationships and improve prediction accuracy.

Performance Metrics

Model performance is evaluated using:

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² (Coefficient of Determination)
  
<img width="704" height="140" alt="image" src="https://github.com/user-attachments/assets/f795726f-5189-49e8-8cca-7218c5a15869" />

### method V: Model Evaluation and Visualization

Several visualizations are used to assess model performance.

- Actual vs Predicted Rental Amount
- Lease Commencement Trend by Month
- Lease Expiration Trend by Month
- Top 20 Feature Importances

<img width="2154" height="768" alt="image" src="https://github.com/user-attachments/assets/216c5cba-be2b-4516-a220-bfee70deea28" />
 <img width="2040" height="828" alt="image" src="https://github.com/user-attachments/assets/70cec061-4568-4486-901d-c8b54201f726" />
 <img width="2056" height="848" alt="image" src="https://github.com/user-attachments/assets/095378b7-6e55-4d9e-8f34-8c7542f7db1d" />
 <img width="2056" height="764" alt="image" src="https://github.com/user-attachments/assets/bfd703a8-31ff-4a8a-9d79-20b89f2a81dc" />








### Method VI: Business Recommendations
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
- Joblib (library used to save and load Python objects efficiently, especially used in scikit-learn)
- GitHub


## Author

Prakash Ghatani Master in Data Science, Regis University pghatani@regis.edu
