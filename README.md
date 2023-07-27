# Loan Payment Status Prediction

## Project Overview
This project aims to build a machine learning model to accurately predict the future status of a loan payment. The goal is to proactively manage risk, optimize intervention strategies throughout the loan cycle, and minimize potential financial losses.

## Dataset
The dataset used in this project is a historical dataset of loans issued by All Lending Club, including details about the loan amount, term, interest rate, grade, and other relevant information.

## Analysis Steps
1. **Data Loading:** The dataset was loaded into a Python notebook for analysis.
2. **Statistical Summary:** A statistical summary of the dataset was performed using `df.describe()`.
3. **Data Cleaning:** Checked for missing values and duplicates in the dataset. A copy of the original dataframe was created, the `member_id` column was dropped, and other rows with missing values were removed.
4. **Data Distribution:** Checked the distribution of the `loan_amnt` column.
5. **Correlation Analysis:**
   * Initialize a label encoder and convert 'loan_status' to numerical form.
   * Compute the correlation of 'loan_status' with other variables.
   * Sort the correlations and display the sorted correlations.
6. **Data Visualization:**
  * **Pairplot:** We create a pairplot for a subset of columns in the dataset to visualize the pairwise relationships between them. The subset of columns includes 'loan_amnt', 'funded_amnt', 'int_rate', and 'installment'.

  * **Heatmap:** We create a heatmap to visualize the correlation matrix of the dataset. The heatmap helps us understand the linear relationships between different variables in the dataset. We also create a heatmap for the top 10 variables that are most correlated with 'loan_status'.

## Future Work
The next steps of this project will involve feature engineering, model selection, model training, and evaluation of the model's performance.
