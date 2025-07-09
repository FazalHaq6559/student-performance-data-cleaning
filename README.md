# student-performance-data-cleaning
This project is part of the **Google Data Analytics Certificate**. It focuses on cleaning real-world student performance data from two public high schools in Portugal: **Gabriel Pereira (GP)** and **Mouzinho da Silveira (MS)**. The goal is to prepare the dataset for analysis to help the superintendent understand what factors influence student academic performance.

## 🎯 Objective

To clean and prepare the dataset by:
- Removing invalid or incorrect entries (e.g., age above the legal limit)
- Filling in missing values (e.g., unknown reasons for school selection)
- Converting text data into numerical format (for statistical analysis)
- Making the dataset ready for data-driven decision-making


## 🧰 Tools Used

- ✅ **Google Sheets** for data cleaning
- ✅ **Sorting** and **Filtering** for identifying errors
- ✅ **Find and Replace** for transforming text to numbers
- ✅ **Fill Handle** for completing missing values

---

## ✅ Cleaning Steps Overview

### 1. **Sorted Data**
- Sorted by `school` (A–Z) and then by `age` (Z–A)
- Identified students with ages over 19 (not valid for high school)

### 2. **Filtered and Removed Invalid Ages**
- Applied filter to `age` column
- Removed 9 rows with age 20, 21, or 22 (7 from GP, 2 from MS)
- Retained students aged **15–19** only

### 3. **Filled in Missing Data (reason)**
- Filtered `reason` column to show only blank values
- Replaced all blank values with `"none_given"` using the **fill handle**

### 4. **Converted Parent Education Levels to Numbers**
Mapped `Medu` and `Fedu` values as follows:

| Text Description         | Numeric Value |
|--------------------------|----------------|
| none                     | 0              |
| primary education        | 1              |
| 5th to 9th grade         | 2              |
| secondary education      | 3              |
| higher education         | 4              |

- Used **Find & Replace** in Google Sheets to convert values
- Ensured both columns (`Medu`, `Fedu`) now contain numbers only

---

## 📈 Final Outcome

- The dataset is now clean, consistent, and ready for analysis.
- Valid ages (15–19), complete `reason` values, and numeric formats for parental education are in place.
- This prepares the data for deeper analysis on what influences student grades.

---

## 📦 Files for Review

- [`student_data_cleaned.csv`](./data/student_data_cleaned.csv) — Final cleaned dataset
- [`cleaning_summary.md`](./reports/cleaning_summary.md) — All cleaning steps and logic
- Screenshots folder (optional) — Visual documentation of cleaning steps

---

## 📌 Next Steps (optional for future work)

- Perform exploratory data analysis (EDA)
- Run correlation or regression to find links between grades and factors
- Share visual insights with school leadership

---

## 🧑‍🏫 Author

**Fazal Haq**  
Data Analyst | Google Data Analytics Certificate Learner  
🇵🇰 Pakistan

