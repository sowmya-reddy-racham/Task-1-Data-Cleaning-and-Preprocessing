# Task-1-Data-Cleaning-and-Preprocessing
Data Cleaning and Preprocessing using Excel - Medical Appointment No Shows Dataset
# Task 1: Data Cleaning and Preprocessing using Microsoft Excel

## Objective

The objective of this project was to clean and preprocess the **Medical Appointment No Shows** dataset using **Microsoft Excel**. The dataset was examined for common data quality issues such as missing values, duplicate records, inconsistent formatting, invalid values, and data type inconsistencies to prepare it for further analysis.

---

## Dataset

**Dataset Name:** Medical Appointment No Shows

**Source:** https://www.kaggle.com/datasets/joniarroba/noshowappointments

**Original Dataset Size:**

* Rows: **110,527**
* Columns: **14**

---

## Tools Used

* Microsoft Excel
* GitHub

---

## Dataset Overview

The dataset contains information about medical appointments in Brazil and whether patients attended their scheduled appointments. It includes demographic information, appointment details, and patient health-related attributes.

### Features Included

* Patient ID
* Appointment ID
* Gender
* Scheduled Day
* Appointment Day
* Age
* Neighbourhood
* Scholarship
* Hypertension
* Diabetes
* Alcoholism
* Handicap
* SMS Received
* No-show

---

## Data Cleaning Process

The following data cleaning steps were performed:

### 1. Missing Value Analysis

* Checked all columns using Excel filters.
* No missing values were found in the dataset.

### 2. Duplicate Record Check

* Used Excel's **Remove Duplicates** feature.
* No duplicate records were identified.

### 3. Invalid Data Handling

* Inspected the **Age** column for unrealistic values.
* Identified one record with **Age = -1**.
* Removed the entire row because age cannot be negative.

### 4. Date Standardization

* Converted **ScheduledDay** and **AppointmentDay** from ISO 8601 datetime format to **dd-mm-yyyy** for better readability and consistency.

### 5. Column Name Standardization

Renamed column headers to improve readability and maintain consistency.

Examples:

* PatientId → patient_id
* AppointmentID → appointment_id
* ScheduledDay → scheduled_day
* AppointmentDay → appointment_day
* Hipertension → hypertension
* Handcap → handicap
* No-show → no_show

### 6. Data Validation

* Verified that the **Gender** column contained consistent values (`F` and `M`).
* Verified that the **No-show** column contained consistent values (`Yes` and `No`).
* Confirmed that binary columns contained only valid values (`0` and `1`).

---

## Summary of Cleaning

| Data Cleaning Task | Result                                  |
| ------------------ | --------------------------------------- |
| Missing Values     | No missing values found                 |
| Duplicate Records  | No duplicate records found              |
| Invalid Values     | Removed one record with Age = -1        |
| Date Format        | Converted to dd-mm-yyyy                 |
| Column Headers     | Renamed using lowercase and underscores |
| Categorical Data   | Verified consistent values              |
| Numeric Data       | Validated binary columns                |

---

## Dataset Summary

| Description         | Original | Cleaned |
| ------------------- | -------: | ------: |
| Number of Records   |  110,527 | 110,526 |
| Missing Values      |        0 |       0 |
| Duplicate Records   |        0 |       0 |
| Invalid Age Records |        1 |       0 |

---

## Files Included

* `medical_appointment_raw.csv`
* `medical_appointment_cleaned.xlsx`
* `medical_appointment_cleaned.csv`

---

## Skills Demonstrated

* Data Cleaning
* Data Validation
* Data Preprocessing
* Microsoft Excel
* Missing Value Analysis
* Duplicate Detection
* Date Formatting
* Data Quality Assessment
* Dataset Preparation

---

## Learning Outcomes

Through this project, I learned how to:

* Inspect raw datasets for quality issues.
* Identify and handle invalid data.
* Detect duplicate records.
* Verify missing values.
* Standardize date formats and column names.
* Prepare a clean dataset suitable for analysis and visualization.
* Organize project files and document the cleaning process using GitHub.




Conclusion

This project demonstrates a complete data cleaning workflow using Microsoft Excel. The dataset was validated, cleaned, standardized, and prepared for further analysis by following common data preprocessing practices used in real-world data analytics projects.



