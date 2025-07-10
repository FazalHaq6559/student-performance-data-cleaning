# 🧹 Data Cleaning Summary

This document outlines all the steps I took to clean the **Student Performance** dataset using **Google Sheets**. The cleaning process ensures the data is accurate, complete, and ready for analysis as part of the Google Data Analytics Certificate program.

---

## 🔍 Columns Focused On

- `school`: The school each student attends (GP or MS)
- `age`: Student's age
- `reason`: Reason for choosing the school
- `Medu`: Mother's education level
- `Fedu`: Father's education level

---

## 🧼 Step-by-Step Cleaning Process

### ✅ Step 1: Sorted the Data

**Why:** To better understand data distribution and spot unusual values.

- Selected the entire dataset
- Applied sorting by:
  - `school` (A → Z)
  - then `age` (Z → A)
- Observed some students were aged **20, 21, 22**, which is above the legal high school age limit in Portugal

---

### ❌ Step 2: Filtered and Removed Invalid Ages

**Why:** The superintendent confirmed that public high school age should range from **15 to 19**.

- Applied filter on `age` column
- Displayed only students aged **20, 21, and 22**
- Identified **9 rows** outside the valid range
- Deleted those 9 rows
- Turned off filter and confirmed age column now only includes valid ages (15–19)

---

### ✏️ Step 3: Filled in Missing Values in `reason` Column

**Why:** The `reason` column helps explain why students chose a specific school—an important factor in performance.

- Applied a filter to the `reason` column
- Isolated rows with **blank cells**
- Replaced all blanks with the label: `none_given`
- Used the **fill handle** to quickly populate all blank rows with this value
- Turned off filter and verified the column is now complete

---

### 🔢 Step 4: Converted Text to Numbers in `Medu` and `Fedu`

**Why:** Text values need to be numeric for statistical analysis or machine learning.

Used **Find & Replace** on both `Medu` and `Fedu` columns:

| Text Value             | Numeric Code |
|------------------------|--------------|
| none                   | 0            |
| primary education      | 1            |
| 5th to 9th grade       | 2            |
| secondary education    | 3            |
| higher education       | 4            |

- Checked “Match entire cell contents”
- Repeated for both columns
- Verified that only numeric values remained in both columns

---

## 🧾 Final Notes

- All invalid ages removed  
- Missing values replaced meaningfully (`none_given`)  
- Text-based education levels successfully converted to numeric codes  
- Dataset is clean, structured, and ready for analysis

---

✅ Cleaned file saved as `student_data_cleaned.csv`  
📁 You can find the original and cleaned files in the `data/` folder.

