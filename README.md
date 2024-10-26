## Introduction
This project focuses on predicting Metabolic Syndrome using various machine learning techniques, with an emphasis on 
**explainable artificial intelligence (XAI)** to understand the decision-making processes of the models. The dataset includes 
multiple health-related features, and the goal is to build an accurate classification model while also providing insights into 
why the models produce specific results.

## Aim of the Project
- To develop a predictive model for identifying individuals with Metabolic Syndrome.
- To implement various machine learning techniques, including data preprocessing, exploratory data analysis (EDA), model training, and evaluation.
- To utilize XAI methods such as SHAP and LIME to interpret model predictions and understand the underlying factors influencing the results.

## Code Summary

### 1. Libraries Installation
- Installed necessary libraries for data manipulation, visualization, and machine learning:
  - `catboost`, `pandas-summary`, `optuna`, `pycaret`, `numpy`, `scikit-learn`.

### 2. Data Loading
- Loaded the dataset from a CSV file and displayed its structure and summary statistics.

### 3. Data Preprocessing
- **Null Value Handling**:
  - Filled missing values in 'Income', 'WaistCirc', and 'BMI' with their respective means.
  - Performed label encoding on categorical features: 'Race', 'Sex', and 'Marital'.
  
- **Feature Scaling**:
  - Scaled features using `StandardScaler`.

### 4. Exploratory Data Analysis (EDA)
- Visualized data distributions using boxplots and histograms.
- Analyzed correlations between features using a heatmap.
- Conducted Chi-squared tests for categorical features against the target variable.

### 5. Outlier Detection
- Implemented the IQR method to identify and remove outliers from the dataset.

### 6. Model Training with PyCaret
- Set up the PyCaret environment for classification.
- Compared multiple models based on accuracy and selected the top five.
- Created a stacked ensemble model using XGBoost as the meta-model.

### 7. Model Evaluation
- Evaluated the stacked model using metrics like accuracy score.
- Implemented SHAP (Shapley Additive Explanations) for model interpretability.

### 8. LIME (Local Interpretable Model-agnostic Explanations)
- Used LIME to explain individual predictions by generating local approximations of the model's decision-making process.

### 9. Advanced Modeling Techniques
- Explored bagging, boosting, stacking, and voting classifiers.
- Evaluated each model's performance based on accuracy scores.

### Conclusion
The project successfully implemented a comprehensive pipeline for predicting Metabolic Syndrome while leveraging XAI techniques to 
enhance understanding of model predictions. The final stacked model demonstrated promising accuracy in classifying individuals at risk
of Metabolic Syndrome, with SHAP and LIME providing valuable insights into feature importance and decision rationale.
