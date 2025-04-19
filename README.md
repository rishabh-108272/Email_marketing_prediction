# Email_marketing_prediction
This project focuses on email classification and analysis using machine learning techniques. The goal is to effectively identify and maximize the probability of click through rates of the links in the emails.

#Methodology
# Email Campaign Analysis Steps

## 1. Data Preparation
- Merge email sent, opened, and clicked tables
- Create binary flags: `opened` and `clicked` columns

## 2. Key Metrics Calculation
- Calculate overall:
  - Open Rate (Opened/Sent)
  - Click-Through Rate - CTR (Clicked/Sent)
  - Click-to-Open Rate - CTOR (Clicked/Opened)

## 3. Segmented Performance Analysis
- Break down metrics by:
  - Email content (long vs short)
  - Version (personalized vs generic)
  - Weekday and time binned
  - User country
  - Past purchase tiers (0, 1-3, 4+)

## 4. Predictive Modeling
- Build classification model predicting clicks
- Preprocess categorical features (one-hot encoding)
- Test models: Logistic Regression → Random Forest/XGBoost
- Evaluate with ROC-AUC, precision-recall metrics

## 5. A/B Testing Framework
- Design controlled experiment:
  - Control group: Business-as-usual targeting
  - Treatment group: Model-recommended targeting
- Use statistical tests to validate results

## 6. Visualization
- Create plots showing:
  - top features contributing in making predictions.
  - Using Explainable machine learning library SHAP, we analyzed how the top features are creating the impact in making predictions.

