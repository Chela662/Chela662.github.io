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


# PROJECT 2
# Exploratory Data Analysis on the Titanic Dataset

This project involved performing Exploratory Data Analysis (EDA) on the Titanic dataset using Python. The objective was to understand the structure of the data, identify missing values, detect outliers, and uncover patterns that influenced passenger survival.

Using Pandas, NumPy, Matplotlib, and Seaborn, I explored demographic information such as age, gender, passenger class, fare, and embarkation point. Various visualizations, including histograms, box plots, count plots, heatmaps, and scatter plots, were created to reveal relationships between variables and survival outcomes.

Key findings showed that survival rates varied significantly by passenger class, gender, age, and embarkation location. Missing values were identified and analyzed, while fare outliers were handled through percentile capping. The project strengthened my skills in data cleaning, data visualization, statistical analysis, and extracting insights from real-world datasets.

**Tools Used:** Python, Pandas, NumPy, Matplotlib, Seaborn, Kaggle

**Skills Demonstrated:** Data Cleaning, Exploratory Data Analysis (EDA), Data Visualization, Feature Analysis, Outlier Detection, Insight Generation

# Project link
https://www.kaggle.com/code/k41522476/cynthia-kiptoo-eda
