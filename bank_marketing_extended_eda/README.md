# Bank Marketing Dataset - EDA and Machine Learning

This repository contains a Jupyter Notebook that performs Exploratory Data Analysis (EDA) and develops Machine Learning models on the Bank Marketing dataset. The primary objective is to predict whether a client will subscribe to a term deposit based on various attributes related to the client and the marketing campaign.

## Overview

### 1. **Library Loading**
The notebook begins by loading the necessary Python libraries, including:
- `pandas` for data manipulation.
- `numpy` for numerical computations.
- `matplotlib` and `seaborn` for data visualization.
- `scikit-learn` for building and evaluating Machine Learning models.

### 2. **Data Import**
The Bank Marketing dataset is loaded into a pandas DataFrame. This dataset contains information about different marketing campaigns conducted by a Portuguese bank, including details about the clients and their responses to the campaigns.

### 3. **Data Exploration**
In this section, the notebook performs an initial exploration of the data:
- **Dataset Inspection:** Displaying the first few rows of the dataset to understand its structure.
- **Summary Statistics:** Generating summary statistics to get a sense of the data distribution.
- **Missing Values:** Checking for any missing values in the dataset and handling them if necessary.

### 4. **Data Cleaning**
The notebook proceeds to clean the data:
- **Handling Missing Values:** Addressing any missing data to ensure the dataset is complete.
- **Dropping Unnecessary Columns:** Removing columns that do not contribute to the predictive analysis.
- **Feature Engineering:** Creating new features or transforming existing ones to enhance model performance, such as creating age groups or combining similar categories.

### 5. **Exploratory Data Analysis (EDA)**
Detailed exploration of the data is conducted:
- **Target Variable Analysis:** Analyzing the distribution of the target variable (`y`), which indicates whether a client subscribed to a term deposit.
- **Feature Analysis:** Examining how different features like age, job, marital status, and previous contact affect the likelihood of subscription.
- **Visualization:** Using bar plots, histograms, and pair plots to visualize relationships between features and the target variable.
- **Correlation Analysis:** Investigating correlations between features to understand relationships and multicollinearity.

### 6. **Data Preprocessing**
Before building models, the data is preprocessed:
- **Encoding Categorical Variables:** Converting categorical features such as `job`, `marital`, `education`, and `contact` into numerical values using one-hot encoding.
- **Feature Scaling:** Normalizing continuous features such as `age`, `balance`, and `duration` to bring them onto a common scale.

### 7. **Modeling**
The notebook builds and evaluates several Machine Learning models to predict whether a client will subscribe to a term deposit:
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
- **Precision, Recall, and F1-Score:** Metrics to assess the performance of the models in predicting subscription.
- **AUC-ROC Curve:** A curve that provides insight into the trade-off between sensitivity and specificity.
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

