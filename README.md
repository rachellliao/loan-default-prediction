# Loan Default Prediction Project

## Project Overview

This project aims to build a machine learning model to accurately predict loan default status based on various features related to the loan and the borrower. The ability to accurately predict loan defaults can add significant business value to lending institutions by enhancing their risk assessment capabilities, improving decision-making processes, and potentially reducing financial losses.

## Dataset

The dataset for this project was obtained from LendingClub, a leading peer-to-peer lending platform based in the United States. Each row of the dataset represents a unique loan and each column represents a different attribute or feature of that loan. These features include loan amount, term, interest rate, grade, sub-grade, employment title, employment length, home ownership, and annual income.

## Project Workflow

### Data Cleaning

The first step was to clean the dataset by removing irrelevant features and handling missing data. Any features that would not be available at the time of issuing the loan (to prevent data leakage) were also removed.

### Exploratory Data Analysis (EDA)

EDA was performed to understand the distribution of different features and their relationship with the loan status. This step helped to inform the choice of appropriate models and guided the feature engineering process.

### Feature Engineering

New features were created from the existing data through one-hot encoding to convert categorical variables into a format that can be provided to machine learning algorithms, which can improve prediction performance.

### Modeling

Several machine learning models were tested, including Logistic Regression, Support Vector Machine, Decision Tree, Random Forest, and XGBoost. Each model was evaluated based on its F1 score, precision, recall, and accuracy. The Random Forest model was selected due to its superior performance.

## Findings and Conclusions

The best performing model achieved an accuracy of approximately 80%, correctly identifying 93% of the loans that were actually paid off. This demonstrates the model's value in providing insights for risk assessment. 

However, there are several areas for potential improvement:

1. **Addressing Class Imbalance:** The dataset had many more loans that were paid off than defaulted. Techniques such as SMOTE or random oversampling could be used to address this imbalance.

2. **Incorporating More Features:** Additional features not included in the current dataset could potentially enhance the predictive power of the model.

3. **Using Different Modeling Techniques:** While the Random Forest model performed best in this project, other techniques such as gradient boosting, neural networks, or ensemble methods could potentially yield better results.

4. **Model Interpretability:** Depending on the needs of the end user, future work could focus on models that balance predictive power with interpretability.

This project demonstrates the practical application of data science techniques in predicting loan defaults and provides valuable insights for risk assessment in lending institutions. Future work will aim to further improve the model's performance and interpretability.


  * **Heatmap:** We create a heatmap to visualize the correlation matrix of the dataset. The heatmap helps us understand the linear relationships between different variables in the dataset. We also create a heatmap for the top 10 variables that are most correlated with 'loan_status'.

## Future Work
The next steps of this project will involve feature engineering, model selection, model training, and evaluation of the model's performance.
