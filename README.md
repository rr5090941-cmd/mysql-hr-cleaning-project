 MySQL HR Data Cleaning Project
📄 Project Overview
This project focuses on cleaning, standardizing, and preparing HR employee data using MySQL.
The dataset originally contained multiple issues such as missing values, inconsistent formats, duplicate records, invalid entries, and structural problems.
The goal was to transform the messy HR dataset into a clean, analysis‑ready, and reliable dataset suitable for HR Operations, reporting, and compliance workflows.

🎯 Objectives
Clean and standardize employee data

Remove duplicates and invalid records

Fix inconsistent date formats and text fields

Handle missing values

Validate key HR fields (email, phone, job role, salary, etc.)

Produce a final cleaned dataset for HR reporting

Document the entire SQL workflow for transparency

🗂️ Project Structure
Code
mysql-hr-cleaning-project/
│
├── hr_raw.csv               # Original messy dataset
├── messy_HR_data.csv        # Additional raw HR data
├── hr_clean.csv             # Final cleaned dataset
└── README.md                # Project documentation
🛠️ Tools & Technologies
MySQL (Data cleaning & transformation)

phpMyAdmin / XAMPP (Database management)

Excel / CSV (Raw & cleaned data handling)

GitHub (Version control & documentation)

🔍 Key Data Issues Identified
Duplicate employee records

Inconsistent date formats (DD/MM/YYYY vs YYYY-MM-DD)

Null or missing values in key fields

Incorrect capitalization in names & departments

Invalid email formats

Extra spaces, special characters, and formatting errors

Salary values stored as text

Mixed data types across columns

🧹 Cleaning Steps Performed (SQL)
The cleaning workflow included:

Removing duplicates using ROW_NUMBER()

Standardizing date formats using STR_TO_DATE()

Trimming spaces using TRIM()

Converting text salary fields to numeric

Validating email formats with LIKE patterns

Replacing missing values with defaults or NULL

Normalizing department and job title names

Creating a final cleaned table


📊 Before vs After (Data Quality Improvements)
Before Cleaning
The dataset contained duplicate employee records.

Dates were stored in multiple inconsistent formats.

Many fields had missing or null values.

Email formats were invalid or incorrectly structured.

Names, departments, and job titles had inconsistent capitalization.

Extra spaces, special characters, and formatting issues were common.

Salary values were stored as text instead of numbers.

Overall data quality was too low for HR reporting or analysis.

After Cleaning

All duplicate records were removed.

Dates were standardized into one consistent format.

Missing values were handled or replaced appropriately.

Email formats were corrected and validated.

Text fields were cleaned and properly capitalized.

Extra spaces and unwanted characters were removed.

Salary values were converted into proper numeric types.

The dataset became clean, consistent, and ready for HR reporting and operations


📁 Final Output
The final cleaned dataset is stored in:

Code
hr_clean.csv
This dataset is now ready for:

HR dashboards

Employee reporting

Compliance checks

Attrition analysis

Payroll validation

Workforce planning

🚀 What I Learned
Practical SQL data‑cleaning techniques

Handling real‑world HR data issues

Structuring a data project for GitHub

Improving data quality for HR Operations

Building a portfolio‑ready technical project
