# bits-ml-assignment2
This repo will contain all files for bits pilani ml assignment 2
Repo for ML assignment.
Problem statement: Early Stage Diabetes Risk Prediction using following 6 classification models.

Logistic Regression
Decision Tree Classifier
K-Nearest Neighbor Classifier
Naive Bayes Classifier - Gaussian or Multinomial
Ensemble Model - Random Forest
Ensemble Model - XGBoost
Dataset description : https://archive.ics.uci.edu/dataset/529/early+stage+diabetes+risk+prediction+dataset This dataset contains the sign and symptpom data of newly diabetic or would be diabetic patient. Dataset Shape: (520, 16)

Model Performance Comparison (Unified Scale)
The following metrics represent the performance of each model on the test set after advanced preprocessing (Standard Scaling and SMOTE).
ML Model Name	Accuracy	Precision	Recall	F1-Score	AUC	MCC
Random Forest	98.08%	98.10%	99.02%	98.56%	99.45%	96.12%
XGBoost	97.12%	97.15%	98.05%	97.60%	99.10%	94.20%
Decision Tree	96.15%	96.20%	96.15%	96.17%	96.15%	92.30%
kNN	94.23%	93.50%	97.10%	95.27%	98.12%	88.45%
Logistic Regression	93.27%	92.45%	96.08%	94.23%	97.55%	86.50%
Naive Bayes	90.38%	89.20%	94.12%	91.60%	95.30%	81.15%

<img width="742" height="151" alt="image" src="https://github.com/user-attachments/assets/d9c1f822-e6ea-42cb-bddc-f7bbce0f0d9d" />


Model Performance Analysis & Observations
ML Model Name,Performance Level,Key Observations & Clinical Relevance
Random Forest,Highest,"Excellent at capturing non-linear relationships between symptoms like Polyuria and Age. The ensemble nature prevents overfitting, making it the most reliable for diagnosis."
XGBoost,Very High,"Highly efficient. The gradient boosting framework focuses on ""hard to predict"" cases, which is useful for identifying early-stage patients with subtle symptoms."
Decision Tree,High,"Provides a clear ""Decision Path."" For example, it easily identifies that Sudden Weight Loss combined with Polydipsia is a near-certain indicator of risk."
k-Nearest Neighbors,Moderate,"Accuracy improved significantly after Standard Scaling. It relies on patient ""similarity,"" meaning patients with similar symptom clusters are grouped effectively."
Logistic Regression,Stable,"Acts as a strong baseline. Since it uses a linear combination of features, it shows that clinical symptoms have an additive effect on diabetes risk."
Naive Bayes,Baseline,"Fast but slightly less accurate. It assumes symptoms are independent (e.g., Polyphagia doesn't depend on Polyuria), which isn't always true in medical cases."

