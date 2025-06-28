# 🧠 Customer Churn Prediction using ANN

This project predicts whether a customer will churn (i.e., stop using a service) using an Artificial Neural Network (ANN). It is built using Python and provides a simple and interactive frontend using Streamlit.

---

## 📌 Overview

Churn prediction helps companies retain customers by identifying potential dropouts early. This project trains an ANN model on structured customer data and presents the prediction results via a user-friendly Streamlit app.

---

## 🔍 Features Used

| **Feature**       | **Description**                                 | **Possible Influence on Churn**                                      |
| ----------------- | ----------------------------------------------- | -------------------------------------------------------------------- |
| `CreditScore`     | Creditworthiness of the customer                | Lower scores may indicate higher risk of churn                       |
| `Geography`       | Country of the customer (e.g., France, Spain)   | Churn rates may vary by region due to market factors                 |
| `Gender`          | Gender of the customer                          | Sometimes included, but usually low influence on churn               |
| `Age`             | Age of the customer                             | Older or very young customers may have higher churn risk             |
| `Tenure`          | How long the customer has been with the company | Shorter tenure can indicate a higher chance of churn                 |
| `Balance`         | Account balance                                 | Zero balance or very high balance could both affect churn likelihood |
| `NumOfProducts`   | Number of products/services used                | Fewer products often correlates with higher churn                    |
| `HasCrCard`       | Whether the customer has a credit card (0 or 1) | Slight influence; not always significant                             |
| `IsActiveMember`  | Whether the customer is actively using services | Very important — inactive users are more likely to churn             |
| `EstimatedSalary` | Income level of the customer                    | May influence churn depending on affordability                       |

---

## 🧰 Tech Stack

- **Frontend**: [Streamlit](w) 
- **Backend**: [Python](w)
- **Modeling**: [TensorFlow](w), [Keras](w) (for ANN), [Scikit-learn](w)
- **Data Handling**: [Pandas](w), [NumPy](w)

---

## 🧠 Model

The classification model is an **Artificial Neural Network (ANN)** with:

- Input layer: 10 features
- Hidden layers: Dense layers with ReLU activation
- Output layer: ReLU activation(> 0.5 is True)

Trained using `binary_crossentropy` loss and `Adam` optimizer.

---

## ⚙️ How to Run Locally

```bash
git clone https://github.com/yourusername/customer-churn-prediction.git
cd customer-churn-prediction
pip install -r requirements.txt
streamlit run app.py
