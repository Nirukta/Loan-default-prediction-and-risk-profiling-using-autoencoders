# Loan Default Prediction & Risk Profiling

Project Overview:

This project aims to predict the probability of loan default and profile borrowers based on their risk using machine learning.
The dataset used is from Home Credit Default Risk (Kaggle).
The analysis involves:
1. Cleaning and preprocessing the data
2. Handling imbalance using SMOTE
3. Building baseline and advanced models (Logistic Regression, Autoencoder, Hybrid)
4. Performing Risk Profiling using clustering
5. Model interpretability using SHAP and visual analytics

Objective:

1. To identify high-risk loan applicants and assist financial institutions in data-driven credit approval by:
2. Predicting loan default probability
3. Segmenting applicants into Low, Medium, and High Risk profiles

Workflow:

| Step                       | Description                                                    |
| -------------------------- | -------------------------------------------------------------- |
| 1. **Data Preprocessing** | Handle missing values, outliers, irrelevant columns, and types |
| 2. **Feature Engineering** | Create ratios and behavioral flags                             |
| 3. **EDA**                 | Univariate, bivariate, and correlation analysis                |
| 4. **Feature Reduction**   | Remove low-variance and highly correlated columns              |
| 5. **SMOTE**               | Balance default / non-default classes                          |
| 6. **Train-Test Split**    | 80 / 20 stratified split                                       |
| 7. **Logistic Regression** | Baseline interpretable model                                   |
| 8. **Autoencoder**         | Learn latent features, detect anomalies                        |
| 9. **Risk Profiling**      | Cluster latent features into risk segments                     |
| 10. **Hybrid Model**       | Combine autoencoder + supervised features                      |
| 11. **Evaluation**         | AUC, KS, Precision-Recall, ROC                                 |
| 12. **Explainability**     | SHAP-based interpretation & visualization                      |
