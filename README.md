## Introduction
This project involves exploratory data analysis (EDA) to assess and analyze the risk associated with bank loan applications. The goal is to identify patterns and factors that contribute to loan defaults and to provide insights that could help in risk mitigation.

## Data Description
The dataset used in this analysis is `application_data.csv`, which contains various features related to loan applicants. Key features include:
- `Loan_ID`: Unique identifier for each loan application.
- `Gender`: Gender of the applicant.
- `Married`: Marital status of the applicant.
- `Dependents`: Number of dependents.
- `Education`: Educational level of the applicant.
- `Self_Employed`: Employment status of the applicant.
- `ApplicantIncome`: Income of the applicant.
- `CoapplicantIncome`: Income of the co-applicant (if any).
- `LoanAmount`: Requested loan amount.
- `Loan_Amount_Term`: Term of the loan in months.
- `Credit_History`: Credit history of the applicant.
- `Property_Area`: Area of property (Urban, Semi-Urban, Rural).
- `Loan_Status`: Status of the loan (Y: Approved, N: Not Approved).

## Analysis Steps
The analysis in the notebook follows these main steps:
1. **Data Loading**: Importing necessary libraries and loading the dataset.
2. **Data Inspection**: Exploring the structure and basic statistics of the data.
3. **Data Cleaning**: Handling missing values, outliers, and data inconsistencies.
4. **Exploratory Data Analysis (EDA)**: Visualizing data distributions, relationships, and trends.
5. **Feature Engineering**: Creating new features or modifying existing ones to improve model performance.
6. **Modeling**: Applying machine learning algorithms to predict loan risk (if applicable).

## Results
### Key Insights
Based on the analysis, we have gathered the following insights:

#### People Who Are More Likely to Default
- **Age**: Young people – 25 to 35 age group
- **Income**: Lower income group with a total income of less than 5 lakhs
- **Occupation**: Low-skill laborers, drivers, waiters/barmen staff
- **Education**: Lower / secondary education
- **Gender**: Males
- **Income Type**: On maternity leave and unemployed
- **Family Status**: Civil marriage, single/unmarried
- **Housing Type**: Rented apartment or with parents
- **Contract Type**: Cash loan
- **Cash Loan Purpose**: Repairs and urgent needs
- **Previous Loan Status**: Approved

#### People Who Will Repay on Time
- **Age**: Older people – above 50
- **Income**: Higher income group
- **Occupation**: Managers, high-skilled tech staff, accountants
- **Education**: Higher education and academic degree
- **Gender**: Females
- **Income Type**: Working class, businessmen and students
- **Family Status**: Married
- **Housing Type**: Own house/apartment
- **Contract Type**: Revolving loan
- **Cash Loan Purpose**: Buying garage, home etc.
- **Previous Loan Status**: Unused offer

### Conclusion and Recommendations
- **Deny Loans to High-Risk Applicants**: Young males with lower secondary education, lower income group, staying with parents or in rented houses, and applying for low-range cash contracts should be denied.
- **Adjust Loan Amount for Females on Maternity Leave**: Females are likely to repay but not if they are on maternity leave. Hence, the bank can reduce the loan amount for female applicants who are on maternity leave.
- **Refuse Cash Loans for Repairs and Urgent Needs**: Since people taking cash loans for repairs and urgent needs are more likely to default, the bank can refuse these loans.
- **Higher Interest Rates for High-Income Applicants with Unused Offers**: People with unused offers are more likely to default even though they have comparatively high total income. They can be offered loans at a higher interest rate.
- **Target Low-Risk Segments**: Banks can target businessmen, students, and working-class people with academic degrees/higher education as they have no difficulty in repayment.
- **Approve Loans for Home or Garage Purchases**: Loans taken for buying homes or garages have a lower chance of defaulting and can be approved.

## Dependencies
The project requires the following Python libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `warnings`
