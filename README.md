
# SWYNEX – Data Cleaning & Preparation

## Project Overview

This project was completed as part of the SWYNEX Technologies Data Cleaning & Preparation task.

The objective is to identify and resolve common data quality issues such as missing values, duplicate records, invalid values, inconsistent formats, and data type issues using Microsoft Excel.

## Dataset

Dataset: Telecom Customer Churn & Data Quality Dataset

The dataset contains customer information, monthly usage data, and churn labels.

### Files

- `cleaned_customer_info.csv` – Cleaned customer demographic and subscription information
- `cleaned_usage_data.csv` – Cleaned monthly customer usage information
- `cleaned_churn_labels.csv` – Cleaned customer churn labels

## Data Cleaning Performed

### 1. Missing Values

- Identified missing values in the customer information dataset.
- Missing Age values were handled using the median age.
- Median age used for imputation: **43**
- Verified that missing Age values were reduced to zero.

### 2. Duplicate Records

- Checked datasets for duplicate records.
- Duplicate CustomerID records were identified in the customer information dataset.
- **200 duplicate records** were removed.
- Usage data and churn labels were also checked for duplicate records.

### 3. Invalid Values

- Negative MonthlyCharges values were identified.
- Since monthly charges cannot logically be negative, the invalid values were replaced using the median MonthlyCharges value.
- Median MonthlyCharges used: **50.07**

### 4. Data Type and Format Validation

- Verified numeric fields such as Age, MonthlyCharges, CallMinutes, DataUsageGB, SMSCount, and Complaints.
- Verified Month/SignupDate fields as date values.
- Verified Churn values as binary values (`0` and `1`).

### 5. Consistency Checks

The following categorical fields were checked for consistent values:

- Gender
- Region
- ContractType
- Churn

## Tools Used

- Microsoft Excel
- GitHub
- CSV

## Before and After Summary

| Data Quality Issue | Before Cleaning | After Cleaning |

| Missing Age Values | 3584 | 0 |
| Duplicate Customer Records | 200 | 0 |
| Negative MonthlyCharges | 5 | 0 |
| Invalid Churn Values | 0 | 0 |

## Outcome

The datasets were cleaned and validated to improve data quality, consistency, and readiness for further analysis.

The cleaned datasets are available in this repository.

## Author

Sebastin Naveen Kumar
