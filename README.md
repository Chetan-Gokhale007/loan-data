Loan Data Preprocessing
This repository contains a Jupyter Notebook (.ipynb file) that performs data preprocessing on a loan dataset. The dataset is not included in this repository, but the notebook assumes that it is stored in a file named loan-data.csv in the same directory.

Description
The notebook performs the following tasks:

Imports the loan dataset from a CSV file.
Check for missing values and replace them with a temporary fill value.
Splits the dataset into numeric and string columns.
Reimports the dataset, separating numeric and string columns.
Performs data manipulation on the string columns, including:
Renaming the "issue_d" column to "issue_date".
Converting the "issue_date" column to a numerical format.
Replacing the "loan_status" column with a binary good/bad status.
Replacing the "term" column with a numerical format.
Performs data manipulation on the numeric columns, including:
Converting the "int_rate" column to a percentage format.
Creating new columns for the exchange rate.
Concatenates the numeric and string columns into a single dataset.
Sort the dataset by the "id" column.
Saves the preprocessed dataset to a new CSV file named loan-data-preprocess.csv.
Requirements
Python 3.x
NumPy
Pandas (not explicitly used, but required for some functions)
Usage
Clone this repository to your local machine.
Make sure you have the required libraries installed (Python, NumPy).
Place the loan-data.csv file in the same directory as the notebook.
Open the notebook in Jupyter Notebook or Jupyter Lab.
Run the notebook from top to bottom to perform the data preprocessing.
Notes
The notebook assumes that the loan-data.csv file has a specific structure, with columns in a specific order. If your dataset has a different structure, you may need to modify the notebook accordingly.
The notebook uses a temporary fill value to replace missing values. You may want to modify this value or use a different imputation strategy depending on your specific use case.
