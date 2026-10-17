# Exploratory Data Analysis & Classical Machine Learning

A collection of seven historical Python learning notebooks by **Bola Maged Ramses Nessim**, covering tabular exploration, preprocessing, classification and regression. These complement my newer speech, computer-vision and agentic-AI applications by showing earlier work with data and conventional ML.

## Explore the notebooks

| Analysis | Folder |
| --- | --- |
| [Titanic survival](EDA_1/EDA_and_ML_for_titanic_dataset_.ipynb) | `EDA_1` |
| [Breast cancer classification](EDA_2/EDA_and_ML_for_breast_cancer_dataset.ipynb) | `EDA_2` |
| [Diamond price regression](EDA_3/EDA_EDA_and_ML_for_diamonds_dataset_ipynb.ipynb) | `EDA_3` |
| [Bank marketing classification](EDA_4/EDA_EDA_and_ML_for_bank_marketing_dataset_ipynb.ipynb) | `EDA_4` |
| [Credit-card fraud detection](EDA_5/EDA_ML_creditcardfraud_dataset.ipynb) | `EDA_5` |
| [Insurance cost analysis](EDA_6/EDA_ML_form_scratch_insurance_dataset_.ipynb) | `EDA_6` |
| [Bank marketing: extended exploration](EDA_7/Bank_Marketing_Dataset_EDA_Notebook(Python_For_AI).ipynb) | `EDA_7` |

Start with the fraud notebook for imbalanced classification, diamonds for regression, and insurance for exploratory/statistical analysis. These are learning examples, not validated clinical, financial or forecasting systems.

## Methods visible in the collection

Pandas/NumPy data inspection; duplicate and missing-value handling; distributions, box plots and correlation heatmaps; categorical encoding and scaling; scikit-learn classification/regression; and statistical tests in the insurance analysis. Methods vary by notebook—no single notebook implements every method.

## Open and run

Browse the rendered `.ipynb` files on GitHub or use their corrected **Open in Colab** badges. Original notebooks expect dataset ZIPs under `/content/` and read extracted CSVs from those paths. Obtain the appropriate source data, inspect the relevant notebook's first cells, and adjust paths and CSV delimiters before running.

For local exploration, use an isolated Python environment and Jupyter with NumPy, Pandas, Matplotlib, Seaborn, SciPy and scikit-learn. This repository does not provide a validated dependency lock or all source datasets; do not assume a clean top-to-bottom run without adapting the original Colab setup.

## Evaluation and reproducibility

Saved notebook outputs are historical, not a newly reproduced benchmark. Some notebooks perform scaling or other preprocessing before splitting, which can leak information into evaluation. The Titanic notebook also includes an invalid intermediate indexing expression, and original data paths must be adapted. No accuracy/F1 result is promoted as independently validated in this README.

Before using results in an application or CV: repair execution order, fit learned transformations only on training data, reserve validation/test sets, and verify class balance and appropriate metrics. For fraud, report precision/recall, F1 and PR-AUC rather than accuracy alone. For regression, report MAE/RMSE alongside R². Record dataset provenance and redistribution rights before adding data files.

The existing per-folder notes and original notebook outputs are retained for context; they may describe historical experiments rather than current, verified performance.
