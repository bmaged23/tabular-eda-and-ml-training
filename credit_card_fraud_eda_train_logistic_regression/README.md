# Credit Card Fraud Detection - EDA and Machine Learning

This repository contains a Jupyter Notebook that performs Exploratory Data Analysis (EDA) and builds Machine Learning models on a Credit Card Fraud Detection dataset. The notebook aims to identify fraudulent transactions using various classification algorithms.

## Overview

The notebook includes the following sections:
- **Library Loading:** Importing the necessary libraries for data manipulation, visualization, and modeling.
- **Data Import:** Loading the Credit Card Fraud Detection dataset.
- **Data Exploration:** Inspecting the dataset, handling missing data, and understanding the distribution of fraudulent and non-fraudulent transactions.
- **Data Cleaning:** Preparing the data by handling imbalances and normalizing features.
- **Modeling:** Building and evaluating various Machine Learning models to detect fraudulent transactions.

## Dataset

The dataset used for this analysis is the Credit Card Fraud Detection dataset. The dataset contains transactions made by credit cards in September 2013 by European cardholders. It is highly unbalanced, with the majority of transactions being legitimate. The key attributes include:

- `Time`: The seconds elapsed between this transaction and the first transaction in the dataset.
- `V1` to `V28`: The result of a PCA transformation applied to the original features for confidentiality reasons.
- `Amount`: The transaction amount.
- `Class`: The response variable, where `1` indicates fraud and `0` indicates a legitimate transaction.

### Data Preprocessing

- **Handling Missing Data:** Ensuring there are no missing values in the dataset.
- **Feature Scaling:** Normalizing the `Amount` and `Time` features.
- **Handling Imbalances:** Addressing the class imbalance using techniques like undersampling, oversampling, or SMOTE.

### Exploratory Data Analysis (EDA)

- **Distribution Analysis:** Understanding the distribution of the data, particularly the distribution of fraudulent vs. non-fraudulent transactions.
- **Correlation Analysis:** Analyzing correlations between different features and their relationship with the target variable (fraud vs. non-fraud).

### Modeling

The notebook implements and evaluates several Machine Learning models to detect fraudulent transactions, including:
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **Neural Networks**

Each model's performance is evaluated using metrics such as accuracy, precision, recall, F1-score, and AUC-ROC.

## Requirements

The following Python packages are required to run the notebook:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `tensorflow` (if neural networks are used)

You can install the required packages using `pip`:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow

