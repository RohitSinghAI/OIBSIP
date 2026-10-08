# 📊 Unemployment Analysis in India

## Oasis Infobyte Data Science Internship — Task 2

### 📌 Project Overview

This project analyzes unemployment data in India using Python and
Exploratory Data Analysis (EDA) techniques.

Two unemployment datasets were analyzed in the same Jupyter Notebook
to identify regional, monthly, statistical, COVID-19 related, and
geographical patterns.

---

## 🎯 Objectives

- Analyze unemployment rates across different regions.
- Identify regions with higher average unemployment rates.
- Analyze monthly unemployment trends.
- Compare unemployment conditions before and after COVID-19.
- Study relationships between unemployment, employment, and labour
  participation.
- Visualize the geographical distribution of unemployment observations.
- Extract meaningful insights from the datasets.

---

## 📂 Datasets

### Dataset 1
**File:** `Unemployment in India.csv`

Contains unemployment-related information such as:

- Region
- Date
- Frequency
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Area

### Dataset 2
**File:** `Unemployment_Rate_upto_11_2020.csv`

Contains unemployment-related information along with geographical
coordinates:

- Region
- Date
- Frequency
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Region.1
- Longitude
- Latitude

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🔍 Analysis Performed

### 1. Data Loading
Both datasets were loaded using Pandas.

### 2. Data Cleaning
- Removed completely empty rows.
- Cleaned column names.
- Removed unnecessary spaces from text data.
- Converted dates into datetime format.
- Converted numerical columns into appropriate numeric types.
- Checked missing values.

### 3. Exploratory Data Analysis

The following analysis was performed:

- Dataset shape and structure
- Data types
- Missing value analysis
- Descriptive statistics
- Region-wise average unemployment
- Top 10 regions by unemployment rate
- Monthly unemployment trends
- Top 3 regions time-series analysis
- Correlation analysis
- Correlation heatmap
- Pre-COVID vs Post-COVID comparison
- Geographical distribution using longitude and latitude

---

## 📈 Visualizations

The project includes:

- Top 10 regions bar chart
- Monthly unemployment line chart
- Top 3 regions time-series chart
- Correlation heatmap
- Pre-COVID vs Post-COVID comparison chart
- Geographical unemployment distribution plot

---

## 📊 Dataset Comparison

| Metric | Dataset 1 | Dataset 2 |
|---|---:|---:|
| Records | 740 | 267 |
| Average Unemployment Rate | 11.79% | 12.24% |
| Average Employed | 7.20M | 13.96M |
| Average Labour Participation | 42.63% | 41.68% |

---

## 🔎 Key Findings

- Unemployment rates vary considerably across different regions.
- Monthly analysis shows changes in unemployment rates during 2020.
- Dataset 2 provides additional geographical information through
  longitude and latitude.
- Correlation analysis helps understand relationships between
  unemployment, employment, and labour participation.
- Pre-COVID and Post-COVID analysis provides insight into unemployment
  changes during the COVID-19 period.
- Geographic visualization helps understand the spatial distribution
  of unemployment observations.

---

## 📝 Conclusion

This project demonstrates how Python-based Exploratory Data Analysis
can be used to understand unemployment patterns in India.

Using Pandas, NumPy, Matplotlib, and Seaborn, the project covers data
cleaning, statistical analysis, regional analysis, time-series
analysis, correlation analysis, COVID-19 comparison, and geographical
visualization.

---

## 👨‍💻 Author

**Rohit Singh**

Data Science Intern — Oasis Infobyte

GitHub: RohitSinghAI