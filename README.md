# Student Performance Data Cleaning in Excel

## Project Overview

This project demonstrates fundamental data cleaning techniques in Microsoft Excel using a real-world student performance dataset from two Portuguese public high schools: **Gabriel Pereira (GP)** and **Mouzinho da Silveira (MS)**.

The project was completed as part of the **Google Data Analytics Certificate** and focuses on improving data quality before analysis. The cleaning process ensures the dataset is accurate, consistent, and suitable for further statistical analysis and visualization.

---

## Dataset

The dataset contains demographic, social, family, and academic information about secondary school students.

The primary objective of this project is to prepare the data for analysis by identifying data quality issues and applying appropriate cleaning techniques.

---

## Project Objectives

The data cleaning process was performed to:

- Identify and remove invalid records
- Handle missing values
- Standardize categorical variables
- Convert text values into numeric representations where appropriate
- Improve overall data consistency and reliability for analysis

---

## Tools Used

- Microsoft Excel
- Sorting
- Filtering
- Find and Replace
- Fill Handle

---

## Data Cleaning Process

### 1. Data Validation

The dataset was sorted by **school** and **age** to identify records containing unrealistic age values.

**Actions Performed:**

- Sorted the dataset by `school` (A–Z) and `age` (Z–A).
- Identified records where student age exceeded the valid high school age range.
- Removed **9 invalid records** (ages 20–22).
- Retained only students aged **15–19 years**.

---

### 2. Handling Missing Values

The **reason** column contained missing values representing the student's reason for choosing a school.

**Actions Performed:**

- Filtered the `reason` column to identify blank cells.
- Replaced missing values with `none_given`.
- Used Excel's **Fill Handle** to populate the missing entries consistently.

---

### 3. Standardizing Categorical Data

The parental education columns (`Medu` and `Fedu`) originally contained descriptive text values.

To make the dataset suitable for quantitative analysis, these values were encoded numerically.

| Education Level | Encoded Value |
|-----------------|--------------:|
| none | 0 |
| primary education | 1 |
| 5th to 9th grade | 2 |
| secondary education | 3 |
| higher education | 4 |

**Actions Performed:**

- Converted text categories into numeric values using **Find and Replace**.
- Verified that both `Medu` and `Fedu` contained only numeric values after transformation.

---

## Data Quality Improvements

After cleaning, the dataset:

- Contains only valid student records.
- Has no missing values in the `reason` column.
- Uses standardized numeric values for parental education.
- Is consistent and ready for statistical analysis and visualization.

---

## Project Files

| File | Description |
|------|-------------|
| `student_data_cleaned.csv` | Cleaned dataset |
| `cleaning_summary.md` | Documentation of the data cleaning process |
| `screenshots/` | Optional screenshots demonstrating the cleaning workflow |

---

## Skills Demonstrated

- Data Cleaning
- Data Validation
- Missing Value Handling
- Data Standardization
- Categorical Data Encoding
- Data Quality Assessment
- Microsoft Excel

---

## Future Work

The cleaned dataset can be used for:

- Exploratory Data Analysis (EDA)
- Data Visualization
- Correlation Analysis
- Regression Modeling
- Student Performance Analysis

---

## Author

**Fazal Haq**

Aspiring Data Analyst | Google Data Analytics Certificate Learner

Pakistan
