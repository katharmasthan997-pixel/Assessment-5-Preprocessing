Assessment-5 Preprocessing 📊

A Python-based data preprocessing project that analyzes and prepares a diabetes-related patient dataset for further data analysis and machine learning.

This project was developed as part of my Data Science learning journey to practice data loading, data inspection, data cleaning, missing value handling, duplicate removal, outlier handling, categorical encoding, and feature scaling using Python.

---

📌 Project Overview

The Assessment-5 Preprocessing project takes a raw patient dataset and performs different preprocessing techniques to make the data clean, consistent, and ready for machine learning.

The project performs tasks such as:

- Loading and inspecting the dataset
- Understanding rows, columns, and data types
- Identifying numerical and categorical columns
- Renaming columns for better understanding
- Checking unique values in categorical columns
- Generating statistical summaries
- Visualizing numerical data using box plots
- Identifying missing values
- Imputing missing values
- Removing duplicate records
- Handling selected outliers
- Retaining important medical outliers
- Encoding categorical data
- Scaling numerical features
- Preparing the final processed dataset

The main goal is to understand how raw healthcare data can be cleaned and transformed into a useful dataset for further analysis and machine learning.

---

🎯 Objectives

The main objectives of this project are:

- Understand the structure of a real-world dataset.
- Practice data loading and inspection using Pandas.
- Identify numerical and categorical variables.
- Rename unclear column names.
- Validate categorical values.
- Generate statistical summaries.
- Identify and handle missing values.
- Remove duplicate records.
- Understand and handle outliers.
- Preserve medically meaningful outliers where necessary.
- Apply percentile-based outlier filtering.
- Encode categorical variables into numerical form.
- Standardize numerical features.
- Prepare clean data for machine learning.

---

🧹 Data Cleaning

The following data cleaning operations are performed:

Column Renaming

Column names are updated to make them more descriptive:

ID        → Visit_ID
No_Pation → Patient_ID

Categorical Value Checking

The unique values of categorical columns are checked.

Gender:

F → Female
M → Male

CLASS:

N → No Diabetes
P → Pre-diabetes
Y → Diabetes

Unexpected values are reviewed and corrected when required.

Missing Values

Missing values are identified using Pandas and handled using an appropriate method such as:

- Mean
- Median
- Mode

The choice depends on the data type and distribution of the column.

Duplicate Values

Duplicate rows are identified and removed to avoid repeated records affecting the analysis.

---

📊 Statistical Analysis

A statistical summary is generated for numerical columns.

The following values are analyzed:

- Mean
- Median
- Minimum
- Maximum
- Standard Deviation

A box plot is also created to understand the distribution and identify possible outliers.

---

📉 Outlier Handling

Different techniques are used depending on the column.

Outliers Retained

Outliers in the following columns are retained:

- "AGE"
- "HbA1c"
- "BMI"

These values may represent genuine patient measurements and can contain important medical information.

Creatinine Ratio

For the "Cr" column:

- Values above the 99.5th percentile are removed.

Urea

For the "Urea" column:

- Values above the 99.9th percentile are removed.

Lipid Columns

Extreme outliers are handled for:

- "LDL"
- "VLDL"
- "HDL"
- "TG"
- "Chol"

An appropriate method such as IQR or Z-score is used based on the data distribution.

---

🔄 Data Transformation

Gender Encoding

The categorical "Gender" column is converted into numerical form using an encoding technique such as Label Encoding or One-Hot Encoding.

Example:

F → 0
M → 1

This makes the categorical feature suitable for machine learning algorithms.

Feature Scaling

Numerical features with different ranges are standardized.

Examples include:

- "AGE"
- "BMI"
- "Cr"
- Other selected numerical features

Standardization is used because it transforms features to a comparable scale with approximately:

Mean = 0
Standard Deviation = 1

This helps prevent features with larger numerical ranges from having an unnecessary influence on certain machine learning algorithms.

---

🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

---

📂 Project Structure

Assessment-5 Preprocessing
│
├── Assessment_5_Preprocessing.ipynb
├── diabetes_dataset.csv
└── README.md

---

📁 Files Description

File| Description
"Assessment_5_Preprocessing.ipynb"| Jupyter Notebook containing the complete preprocessing process
"diabetes_dataset.csv"| Original/raw dataset
"processed_dataset.csv"| Cleaned and transformed dataset
"README.md"| Project documentation

---

🔍 Preprocessing Workflow

Raw Dataset
     ↓
Data Loading
     ↓
Data Inspection
     ↓
Column Renaming
     ↓
Categorical Value Checking
     ↓
Statistical Analysis
     ↓
Missing Value Handling
     ↓
Duplicate Removal
     ↓
Outlier Handling
     ↓
Gender Encoding
     ↓
Feature Scaling
     ↓
Processed Dataset

---

✅ Final Outcome

After completing the preprocessing steps, the dataset is:

- Cleaned and organized
- Checked for incorrect categorical values
- Processed for missing values
- Free from duplicate records
- Processed according to the specified outlier rules
- Important "AGE", "HbA1c", and "BMI" outliers retained
- Extreme "Cr" and "Urea" values filtered using the required percentile thresholds
- Extreme lipid outliers handled
- Categorical features encoded
- Numerical features standardized
- Ready for further Exploratory Data Analysis (EDA) and Machine Learning

---

🎓 Learning Outcome

Through this project, I practiced important Data Preprocessing concepts including:

- Data loading
- Data inspection
- Data cleaning
- Missing value treatment
- Duplicate handling
- Statistical analysis
- Data visualization
- Outlier detection and handling
- Categorical encoding
- Feature scaling
- Preparing real-world data for machine learning

---

👨‍💻 Project

Project Name: Assessment-5 Preprocessing
Topic: Data Preprocessing
Language: Python
Environment: Jupyter Notebook / Google Colab
