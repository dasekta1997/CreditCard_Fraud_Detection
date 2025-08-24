💳 Credit Card Fraud Detection


📌 Project Overview
Credit card fraud is a major financial risk for banks and customers. In this project, I am building a machine learning pipeline to detect fraudulent transactions with very high accuracy, recall, and precision.


The project demonstrates:
End-to-end data preprocessing, EDA, feature engineering, and model building.
Handling imbalanced datasets using SMOTE.
Training and comparing multiple ML models (Logistic Regression, Decision Tree, Random Forest, XGBoost, KNN).
Model explainability with SHAP values.
Saving/loading models for production use.
Deriving business insights such as estimated financial savings.


📂 Dataset
Source: creditcard_2023.csv 
[Link Text](https://drive.google.com/file/d/1mdmcWcIacPNqqGGIKMdvjVqhpOf61NUy/view?usp=drive_link)


Features:
28 anonymized features (V1–V28) from PCA transformation.


Amount: Transaction amount.
Class: Target variable (0 = Legit, 1 = Fraud).
Challenge: Severe class imbalance (frauds are <1%).


⚙️ Tech Stack
Languages: Python
Libraries: pandas, numpy, scikit-learn, xgboost, shap, imbalanced-learn, seaborn, matplotlib
Environment: Jupyter Notebook, Google Colab


📊 Exploratory Data Analysis (EDA)
Class distribution (fraud vs non-fraud).
Transaction amount distribution.
Feature correlations with fraud.
Feature importance (Random Forest).
Fraud vs non-fraud distributions for top correlated features.


🤖 Models Trained
Model	              Accuracy	Precision	Recall	F1 Score
Logistic Regression	96.5%	     97.7%	   95.3%	 0.965
Decision Tree	      96.0%	     96.7%	   95.3%	 0.960
Random Forest	      98.6%	     99.8%	   97.4%	 0.986
KNN	                99.1%	     98.2%	   99.9%	 0.991
XGBoost       	    99.9%	     99.8%	   99.9%	 0.999


🔎 Model Explainability
SHAP values show how each feature impacts fraud prediction.
Fraud-prone features (e.g., V4, V11, V2) strongly influence predictions.


📈 Results & Business Insights
Recall (Fraud Detection Rate): 99.27%
False Positive Rate: 0.57%
Estimated Savings: $5.65M per month (assuming $100 average fraud loss).

How to run:
Run Jupyter Notebook:
jupyter notebook
[Link Text](https://drive.google.com/file/d/1DIVrCluwsh3WuhNumnKfKFfln6nOhco6/view?usp=drive_link)
Or
open in Colab with the badge below
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dasekta1997/CreditCard_Fraud_Detection/blob/main/creditcard_2023.ipynb))


📌 Next Steps / Improvements
Deploy as a Flask/FastAPI app for real-time fraud detection.
Integrate with streaming data (Kafka / Spark).
Implement cost-sensitive learning to minimize false positives.


👤 Author
Ekta Das
💼 MIS Executive/Aspired Data Analyst
📫 LinkedIn [Connect with me on LinkedIn](https://www.linkedin.com/in/ektadas97/)
