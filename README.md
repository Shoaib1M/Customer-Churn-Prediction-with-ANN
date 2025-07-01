# 🧠 Customer Churn Prediction with ANN

This project uses an Artificial Neural Network (ANN) to predict whether a customer will leave a bank, using the **Churn Modelling** dataset. The model is built using TensorFlow and applies preprocessing techniques such as One-Hot Encoding, Label Encoding, Feature Scaling, and Train-Test Splitting.

---

## 📁 Dataset

- File: `Churn_Modelling.csv`
- **Target**: `Exited` (1 = Customer left, 0 = Customer stayed)
- Key Features used:
  - Geography
  - Gender
  - Age
  - Tenure
  - Balance
  - Credit Score
  - Number of Products
  - Has Credit Card
  - Is Active Member
  - Estimated Salary

---

## ⚙️ Features

- ✅ Label Encoding (`Gender`)
- ✅ One-Hot Encoding (`Geography`)
- ✅ Feature Scaling (StandardScaler)
- ✅ Binary classification using a Sequential ANN model
- ✅ Evaluation via confusion matrix and accuracy score

---

## 🧪 Model Architecture

```python
model = Sequential()
model.add(Dense(units=6, activation='relu'))
model.add(Dense(units=6, activation='relu'))
model.add(Dense(units=1, activation='sigmoid'))
```

Loss function: binary_crossentropy

Optimizer: adam

Epochs: 100

Batch size: 32

📊 Results

✅ Final Accuracy: ~86%

✅ Confusion Matrix & Evaluation printed after prediction

