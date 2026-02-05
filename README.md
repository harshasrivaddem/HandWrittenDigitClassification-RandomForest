# 🔢 Handwritten Digit Classification using Random Forest

## 📌 Project Overview
This project focuses on **classifying handwritten digits (0–9)** using the **Digits dataset** from scikit-learn and a **Random Forest Classifier**.

Each digit image is represented as an **8×8 grayscale image**, which is flattened into a feature vector.  
The goal is to accurately predict the digit shown in an image based on pixel intensity values.

---

## 📊 Dataset Description
- Dataset: `load_digits()` from scikit-learn
- Total samples: **1,797**
- Image size: **8 × 8 pixels**
- Features: **64 pixel intensity values**
- Target classes: **Digits from 0 to 9**

Each image is flattened into a **64-dimensional vector**.

---

## 🛠️ Tools & Libraries Used
- Python
- Pandas
- Matplotlib
- Scikit-learn

---

## 🔍 Exploratory Data Analysis (EDA)
- Inspected dataset structure and attributes
- Visualized sample digit images using Matplotlib
- Converted pixel data into a Pandas DataFrame
- Added target labels to the dataset

---

## 🤖 Model Building
- **Algorithm:** Random Forest Classifier
- **Train-Test Split:** 80% training, 20% testing
- **Input Features:** 64 pixel intensity values
- **Target Variable:** Digit label (0–9)

Two models were trained:
1. Default Random Forest
2. Random Forest with `n_estimators = 50`

---

## 📈 Model Performance

| Model | Accuracy |
|-----|---------|
| Random Forest (default) | **97.5%** |
| Random Forest (50 estimators) | **97.22%** |

The model demonstrates strong performance in digit classification.

---

## 🔮 Predictions

### Predict a Single Digit
```python
model.predict([digits.data[12]])

