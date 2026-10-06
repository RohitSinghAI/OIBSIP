# Iris Flower Classification

## Oasis Infobyte Data Science Internship — Task 1

### Project Overview

This project focuses on building a machine learning classification model to
predict the species of an iris flower based on its physical measurements.

The three target species are:

- Setosa
- Versicolor
- Virginica

## Objective

The objective of this project is to explore the Iris dataset, perform
exploratory data analysis, train multiple classification models, evaluate
their performance, and identify the best-performing model.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset

The Iris dataset contains measurements of iris flowers.

The features used for classification are:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The target variable represents the iris species.

## Exploratory Data Analysis

The following EDA steps were performed:

- Checked dataset shape
- Checked data types
- Checked missing values
- Generated descriptive statistics
- Analyzed species distribution
- Created pairplots
- Created boxplots
- Discussed feature selection

## Data Preprocessing

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

The training set contained 120 samples, while the testing set contained
30 samples.

## Machine Learning Models

Two classification algorithms were implemented:

### 1. Logistic Regression

Logistic Regression achieved an accuracy of:

**96.67%**

### 2. K-Nearest Neighbors (KNN)

KNN achieved an accuracy of:

**100%**

## Model Comparison

| Model | Accuracy |
|---|---:|
| Logistic Regression | 96.67% |
| KNN | 100% |

Based on the test-set results, KNN performed better than Logistic Regression.

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-Score

## Best Model

Based on the test-set results, **K-Nearest Neighbors (KNN)** was selected as
the best-performing model.

The KNN model correctly classified all 30 samples in the test dataset.

## Conclusion

This project demonstrates how machine learning classification techniques can
be used to classify iris flower species.

After performing exploratory data analysis and training two classification
models, KNN achieved the highest test-set accuracy of 100%, while Logistic
Regression achieved 96.67%.

Therefore, KNN was selected as the best-performing model for this task based
on the test-set results.

## Project Structure

```text
DataScience-Task1-IrisClassification/
│
├── Iris_Classification.ipynb
└── README.md