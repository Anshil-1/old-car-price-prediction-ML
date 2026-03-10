# 🚗 Predicting Old Car Prices Using Supervised Machine Learning

## 📌 Project Overview

This project predicts the **resale price of old cars** using **Supervised Machine Learning (Regression)** in Python. It demonstrates an **end-to-end ML workflow** including data loading, cleaning, exploratory data analysis (EDA), feature engineering, model training, evaluation, and final price prediction.



---

## 🎯 Problem Statement

Used car prices depend on factors like **manufacturing year, mileage, fuel type, transmission, ownership, and present price**. The objective is to build a regression model that accurately predicts the **Selling_Price** based on these features.

---

## 🧠 Machine Learning Details

* **Learning Type:** Supervised Learning
* **Problem Type:** Regression
* **Target Variable:** `Selling_Price`

---

## 📊 Dataset Description

The dataset contains historical used-car records with the following features:

| Feature       | Description               |
| ------------- | ------------------------- |
| Car_Name      | Name of the car           |
| Year          | Manufacturing year        |
| Present_Price | Current showroom price    |
| Kms_Driven    | Total kilometers driven   |
| Fuel_Type     | Petrol / Diesel / CNG     |
| Seller_Type   | Dealer / Individual       |
| Transmission  | Manual / Automatic        |
| Owner         | Number of previous owners |
| Selling_Price | **Target variable**       |

---

## 🛠️ Tools & Technologies

* **Python**
* **Pandas, NumPy** – Data manipulation
* **Matplotlib, Seaborn** – Data visualization
* **Scikit-learn** – Machine learning models
* **Jupyter Notebook**
* **GitHub** – Version control

---

## 🔍 Project Workflow

### 1️⃣ Data Loading & Understanding

* Loaded CSV data using Pandas
* Checked shape, data types, and summary statistics

### 2️⃣ Data Cleaning

* Handled missing values
* Removed unnecessary columns

### 3️⃣ Exploratory Data Analysis (EDA)

* Analyzed price distribution
* Studied relationships (Year vs Price, Fuel Type vs Price)
* Identified key price drivers

### 4️⃣ Feature Engineering

* Converted categorical variables using **One-Hot Encoding**
* Applied **StandardScaler** for feature scaling

### 5️⃣ Model Training

* Linear Regression (baseline)
* Random Forest Regressor (final model)

### 6️⃣ Model Evaluation

* **R² Score**
* **MAE** (Mean Absolute Error)
* **RMSE** (Root Mean Squared Error)

### 7️⃣ Prediction

* Predicted selling price for new/unseen car inputs

---

## 📈 Results Summary

| Model                   | Performance                        |
| ----------------------- | ---------------------------------- |
| Linear Regression       | Baseline performance               |
| Random Forest Regressor | **Best accuracy and lowest error** |

**Conclusion:** Random Forest outperformed Linear Regression and was selected as the final model.

---

## 💡 Key Insights

* Newer cars generally have higher resale value
* Lower mileage cars retain more value
* Fuel type and transmission impact resale price
* Ownership count significantly affects price

---

## 🧪 Sample Prediction Code

```python
input_df = pd.DataFrame([[2018, 5.5, 35000, 1, 0, 1, 0, 0]], columns=X.columns)
input_scaled = scaler.transform(input_df)
rf_model.predict(input_scaled)
```

---

## 📸 Screenshots

Add
