# 🚗 Car Price Prediction

## Oasis Infobyte Data Science Internship — Task 3

## 📌 Project Overview

This project focuses on predicting the selling price of used cars using Machine Learning techniques.

The dataset contains information about cars such as:

- Car Name
- Manufacturing Year
- Kilometers Driven
- Fuel Type
- Seller Type
- Transmission
- Owner
- Mileage
- Engine
- Maximum Power
- Torque
- Number of Seats

The project includes data cleaning, exploratory data analysis (EDA), feature engineering, model training, and model evaluation.

---

## 🎯 Objectives

- Analyze the used car dataset.
- Clean and preprocess the data.
- Handle missing values and convert relevant columns into numerical format.
- Perform Exploratory Data Analysis (EDA).
- Analyze relationships between car features and selling price.
- Build Machine Learning models for price prediction.
- Compare model performance using evaluation metrics.
- Select the best-performing model.

---

## 📂 Dataset

**Dataset:** Car Details v3

**File:** `Car details v3.csv`

The dataset contains **8,128 records** and **13 columns** before data cleaning.

### Main Features

| Feature | Description |
|---|---|
| `name` | Name of the car |
| `year` | Manufacturing year |
| `selling_price` | Selling price of the car |
| `km_driven` | Kilometers driven |
| `fuel` | Fuel type |
| `seller_type` | Type of seller |
| `transmission` | Transmission type |
| `owner` | Previous owner information |
| `mileage` | Mileage of the car |
| `engine` | Engine capacity |
| `max_power` | Maximum power |
| `torque` | Torque |
| `seats` | Number of seats |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🔍 Project Workflow

### 1. Data Loading

The dataset was loaded using Pandas.

```python
df = pd.read_csv("Car details v3.csv")