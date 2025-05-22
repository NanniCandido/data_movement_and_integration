# Socioeconomic Factors and Obesity: A US Nation/State-Level Analysis

**Final Project — DBAS3018: Data Movement and Integration**  
**Nova Scotia Community College — November 2024**  
**Elaine da Silva (w0445885) & Tiankun Deng (w0453048)**

---

## 📌 Project Overview

This project was developed as the final assignment for the Data Movement and Integration course, where we learned and explored the Python programming language. It conducts an exploratory analysis of the dataset "Nutrition, Physical Activity, and Obesity - Behavioral Risk Factor Surveillance System" (available on DATA.GOV), with the objective of uncovering patterns and trends related to nutrition, physical activity, and obesity across the United States. The analysis is performed using Python, with a focus on Object-Oriented Programming (OOP) principles and the use of core libraries such as Pandas, NumPy, and Apache Spark.

To complement the analysis, we also used the **"yellow_tripdata_2015-01.csv"** dataset from [Kaggle](https://www.kaggle.com/datasets) to evaluate time and memory performance differences between **Pandas** and **Spark** when processing large datasets.

---

## 🔍 Research Objectives

The project addresses five key research questions and incorporates the following programming and data processing techniques:

- **Python**: Use of functions, loops, and conditional logic
- **Pandas**: CSV I/O operations, DataFrame/Series manipulation
- **NumPy**: Array operations and computations
- **Data Wrangling**: Handling of missing and unstructured data
- **Visualization**: Generation of insightful plots
- **Performance Monitoring**: Comparison of time and memory efficiency between Pandas and Apache Spark

---

## 📊 Datasets Used

### 1. Nutrition, Physical Activity, and Obesity Dataset

- **Source**: Behavioral Risk Factor Surveillance System (BRFSS)
- **Rows**: 104,272  
- **Columns**: 33  
- **Period**: 2011–2023  
- **Demographics**: Gender, Age, Race, Income, Education, and more  
- **Geography**: State-level and national-level data  
- **Topics**:
  - Nutrition (e.g., fruits & vegetables consumption)
  - Obesity and Weight Status
  - Physical Activity

**Note on Structure**: Each demographic group is recorded exclusively, meaning only the relevant category field is populated per record. This requires careful filtering to extract meaningful insights without introducing bias from null fields.

### 2. Yellow Taxi Trip Dataset

- **Source**: Kaggle  
- **Rows**: 12,748,986  
- **Columns**: 19  
- **Date Range**: January 2015  
- **Includes**:
  - Start/end times
  - Pickup/drop-off locations (lat/long)
  - Passenger count
  - Trip distance
  - Fare details (fare, tolls, tips)

This dataset was primarily used to benchmark the **performance of Pandas vs. Spark** for large-scale data handling.

---

## 🔧 Data Wrangling Highlight

A unique aspect of the BRFSS dataset is its **mutually exclusive demographic structure**. When filtering by one category (e.g., gender), other demographic columns remain unpopulated. Proper filtering of the `StratificationCategory1` column ensures clean subsets, such as male/female-only data, simplifying analysis and improving accuracy.

Visual examples of the raw vs. filtered data structures are provided in the notebook.

---

## 📦 Tools & Technologies

- **Python 3.x**
- **Jupyter Notebook**
- **Pandas**
- **NumPy**
- **Apache Spark (PySpark)**
- **Matplotlib / Seaborn**
- **Memory & Time profiling tools**

---



