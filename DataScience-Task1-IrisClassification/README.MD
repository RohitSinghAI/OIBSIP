# Iris Flower Classification

## Oasis Infobyte Data Science Internship — Task 1

### Objective

The objective of this project is to build a machine learning classification model
that can identify the species of an Iris flower based on its physical measurements.

The three Iris species are:

- Setosa
- Versicolor
- Virginica

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 1. Import Libraries

The required Python libraries were imported for data manipulation,
visualization, and machine learning.

---

## 2. Load Dataset

The Iris dataset was loaded using Scikit-learn's built-in
`load_iris()` dataset.

The dataset contains 150 samples and 4 input features.

---

## 3. Create DataFrame

The dataset was converted into a Pandas DataFrame.

### Features

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

A target column was also added to represent the Iris species.

---

# 4. Exploratory Data Analysis

## 4.1 Dataset Shape

The dataset contains:

- 150 rows
- 5 columns including the target column

## 4.2 Data Types

The data types of all columns were checked to understand the structure
of the dataset.

## 4.3 Missing Values

Missing values were checked using `isnull().sum()`.

The dataset contains no missing values.

## 4.4 Descriptive Statistics

Descriptive statistics were calculated using `describe()` to understand
the distribution of the numerical features.

## 4.5 Species Distribution

The number of samples belonging to each species was checked.

Each species contains 50 samples:

- Setosa: 50
- Versicolor: 50
- Virginica: 50

---

# 5. Data Visualization

## 5.1 Pairplot

A pairplot was created to visualize the relationships between the
different Iris features.

The visualization shows that petal-related features provide better
separation between the three species.

## 5.2 Boxplots

Boxplots were created for all four numerical features to understand
their distributions and identify possible outliers.

## 5.3 Correlation Heatmap

A correlation heatmap was used to understand the relationship between
the numerical features.

Higher correlation values indicate a stronger relationship between
two features.

---

# 6. Feature Selection Discussion

Based on the visualizations, petal length and petal width show clearer
separation between the Iris species compared with the sepal features.

However, all four available features were used for model training so
that the models could learn from the complete dataset.

---

# 7. Train-Test Split

The dataset was divided into training and testing sets.

- Training data: 80%
- Testing data: 20%

`random_state=42` was used to make the split reproducible.

Stratified splitting was also used to maintain the class distribution
across the training and testing datasets.

---

# 8. Model 1 - Logistic Regression

Logistic Regression was implemented as the first classification model.

## 8.1 Prediction

The trained Logistic Regression model was used to predict the species
of the test samples.

## 8.2 Accuracy

Logistic Regression achieved:

**96.67% Test Accuracy**

## 8.3 Confusion Matrix

A confusion matrix was generated to understand the correct and incorrect
predictions for each Iris species.

## 8.4 Classification Report

The classification report was used to evaluate:

- Precision
- Recall
- F1-score
- Support

---

# 9. Model 2 - K-Nearest Neighbors (KNN)

KNN was implemented as the second classification model.

## 9.1 Prediction

The KNN model was trained using `n_neighbors=5` and used to predict
the species of the test samples.

## 9.2 Accuracy

Original KNN achieved:

**100% Test Accuracy**

## 9.3 Confusion Matrix

The KNN confusion matrix showed that all 30 test samples were correctly
classified.

## 9.4 Classification Report

The classification report showed:

- Precision: 1.00
- Recall: 1.00
- F1-score: 1.00

for all three Iris species.

---

# 10. Model Comparison

The initial model results were:

| Model | Test Accuracy |
|---|---:|
| Logistic Regression | 96.67% |
| KNN | 100% |

Based on test accuracy, KNN performed better than Logistic Regression.

---

# 11. Overfitting and Underfitting Check

Training and testing accuracy were compared to identify possible
overfitting or underfitting.

## 11.1 Logistic Regression

The training and testing accuracy were compared to check whether the
model generalizes well to unseen data.

## 11.2 KNN

KNN achieved:

- Training Accuracy: 96.67%
- Testing Accuracy: 100%

The testing accuracy was higher than the training accuracy, so this
result does not show the typical pattern of overfitting.

## 11.3 Cross-Validation

5-Fold Cross-Validation was performed to evaluate model performance
across multiple data splits.

Mean accuracy and standard deviation were calculated to understand
the model's consistency.

---

# 12. Feature Scaling

Feature scaling was tested using `StandardScaler` with KNN.

A Pipeline was used to combine:

1. StandardScaler
2. KNN Classifier

The scaled KNN model achieved:

**93.33% Test Accuracy**

This shows that scaling did not improve the performance of KNN on
this particular Iris test split.

---

# 13. Hyperparameter Tuning

`GridSearchCV` was used to find the best value of `k` for the scaled
KNN model.

Different values of `k` from 1 to 15 were tested using 5-Fold
Cross-Validation.

### Best Parameter

**Best k = 5**

### Best Cross-Validation Accuracy

**96.67%**

### Tuned KNN Test Accuracy

**93.33%**

The tuning process selected `k=5` as the best parameter based on
cross-validation performance.

---

# 14. Best Model Selection

Based on the final test-set results:

- Logistic Regression: 96.67%
- Original KNN: 100%
- Scaled KNN: 93.33%
- Tuned Scaled KNN: 93.33%

Therefore, the **Original KNN model** was selected as the best-performing
model for this classification task based on test-set accuracy.

---

# 15. Final Evaluation

The models were evaluated using:

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-score
- Training vs Testing Accuracy
- 5-Fold Cross-Validation
- Hyperparameter Tuning

The original KNN model achieved the highest test accuracy of:

**100%**

---

# 16. Conclusion

In this project, an Iris Flower Classification system was developed
using machine learning techniques.

The Iris dataset was explored using descriptive statistics, pairplots,
boxplots, and a correlation heatmap.

Two classification algorithms were implemented:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)

The models were evaluated using accuracy, confusion matrix,
classification report, precision, recall, and F1-score.

Additional model validation techniques such as training vs testing
accuracy comparison, 5-Fold Cross-Validation, feature scaling, and
hyperparameter tuning were also performed.

The original KNN model achieved the highest test accuracy of **100%**
and was selected as the best-performing model for this project.

---

## Project Structure

```text
OIBSIP/
│
└── DataScience-Task1-IrisClassification/
    │
    ├── Iris_Classification.ipynb
    └── README.md