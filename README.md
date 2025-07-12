# Lending Club Loan Data Analysis

## Introduction
This project focuses on analyzing loan application data to identify patterns associated with loan default risk. The objective is to assist a consumer finance company in making informed decisions when approving loans for urban customers. Incorrect loan approvals can result in financial loss, while denying loans to creditworthy applicants may lead to missed business opportunities. By applying exploratory data analysis (EDA), we aim to uncover insights that help minimize lending risks and improve the company’s risk analytics strategy. The analysis will support actions like adjusting loan amounts, interest rates, or rejecting high-risk applications.

## Data Preparation and Cleaning
- **Libraries Used**: Pandas, NumPy, Matplotlib, Seaborn. Warnings were suppressed for cleaner output.
- **Data Loading**: The dataset was loaded using `pd.read_csv()`. Initial observations were made using `.head()`, `.shape`, and `.describe()`.
- **Cleaning Steps**:
  - Removed columns with 100% missing values.
  - Dropped columns with a single unique value.
  - Eliminated customer behavior columns that don't contribute to loan approval decisions.
  - Converted percentage strings to floats for relevant columns.
  - Cleaned categorical data and handled missing values appropriately.

## Exploratory Data Analysis (EDA)
- Conducted univariate analysis on key numerical and categorical features.
- Utilized boxplots to identify and address outliers, especially in the `annual_inc` column.
- Performed bivariate analysis to explore the relationship between loan status and various predictors.
- Created a correlation matrix to identify significant correlations between features and loan default risk.

## Key Findings and Conclusions
1. **Loan Amount and Funding**: Higher loan amounts slightly more associated with defaults.
2. **Interest Rates**: Higher interest rates correlate with an increased likelihood of default.
3. **Employment Length**: Job stability alone is not a strong predictor of default rates.
4. **Home Ownership**: Renters and mortgage holders show higher default rates.
5. **Loan Purpose**: Debt consolidation is common among defaulted loans, indicating potential risk.
6. **State of Residence**: Geographic location impacts default rates, with some states showing higher defaults.
7. **Annual Income and DTI**: Lower annual incomes and higher DTI ratios are prevalent among defaulted loans.

## Recommendations
- Enhance credit risk models to incorporate findings, especially concerning interest rates, loan purposes, and financial health indicators.
- Incorporate geographic location into risk assessment models.
- Encourage additional screening or financial counseling for debt consolidation loan applicants.

## Technologies Used
- **Python** 3.9.12 for scripting.
- **Pandas** 1.4.2 and **NumPy** 1.21.5 for data manipulation.
- **Matplotlib** 3.5.1 and **Seaborn** 0.11.2 for data visualization.
- **Jupyter Notebook** 3.3.2 as the development environment.

## Acknowledgments
- Insights and methodologies were derived from peer analyses and community discussions.
- Utilized Stack Overflow for troubleshooting and optimizing data manipulation techniques.

## Team
- Ravikiran Krishnaprasad
- Amit Kumar
