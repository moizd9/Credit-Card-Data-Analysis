# Credit Card Consumer Data Analysis and Regression Modeling

## 📋 Project Overview
This project focuses on analyzing consumer credit card data using **Python** on **Google Colab**, followed by building linear and multiple regression models to predict consumer income. The analysis covers exploratory data analysis (EDA), partitioning, correlation testing, and modeling with insights into model performance and limitations.

## 🧠 Key Objectives
- Perform exploratory data analysis on credit card consumer datasets.
- Investigate the relationship between income and number of dependents.
- Build and evaluate single linear regression (SLR) and multiple linear regression (MLR) models.
- Handle multicollinearity and optimize feature selection.
- Evaluate model performance using RMSE and R² on training and validation sets.

## 🛠️ Tools Used
- **Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels)** for data analysis and modeling.
- **Google Colab** for coding, visualization, and documentation.

## 📈 Analysis Highlights
- **Dataset Overview:**  
  - 1,319 records and 13 columns.  
  - Split into 60% training and 40% validation datasets.

- **Exploratory Data Analysis:**  
  - Performed descriptive statistics and visualized income vs. dependents relationship.  
  - Weak but statistically significant positive correlation (r ≈ 0.3572) between income and number of dependents.

- **Single Linear Regression (SLR):**  
  - Built model with dependents as the predictor.  
  - R² ≈ 0.128 indicating a weak relationship.

- **Multiple Linear Regression (MLR):**  
  - Selected predictors: age, dependents, majorcards, and active.
  - Removed `expenditure` due to high correlation with `share` to avoid multicollinearity.
  - Improved model R² to ≈ 0.218 on training data.

- **Model Performance:**  
  - **Training Set:** RMSE = 1.55, R² = 0.218  
  - **Validation Set:** RMSE = 1.49, R² = 0.126  
  - MLR outperformed SLR but still explained a small portion of income variability.

- **Key Insights:**  
  - Dependents have a weak predictive power for income.  
  - Income prediction is limited due to missing critical features like education, industry, and work experience.
