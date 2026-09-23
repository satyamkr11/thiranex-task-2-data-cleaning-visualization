# Thiranex Internship — Task 2
## Retail Sales Data Cleaning, Visualization & Business Insights

A complete data cleaning and exploratory analysis project using the **UCI Online Retail Dataset**.  
The project focuses on cleaning raw retail transaction data, handling missing and invalid records, creating useful features, visualizing sales patterns, and extracting business insights.

---

## 📌 Project Overview

This project was completed as part of the **Thiranex Internship — Task 2: Data Cleaning & Visualization**.

The analysis follows an end-to-end data analytics workflow:

- Load and inspect raw retail transaction data
- Identify missing values and duplicate records
- Investigate cancellations and invalid transactions
- Clean and transform the dataset
- Create revenue-based features
- Analyse sales performance
- Visualize important business patterns
- Extract actionable business insights

---

## 🎯 Objectives

The main objectives of this project are:

1. Understand the structure of a large retail transaction dataset.
2. Identify and handle missing values.
3. Detect and remove duplicate and invalid records.
4. Analyse cancelled and negative transactions.
5. Calculate transaction-level revenue.
6. Analyse sales by country, product and month.
7. Create visualizations for business interpretation.
8. Summarize key findings from the cleaned dataset.

---

## 📊 Dataset

**Dataset:** Online Retail Dataset

**Source:** UCI Machine Learning Repository

The dataset contains retail transactions with information such as:

- Invoice Number
- Stock Code
- Product Description
- Quantity
- Invoice Date
- Unit Price
- Customer ID
- Country

The original dataset contains **541,909 rows and 8 columns**.

Dataset source:

https://archive.ics.uci.edu/dataset/352/online+retail

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Jupyter Notebook**
- **Excel (.xlsx)**

---

## 🔍 Data Cleaning Process

The following cleaning steps were performed:

### 1. Initial Data Inspection
- Checked dataset dimensions
- Examined data types
- Inspected descriptive statistics
- Analysed missing values
- Identified duplicate records

### 2. Missing Values
Missing values were investigated, particularly in:

- `Description`
- `CustomerID`

Cleaning decisions were made based on whether the records were still useful for transaction analysis.

### 3. Duplicate Records
Duplicate transaction rows were identified and removed.

### 4. Invalid Transactions
The dataset was examined for:

- Cancelled transactions
- Negative quantities
- Invalid prices
- Non-positive sales values

Only valid positive-sales transactions were retained for the main revenue analysis.

### 5. Feature Engineering

A revenue feature was calculated using:

```python
Revenue = Quantity × UnitPrice
