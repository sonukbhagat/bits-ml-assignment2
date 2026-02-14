# bits-ml-assignment2
This repo will contain all files for bits pilani ml assignment 2

Problem statement:
The objective of this project is to develop a robust machine learning system for the early-stage identification of diabetes risk using clinical and lifestyle data . Diabetes is a chronic condition that, if left undetected, can lead to severe complications. By implementing and comparing six distinct classification algorithms—Logistic Regression, Decision Tree, kNN, Naive Bayes, Random Forest, and XGBoost—this study aims to identify the most reliable predictive model . The final solution provides an interactive diagnostic dashboard where medical practitioners can upload test data and analyze performance through standardized evaluation metrics, ensuring an end-to-end clinical decision-support workflow

Dataset description : https://archive.ics.uci.edu/dataset/529/early+stage+diabetes+risk+prediction+dataset 
The dataset used for this assignment is the Early Stage Diabetes Risk Prediction Dataset, sourced from the UCI Machine Learning Repository.
Target Task: Binary classification to predict whether a patient is at risk of diabetes (Positive/Negative).
Instance Size: 520 instances.
Feature Size: 16 clinical features (including Age, Gender, Polyuria, Polydipsia, etc.).

Preprocessing: Categorical variables were encoded using Label Encoding, and numerical features were standardized using a Scaler to ensure model stability.

Models Used: Comparison Table
The following table summarizes the evaluation metrics calculated for all 6 mandatory classification models . These results were obtained using a balanced test set to ensure metric reliability.

<img width="603" height="246" alt="image" src="https://github.com/user-attachments/assets/383ffb86-07b8-479a-98dc-af1f4b3ad6a7" />

Model Performance Observations
<img width="691" height="364" alt="image" src="https://github.com/user-attachments/assets/6a12eda5-b701-40d1-b120-631048be04da" />
Based on the experimental results above, the following observations are noted:
Top Performer: Random Forest achieved perfect scores across all metrics (1.0000), indicating it successfully captured all patterns within this specific clinical dataset without overfitting during this evaluation.
Tree-Based Dominance: Both Random Forest and Decision Tree outperformed linear and probabilistic models, suggesting that the underlying symptoms of diabetes in this dataset have strong non-linear decision boundaries.
Precision vs. Recall: kNN achieved a perfect Precision (1.0000) but a lower Recall (0.8333). In a medical context, this means while it never misidentifies a healthy person as diabetic, it misses roughly 16% of at-risk patients.
Stability: XGBoost and Logistic Regression showed very high AUC scores (>0.99), demonstrating strong discriminatory power between the risk classes.
