 Loan Eligibility Prediction

This repository contains the code and analysis for predicting loan eligibility using machine learning techniques. The dataset used includes demographic and financial information of applicants and aims to determine the probability of loan approval.

 Project Overview

The goal of this project is to predict whether a loan will be approved based on various features such as applicant income, loan amount, credit history, and more.

 Dataset

The dataset contains 614 records and 13 features:
- Loan_ID: Unique identifier for each applicant
- Gender: Gender of the applicant
- Married: Marital status
- Dependents: Number of dependents
- Education: Educational background (Graduate/Non-Graduate)
- Self_Employed: Whether the applicant is self-employed
- ApplicantIncome: Income of the applicant
- CoapplicantIncome: Income of the coapplicant (if any)
- LoanAmount: Loan amount requested
- Loan_Amount_Term: Term of the loan (in months)
- Credit_History: History of credit repayment (1: good, 0: bad)
- Property_Area: Area where the property is located (Urban, Semiurban, Rural)
- Loan_Status: Target variable indicating loan approval status (Y/N)

 Methods

1. Data Preprocessing
   - Handled missing values using mean imputation for numerical features (LoanAmount, Loan_Amount_Term) and mode imputation for categorical features (Gender, Married).
   - Converted categorical variables such as Gender, Education, and Property_Area into numerical format using one-hot encoding.

2. Exploratory Data Analysis (EDA)
   - Visualized relationships between key features and loan status.
   - Assessed correlations to determine the impact of ApplicantIncome, Credit_History, and other features on loan approval.

3. Modeling
   - Built classification models using:
     - Logistic Regression
     - Decision Tree Classifier
   - Evaluated model performance using accuracy and confusion matrix.
   - Achieved an accuracy of 80% using Logistic Regression and 78% using Decision Trees.

 How to Use

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/loan-eligibility-prediction.git
    cd loan-eligibility-prediction
    ```

2. Install required libraries:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Jupyter notebook for data preprocessing, model building, and predictions:
    ```bash
    jupyter notebook Loan_Eligibility_Prediction.ipynb
    ```

 Results

- Decision Tree model achieved an accuracy of 80%.
- Feature importance analysis showed that Credit History and ApplicantIncome were the strongest predictors of loan approval.

 Conclusion

The project demonstrates the use of machine learning to predict loan eligibility based on applicant data. Logistic Regression performed best, indicating that the problem is linearly separable with the selected features.
