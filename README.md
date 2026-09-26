# 🚗 Car Price Prediction with Machine Learning

A robust machine learning model designed to predict the selling price of used cars based on various vehicle attributes and market features. Developed as part of the **CodeAlpha Machine Learning Internship**.

---

## 📊 Dataset Overview
The dataset contains **301 records** of various car models with the following features:
* **Car_Name**: Name of the car model.
* **Year**: Manufacturing year of the car.
* **Present_Price**: Current ex-showroom price of the car (in lakhs).
* **Selling_Price**: Price at which the car is sold (Target Variable).
* **Driven_kms**: Total distance driven by the car in kilometers.
* **Fuel_Type**: Type of fuel (Petrol, Diesel, CNG).
* **Selling_type**: Dealer or Individual.
* **Transmission**: Manual or Automatic.
* **Owner**: Number of previous owners.

---

## 🛠️ Methodology & Workflow

1. **Data Preprocessing & Cleaning**:
   * Inspected dataset for missing values and data types.
   * Extracted a new feature **`Car_Age`** (`2026 - Year`) to capture vehicle depreciation.
   * Dropped redundant columns (`Year`, `Car_Name`).
2. **Feature Engineering**:
   * Applied **One-Hot Encoding** on categorical variables (`Fuel_Type`, `Selling_type`, `Transmission`) while avoiding multicollinearity (`drop_first=True`).
3. **Model Training**:
   * Trained a **Random Forest Regressor** ensemble model for robust non-linear regression and feature importance handling.
4. **Model Evaluation**:
   * Evaluated performance using **Mean Squared Error (MSE)** and **R-squared ($R^2$) Score**.

---

## 🚀 Tech Stack & Libraries
* **Python** 3.x
* **Pandas & NumPy** (Data manipulation & numerical computations)
* **Matplotlib & Seaborn** (Exploratory Data Analysis & visualization)
* **Scikit-Learn** (Model training, Random Forest Regressor, and evaluation metrics)

---

## ⚙️ Getting Started

### Prerequisites
Make sure you have Python installed along with the required libraries:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn

