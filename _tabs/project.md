---
title: Projects
permalink: /projects/
icon: fas fa-briefcase
---
---
title: "Netflix Data Wrangling (Kaggle Project)"
date: 2026-06-20
categories: [Data Science, Data Cleaning]
tags: [python, pandas, kaggle, data-wrangling]
---

##  Project Overview
This project focuses on cleaning and preparing the Netflix dataset from Kaggle. The goal was to improve data quality through exploration, handling missing values, and exporting a cleaned dataset.

---

##  Dataset
- Source: Kaggle Netflix Dataset  
- Rows: 8807  
- Columns: 12  

---

##  Data Cleaning Steps

### 1. Data Exploration
- Checked dataset shape and structure
- Identified missing values
- Checked duplicates

### 2. Handling Missing Values
- Filled missing director values using cast relationships
- Filled missing country values using director mapping
- Replaced remaining missing values with "Not Given"

### 3. Feature Engineering
- Created director-cast relationship column
- Analyzed frequent director-cast patterns

### 4. Final Cleaning
- Removed unnecessary column: description
- Dropped rows with missing date_added, rating, and duration

---

##  Tools Used
- Python
- Pandas
- NumPy
- Kaggle Notebook

---

##  Outcome
- Clean dataset ready for analysis
- Improved data consistency
- Exported as `cleaned_netflix.csv`

---

##  Project Link
https://www.kaggle.com/code/k41522476/cynthia-kiptoo-netflix-data-wrangling





