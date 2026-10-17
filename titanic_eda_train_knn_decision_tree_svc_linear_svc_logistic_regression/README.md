# Titanic Dataset - EDA and Machine Learning

This repository contains a Jupyter Notebook that performs Exploratory Data Analysis (EDA) and develops Machine Learning models on the Titanic dataset. The main objective is to predict the survival of passengers based on various features like age, gender, class, and more.

## Overview

### 1. **Library Loading**
The notebook starts by importing the necessary Python libraries, including:
- `pandas` for data manipulation.
- `numpy` for numerical computations.
- `matplotlib` and `seaborn` for data visualization.
- `scikit-learn` for building and evaluating Machine Learning models.

### 2. **Data Import**
The Titanic dataset is loaded into a pandas DataFrame. This dataset contains information about the passengers, including whether they survived or not.

### 3. **Data Exploration**
In this section, the notebook performs an initial exploration of the data:
- **Dataset Inspection:** Displaying the first few rows of the dataset to understand its structure.
- **Summary Statistics:** Generating summary statistics to get a sense of the data distribution.
- **Missing Values:** Identifying and analyzing missing values in the dataset, particularly in columns like `Age`, `Cabin`, and `Embarked`.

### 4. **Data Cleaning**
The notebook proceeds to clean the data:
- **Handling Missing Values:** Missing values are handled by various methods, such as imputing the median age for missing `Age` values, and filling missing `Embarked` values with the most common port.
- **Dropping Unnecessary Columns:** Columns like `PassengerId`, `Ticket`, and `Cabin` are dropped as they do not provide significant value for predicting survival.
- **Feature Engineering:** Creating new features like `FamilySize` (combining `SibSp` and `Parch`) and `IsAlone` to capture additional relationships.

### 5. **Exploratory Data Analysis (EDA)**
Detailed exploration of the data is conducted:
- **Survival Rate Analysis:** Analyzing survival rates across different groups such as gender, class, and age.
- **Visualization:** Using bar plots, histograms, and box plots to visualize relationships between features and survival.
- **Correlation Analysis:** Investigating correlations between features to understand their relationships.

### 6. **Data Preprocessing**
Before building models, the data is preprocessed:
- **Encoding Categorical Variables:** Converting categorical features like `Sex` and `Embarked` into numerical values using one-hot encoding.
- **Feature Scaling:** Normalizing continuous features such as `Age` and `Fare` to bring them onto a common scale.

### 7. **Modeling**
The notebook builds and evaluates several Machine Learning models to predict passenger survival:
- **Logistic Regression:** A baseline model used for binary classification.
- **Decision Tree:** A model that captures non-linear relationships in the data.
- **Random Forest:** An ensemble method that averages multiple decision trees to improve accuracy.
- **Support Vector Machine (SVM):** A model that finds the optimal boundary between classes.
- **K-Nearest Neighbors (KNN):** A model that classifies based on the majority vote of nearest neighbors.
- **Neural Networks:** A more complex model used to capture deeper patterns in the data.

### 8. **Model Evaluation**
Each model is evaluated using various metrics:
- **Accuracy:** The proportion of correctly classified instances.
- **Confusion Matrix:** A matrix to visualize true positives, false positives, true negatives, and false negatives.
- **Precision, Recall, and F1-Score:** Metrics to assess the performance of the models in classifying survival.
- **Cross-Validation:** A technique to ensure the model’s performance generalizes well to unseen data.

### 9. **Hyperparameter Tuning**
The notebook also explores hyperparameter tuning to optimize the models:
- **Grid Search:** Used to find the best combination of hyperparameters for each model.

## Requirements

To run the notebook, you'll need the following Python packages:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `tensorflow` (if neural networks are used)

You can install the required packages using `pip`:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
