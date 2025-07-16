# -Complete-Case-Analysis-CCA-for-Missing-Data
This Jupyter Notebook demonstrates Complete Case Analysis (CCA) for handling missing data. It analyzes the impact of CCA on dataset size and variable distributions using a data science job dataset, providing insights into this imputation method.

#  Overview & Purpose
This Jupyter Notebook focuses on demonstrating Complete Case Analysis (CCA), also known as listwise deletion, as a method for handling missing data in a dataset. CCA involves removing observations (rows) that have missing values in any of the variables relevant to the analysis. While simple to implement, it's crucial to understand its implications, particularly regarding data loss and potential bias.

# The primary purpose of this notebook is to:
Illustrate CCA Implementation: Provide a clear, step-by-step guide to applying Complete Case Analysis using Python and Pandas.
Analyze Impact on Dataset: Show how CCA affects the overall size of the dataset and the proportion of data retained.
Assess Distribution Preservation: Compare the distributions of key variables before and after applying CCA to determine if the method introduces significant bias or alters the underlying data patterns. This is critical for ensuring the representativeness of the remaining data.

#  Key Concepts & Functionality
The notebook explores the following aspects of CCA:
Data Loading: Imports the data_science_job.csv dataset.
Missing Value Identification: Calculates and displays the percentage of missing values for each column.
Column Selection for CCA: Identifies columns with missing values below a certain threshold (e.g., less than 5%) where CCA might be a viable strategy.
Applying CCA: Creates a new DataFrame by dropping rows that contain missing values in the selected columns.
Data Retention Calculation: Quantifies the percentage of original data retained after performing CCA.
Distribution Comparison: Uses histograms to visually compare the distribution of variables (e.g., training_hours, city_development_index, experience, enrolled_university, education_level) in the original dataset versus the dataset after CCA. This helps to assess if the complete cases are a random subset of the original data.

#  Technologies Used
Python
Pandas (for data manipulation)
NumPy (for numerical operations)
Matplotlib (for data visualization, specifically histograms)
Jupyter Notebook
