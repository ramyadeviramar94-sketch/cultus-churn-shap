📊 Customer Churn Prediction with SHAP – Interpretable Machine Learning

This project focuses on building an interpretable machine learning model for customer churn prediction using XGBoost and explaining predictions using SHAP (Shapley Additive Explanations).

The goal is not only to achieve high predictive accuracy but also to provide deep insights into why customers churn, helping businesses reduce churn through actionable decisions.


---

🚀 1. Project Objectives

Clean and preprocess the customer churn dataset

Train an advanced ML model (XGBoost)

Generate evaluation metrics

Use SHAP to understand the importance of features

Explain predictions for individual customers

Provide business recommendations based on insights



---

🧠 2. Dataset

The dataset contains customer-level information:

Demographics

Account information

Subscription details

Billing

Service usage

Churn status (Target variable)


File: customer_churn.csv


---

🔧 3. Technologies Used

Python

Pandas

NumPy

Scikit-learn

XGBoost

SHAP

Matplotlib / Seaborn

Google Colab


All required libraries are included in requirements.txt.


---

🛠 4. Steps Performed

✔ 4.1 Data Preprocessing

Handled missing values

Converted categorical variables using OneHotEncoder

Scaled numerical columns

Converted “TotalCharges” to numeric

Removed invalid values

Stratified train-test split


✔ 4.2 Model Training

XGBoost Classifier was used due to:

High performance

Good handling of mixed data types

Works well with SHAP for interpretation


Saved model files:

model.pkl

preprocessor.pkl


✔ 4.3 Model Evaluation

Metrics calculated:

Accuracy

Precision

Recall

F1-score

AUC

Confusion Matrix


(Exact values will come from your notebook output.)


---

🔍 5. SHAP Analysis (Interpretability)

✔ Global Feature Importance

Shows the top factors driving churn across all customers.
File: shap_summary.png

✔ SHAP Bar Plot

Ranks the most important features.
File: shap_bar.png

✔ SHAP Decision Plot

Shows how features push predictions toward churn or non-churn.
File: shap_decision.png

✔ SHAP Force/Waterfall Plot

Explains predictions for individual customers.
File: shap_force_or_waterfall.png


---

👤 6. Individual Customer Analysis

We selected multiple customers to explain:

Why the model predicted churn

Which features increased risk

Which features decreased risk


Examples include explanations such as:

Long-term contracts reduce churn

Electronic check increases churn risk

High monthly charges increase churn

Tenure plays a major role



---

📌 7. Key Insights (Business Recommendations)

🔹 Insight 1: Month-to-Month Customers Are High Risk

📌 Action: Offer discounts or loyalty benefits to convert them to yearly plans.

🔹 Insight 2: High Monthly Charges Customers Churn More

📌 Action: Provide combo/low-cost plans for high-usage customers.

🔹 Insight 3: Electronic Check Users Churn More

📌 Action: Encourage auto-debit or credit card payments.

🔹 Insight 4: Short-Tenure Customers Leave Early

📌 Action: Improve onboarding, deliver value in first 3 months.


---

📂 8. Repository Structure

├── new_customer_churn.ipynb
├── customer_churn.csv
├── model.pkl
├── preprocessor.pkl
├── requirements.txt
├── shap_summary.png
├── shap_bar.png
├── shap_decision.png
├── shap_force_or_waterfall.png
└── README.md


---

📝 9. How to Run the Project

1. Install required libraries:

pip install -r requirements.txt

2. Run the notebook:

Open
new_customer_churn.ipynb
in Jupyter Notebook or Google Colab.

3. View SHAP plots:

All PNG files are inside the repository.


---

🎉 10. Conclusion

This project combines high-performing ML algorithms (XGBoost) with SHAP explainability to give both accuracy + interpretability.
Actionable insights from SHAP help businesses understand:

Why customers churn

Which customers are at high risk

What actions can reduce churn
