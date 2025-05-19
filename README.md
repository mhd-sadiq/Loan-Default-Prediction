# Loan Default Prediction Project

This project aims to predict loan default risk using a dataset sourced from Kaggle. The model can help financial institutions assess the creditworthiness of loan applicants and reduce potential losses.

## 📊 Dataset

- **Source**: [Kaggle - Loan Default Dataset](https://www.kaggle.com/datasets/nikhil1e9/loan-default)
- **Features**:
  - `Age`: Age of the borrower
  - `Income`: Annual income of the borrower
  - `LoanAmount`: Total amount of the loan
  - `CreditScore`: A number representing the borrower’s creditworthiness
  - `MonthsEmployed`: Months the borrower has been employed
  - `NumCreditLines`: Number of credit lines the borrower has
  - `InterestRate`: Interest rate on the loan
  - `LoanTerm`: Loan term in months
  - `DTIRatio`: Debt-to-Income Ratio
  - `Education`, `EmploymentType`, `MaritalStatus`, `LoanPurpose`, etc.
  - `Default`: Target variable indicating loan default (Yes/No)

## 🧼 Data Preprocessing

- Dropped unnecessary features like `LoanID`
- Converted categorical variables to numerical (e.g., Education, EmploymentType)
- Created dummy variables for multi-class categorical columns
- Handled data skewness and scaling using `MinMaxScaler`
- Verified no missing or duplicate entries

## 📈 Exploratory Data Analysis

- Value counts and distribution plots for categorical variables
- KDE plots and histograms for numerical features
- Correlation matrix and heatmaps
- Boxplots for outlier analysis

## 🧠 Model Building

- **Algorithm Used**: Logistic Regression
- **Train/Test Split**: 20% training, 80% testing
- **Feature Scaling**: MinMaxScaler

## ✅ Model Evaluation

- **Accuracy**: ~Obtained using `accuracy_score` from scikit-learn
- **Confusion Matrix**: Visualized using Seaborn heatmap

## 📌 Conclusion

This project demonstrates a full pipeline from data loading, preprocessing, visualization, and modeling to evaluation for predicting loan defaults. It can be extended to use more advanced models like Random Forest, XGBoost, or neural networks for better accuracy.

---

