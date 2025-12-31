# Uncovering the Strategies of Boosting the Sales of ZEDEF Corporation

## 📌 Project Overview

This project analyzes sales data from **ZEDEF Corporation** to uncover actionable strategies for boosting revenue across products and regions. Using structured data cleaning, exploration, and descriptive analysis techniques, the project identifies high‑performing and underperforming products and regions to guide management investment decisions.

The analysis was conducted primarily using spreadsheet‑based tools and focuses on translating raw transactional data into business insights.

---

## ❓ Business Problem

**What should the management do to boost the sales of ZEDEF Corporation?**

The core objective is to determine:

* Which products generate the highest and lowest sales
* Which regions perform best and worst
* Where the company should increase or reduce investment

---

## 📂 Dataset Description

The dataset provided is an **unstructured sales dataset** containing:

* **1010 rows** and **11 columns**

### Columns

* Transaction ID
* Customer Name
* Customer Email
* Region
* Product Category
* Product
* Quantity *(numeric)*
* Unit Price *(numeric)*
* Total Sales *(numeric)*
* Transaction Date *(date)*
* Payment Method

---

## 🧹 Data Cleaning Process

The data cleaning process ensured consistency, accuracy, and completeness.

### Key Steps

1. **VLOOKUP Integration**
   Used VLOOKUP to transfer data from raw sheets into a clean working sheet using unique Transaction IDs.

2. **Duplicate Removal**

   * Applied *Advanced Filter* to extract unique Transaction IDs
   * Ensured only one record per transaction

3. **Date Standardization**

   * Created helper columns: `transactionDay`, `transactionMonth`, `transactionYear`
   * Used TEXT, FIND, DAY, MONTH, YEAR, and DATE functions to generate consistent date formats

4. **Numeric Data Cleaning**

   * Removed extra spaces in Quantity, Unit Price, and Total Sales
   * Converted values using TRIM and NUMBERVALUE

5. **Text Data Cleaning**

   * Applied TRIM across all text columns

6. **Missing Value Handling**

   * Missing emails replaced with `replacement@mail.com`
   * Missing product values replaced with `Blank`

7. **Data Validation**

   * Email column restricted to values containing `@`
   * Total Sales restricted to positive non‑zero numbers

---

## 🔍 Data Exploration

### Summary Statistics

* **Regions:** 4
* **Product Categories:** 5
* **Unique Products:** 622
* **High‑Value Transactions:** 375 transactions above total sales threshold of 3000

### Exploration Techniques

* Sorting and filtering
* Helper columns for ranking top products and regions
* Identification of invalid emails and regions

---

## 📊 Data Analysis

### Descriptive Analysis

* Final cleaned dataset contains **1000 valid transactions**
* High standard deviation indicates significant variability in sales

### Key Insights

* **Highest Monthly Sales:** June
* **Top Product Category:** Books
* **Second Best Product:** Clothing
* **Top Performing Region:** West
* **Lowest Performing Region:** North

### Product & Region Insights

* Books sell best overall, especially in the **East and West**
* Clothing consistently ranks second across regions
* Electronics has the lowest sales
* Food performs poorly in the West
* Books perform poorly in the South

---

## 🚨 Underperforming Areas

* Electronics (all regions)
* Books in the South
* North region (overall)
* Food in the West

---

## ✅ Recommendations

### Recommended Investments

1. Invest in **Books in the East** ⭐
2. Invest in **Books in the West** ⭐
3. Invest in **Clothing across regions**
4. Increase Clothing investment in the West

### Investments to Avoid

1. Electronics products
2. Books in the South ⭐
3. North region
4. Food products in the West

---

## 🛠 Tools & Techniques Used

* Spreadsheet software (Excel)
* VLOOKUP, IFERROR, TRIM, DATE, TEXT functions
* Pivot tables and pivot charts
* Conditional formatting and data validation

---

## 📈 Outcome

This analysis provides ZEDEF Corporation with **data‑driven guidance** on where to allocate resources for maximum sales impact, enabling smarter strategic and financial decisions.

---
