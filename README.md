🛡️ Credit Card Fraud Detection - Machine Learning Project
📌 Project Overview
The goal of this project is to analyze the "Credit Card Fraud Detection" dataset available on Kaggle and develop a predictive model capable of identifying fraudulent credit card transactions.

The dataset is highly imbalanced, which makes fraud detection a non-trivial classification task. Therefore, special attention has been given to evaluation metrics and data balancing techniques.

📊 Dataset Summary
Records: 284,807 transactions

Features: 30 anonymized features resulting from a prior PCA transformation (plus Time and Amount)

Label: Class (0 = legitimate, 1 = fraud)

Imbalance: Fraudulent transactions represent only ~0.17% of the total

🔍 Exploratory Data Analysis (EDA)
The EDA phase included:

Distribution analysis of Amount and Time

Label imbalance visualization

Correlation heatmap to detect any underlying structure in the PCA features

Detection of outliers and unusual patterns

⚖️ Handling Class Imbalance
Given the strong imbalance, naive models tend to be biased toward the majority class (legitimate transactions).
To mitigate this issue, we applied:

Controlled undersampling: reducing the number of majority class samples to balance the dataset

🤖 Models Used
We trained and evaluated several classification models:

Logistic Regression

k-Nearest Neighbors (kNN)

Random Forest

Each model was trained on both the original and the balanced dataset.

📈 Evaluation Metrics
Accuracy alone is not suitable due to class imbalance.
We focused on more informative metrics:

Precision

Recall

F1-score

ROC-AUC

These metrics better capture the trade-off between false positives and false negatives.

🛠️ Tools & Libraries
Python 3.x

pandas, numpy

matplotlib, seaborn

scikit-learn

🚀 How to Run
Clone the repository

Install the required libraries (see requirements.txt if available)

Run the Jupyter Notebook fraud_detection.ipynb step by step


📎 Dataset
Dataset link: Credit Card Fraud Detection on Kaggle
