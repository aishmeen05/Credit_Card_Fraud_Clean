# 💳 Credit Card Fraud Detection

This project is a machine learning-based solution to detect fraudulent credit card transactions using a highly imbalanced dataset.

---

## 📂 Dataset

- Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Records: `284,807` transactions
- Fraudulent: `492` (0.17%)
- All features except `Time` and `Amount` are anonymized (`V1` to `V28`) due to confidentiality

---

## 🎯 Objective

To classify whether a given transaction is fraudulent (`Class = 1`) or legitimate (`Class = 0`) using supervised learning.

---

## 📌 Steps Performed

1. **Data Loading & Exploration**
   - Read CSV file using `pandas`
   - Checked class imbalance
   - Analyzed `Amount` distribution for fraud vs. legit

2. **Data Preprocessing**
   - Created a balanced dataset by sampling 492 legit transactions
   - Combined them with all 492 fraud records

3. **Train-Test Split**
   - Used `train_test_split` with stratification (`test_size = 0.2`)

4. **Model Building**
   - Algorithm used: `Logistic Regression` from `sklearn`
   - Trained on balanced dataset

5. **Evaluation**
   - Accuracy on training data: **93.64%**
   - Accuracy on test data: **94.41%**

---

## 📈 Results

| Dataset        | Accuracy    |
|----------------|-------------|
| Training Set   | 93.64%      |
| Test Set       | 94.41%      |

---

## 📦 Technologies Used

- Python
- pandas, numpy
- scikit-learn (LogisticRegression, train_test_split, metrics)

---

## 📝 Notes

- The original dataset is **highly imbalanced**, so random under-sampling was applied for modeling.
- Logistic Regression performed decently, but in real-world scenarios, further models like Random Forest, XGBoost, or deep learning could be used for better performance.

---

## 👩‍💻 Author

**Aishmeen**  
Project Directory: `Credit_Card_Fraud_Clean`  
