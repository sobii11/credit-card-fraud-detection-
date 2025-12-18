# 💳 Credit Card Fraud Detection using Machine Learning

## 📌 Project Overview
This project aims to detect fraudulent credit card transactions using machine learning.
Because fraud cases are rare compared to legitimate transactions, the focus is on metrics
that better reflect fraud detection performance rather than overall accuracy.

The main evaluation metrics used is **F1-score**.

---

## 📊 Dataset Description
- The dataset contains credit card transaction data with sender and receiver account IDs, and type of transaction.
- All features are numerical and object.
- Target variable:
  - **0** → Legitimate transaction
  - **1** → Fraudulent transaction
- The dataset is highly imbalanced.

---

## 🔍 Exploratory Data Analysis (EDA)
During the EDA phase, the following steps were performed:
- Inspecting dataset structure and class imbalance
- Visualizing feature distributions
- Analyzing relationships between features and the target variable
- Performing **feature engineering as part of the EDA process** to better understand the data
  and support model training

---

## 🛠️ Data Preparation
The data preparation process included:
- Splitting the data into training and testing sets
- Applying feature scaling where required
- Handling class imbalance using **SMOTE**
- Using pipelines to ensure consistent preprocessing and prevent data leakage

---

## 🤖 Model Training
Multiple machine learning models were trained and compared:
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

Cross-validation was used to compare models based on **F1-score**.

---

## 📈 Model Evaluation
The final model was evaluated on the test set using:
- Recall
- F1-score
- Precision
- Confusion Matrix

Accuracy was not used as the main metric due to the imbalanced nature of the dataset.

---

## 🏆 Final Model Selection
**XGBoost** was selected as the final model due to its strong performance and good balance
between fraud detection and false alarms.

---

## 💾 Model Saving
The final trained pipeline was saved using `joblib` for future use and deployment.

---

## 💼 Business Perspective
In fraud detection:
- Both false negatives and false positives have business impact
- Missing fraudulent transactions leads to financial loss, while false alarms affect customer experience
- The model evaluation focuses on **F1-score** to balance precision and recall
- This balance helps reduce missed fraud cases without generating excessive false alerts
---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## 📂 Repository Structure
credit-card-fraud-detection/
│
├── data/
├── model/
├── fraud_card_project_analysis.ipynb
├── final_fraud_model.pkl
├── requirements.txt
└── README.md

---

## 🚀 How to Run the Project
1. Clone the repository:
   git clone https://github.com/sobii11/credit-card-fraud-detection-
   cd credit-card-fraud-detection-
2. Install dependencies:
   pip install -r Requirements.txt
3. Run the notebook:
   jupyter notebook


---

## 👤 Author
**Sobii**  
Machine Learning & Data Science Enthusiast
