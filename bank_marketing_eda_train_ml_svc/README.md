# Bank Marketing Dataset EDA and Machine Learning

This repository contains a Jupyter Notebook that performs Exploratory Data Analysis (EDA) and builds Machine Learning models on the Bank Marketing dataset. The notebook focuses on understanding the data, cleaning it, and developing models to predict whether a client will subscribe to a term deposit.

## Overview

The notebook includes the following sections:
- **Library Loading:** Importing necessary libraries for data manipulation, visualization, and modeling.
- **Data Import:** Downloading and loading the Bank Marketing dataset.
- **Data Exploration:** Inspecting the dataset, identifying unique values, and handling missing data.
- **Data Cleaning:** Removing duplicate rows to ensure data quality.
- **Data Inspection:** Providing an overview of the dataset structure and key statistics.
- **Modeling:** Building and evaluating Machine Learning models to predict client behavior.

## Dataset

The Bank Marketing dataset contains information on a marketing campaign by a Portuguese banking institution. The key attributes include:

- `age`: Age of the client.
- `job`: Type of job.
- `marital`: Marital status.
- `education`: Education level.
- `default`: Has credit in default?
- `housing`: Has housing loan?
- `loan`: Has personal loan?
- `contact`: Type of communication contact (cellular, telephone).
- `month`: Last contact month of year.
- `day_of_week`: Last contact day of the week.
- `duration`: Last contact duration, in seconds.
- `campaign`: Number of contacts performed during this campaign.
- `pdays`: Number of days since the client was last contacted from a previous campaign.
- `previous`: Number of contacts performed before this campaign.
- `poutcome`: Outcome of the previous marketing campaign.
- `emp.var.rate`: Employment variation rate.
- `cons.price.idx`: Consumer price index.
- `cons.conf.idx`: Consumer confidence index.
- `euribor3m`: Euribor 3-month rate.
- `nr.employed`: Number of employees.
- `y`: Has the client subscribed a term deposit?

### Data Preprocessing

- **Handling Missing Data:** Replaced "unknown" values with `NaN` to manage missing data effectively.
- **Removing Duplicates:** Identified and removed duplicate rows to ensure the data's integrity.

### Exploratory Data Analysis (EDA)

- **Data Inspection:** Displayed the first few rows of the dataset and provided a summary of its structure.
- **Handling Categorical Data:** Analyzed and managed categorical data within the dataset.

### Modeling

The notebook implements and evaluates several Machine Learning models to predict whether a client will subscribe to a term deposit, including:
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **Neural Networks**

Each model's performance is evaluated using accuracy, precision, recall, and F1-score.

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

