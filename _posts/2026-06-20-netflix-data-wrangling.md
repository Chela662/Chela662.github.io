---
title: "Netflix Data Wrangling (Kaggle Project)"
date: 2026-06-20
categories: [Data Science, Data Cleaning]
tags: [python, pandas, kaggle, data-wrangling]
---

##  Project Overview
This project focuses on cleaning and preparing the Netflix dataset from Kaggle. The goal was to improve data quality through exploration, handling missing values, feature transformation, and exporting a clean dataset for further analysis.

---

##  Dataset
The dataset contains Netflix titles with attributes such as:
- Title and type (Movie/TV Show)
- Director and cast
- Country of production
- Release year and rating
- Duration and categories

Initial dataset size:
- **8807 rows**
- **12 columns**

---

##  Data Cleaning Process

### 1. Data Exploration
- Checked dataset shape, data types, and structure
- Identified missing values and duplicates

### 2. Handling Missing Values
- Filled missing **director values** using cast relationships
- Filled missing **country values** using director-country mapping
- Replaced remaining missing values with `"Not Given"`
- Dropped rows with missing:
  - `date_added`
  - `rating`
  - `duration`

### 3. Feature Engineering
- Created a `director-cast` relationship column
- Analyzed frequent director-cast combinations

### 4. Data Cleaning Actions
- Removed unnecessary column (`description`)
- Ensured dataset consistency and completeness

---

##  Tools Used
- Python
- Pandas
- NumPy
- Kaggle Notebook Environment

---

##  Outcome
- Cleaned and structured dataset ready for analysis
- Improved data completeness by systematically handling missing values
- Exported final dataset as `cleaned_netflix.csv`

---

##  Output
Final dataset exported successfully and saved for further analysis or visualization.

---

##  Project Link
 [View on Kaggle](kaggle kernels pull k41522476/cynthia-kiptoo-netflix-data-wrangling)
