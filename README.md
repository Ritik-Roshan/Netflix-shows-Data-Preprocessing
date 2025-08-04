# Netflix-shows-Data-Preprocessing
Clean and prepare a raw dataset (with nulls, duplicates, inconsistent formats)

## Overview
This project involved cleaning and preprocessing the Netflix Titles dataset to prepare it for further analysis.

## Steps Performed
### 🧹 Data Cleaning
- Renamed all column headers to **lowercase with underscores** (e.g., `date_added`).
- **Handled missing values** in:
  - `director`, `cast`, `country`, `rating`, and `duration` — filled with `"Unknown"` or `"Not Rated"`.
  - `date_added` — converted to proper datetime; some values were left as `NaT` if they were invalid.
- **Removed duplicates** to ensure uniqueness in rows (though no actual duplicates were found).

### 🔤 Text Standardization
- Cleaned `country` names to **title case** (e.g., `united states` → `United States`).
- Standardized `rating` values to **uppercase** (e.g., `tv-ma` → `TV-MA`).
  
### 🕒 Date and Format Fixes
- Converted `date_added` column to consistent `dd-mm-yyyy` format for clarity.
- Ensured `release_year` was properly typed as an integer.
  
### 🧪 Data Types Verified
- Checked and corrected data types to match expected formats:
  - `date_added`: `datetime` → formatted to string (`dd-mm-yyyy`)
  - `release_year`: `int`

---

## 📁 Output
The final dataset is now:
- Clean
- Uniform
- Free of duplicates
- Formatted properly for immediate analysis or visualization

---

## 👨‍💻 Tools Used
- Python (Pandas)
- Jupyter Notebook / VS Code
- Dataset: `netflix_titles.csv`

---
