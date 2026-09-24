# Supermarket Sales Analysis

A comprehensive Data Analytics Capstone Project analyzing 500 supermarket sales transactions to evaluate revenue trends, branch efficiency, product popularity, category share, customer spending habits, and customer ratings.

**Submitted by:** Harsh Agrawal  
**Program:** IBM SkillsBuild Internship  
**Domain:** Retail Data Analytics & Business Intelligence  

---

## Project Overview
Supermarkets handle diverse merchandise across multiple branches with high transaction volumes daily. This project provides end-to-end data analysis on supermarket transactional logs to help store managers and executives make informed, data-driven decisions.

The analysis is structured around a 6-step analytics pipeline:
1. **Data Loading & Inspection**: Importing 500 retail transactions and auditing data structure.
2. **Data Cleaning & Verification**: Validating zero missing values, zero duplicates, and verifying the core identity:
   $$\text{Sales} = \text{Quantity} \times \text{Unit Price}$$
3. **Exploratory Data Analysis (EDA)**: Answering the 6 core live analysis questions.
4. **Data Visualization**: Creating visual charts to compare branch, category, product, and payment performances.
5. **Business Decisions & Recommendations**: Formulating actionable strategies for inventory, store operations, and customer loyalty.
6. **Project Reporting**: Documenting the complete methodology and results in a formal report.

---

## Dataset Information
* **Dataset File:** [`SUPER MARKET DATA.xlsx`](SUPER%20MARKET%20DATA.xlsx)
* **Total Records:** 500 transactions
* **Time Span:** January 1, 2026 to July 1, 2026
* **Key Columns:**
  * `Invoice ID`: Unique alphanumeric transaction identifier (`INV0001` - `INV0500`)
  * `Date`: Date of purchase
  * `Branch`: Supermarket branch code (`A`, `B`, `C`, `D`)
  * `City`: City location (`Jaipur`, `Delhi`, `Mumbai`, `Bengaluru`)
  * `Customer Type`: Loyalty tier (`Member`, `Normal`)
  * `Gender`: Customer gender (`Female`, `Male`)
  * `Product`: Specific item SKU (20 unique items e.g., Cheese, Coffee, Shampoo)
  * `Category`: Merchandise department (Beverages, Personal Care, Dairy, Grocery, Fruits, Snacks, Vegetables, Bakery)
  * `Quantity`: Number of units bought (1 to 10)
  * `Unit Price`: Price per unit in INR (₹)
  * `Payment`: Payment method used (`UPI`, `Net Banking`, `Card`, `Cash`)
  * `Rating`: Customer feedback rating (scale: 1.0 to 5.0)
  * `Sales`: Total order revenue in INR (₹)

---

## Key Findings & Live Analysis Answers

| # | Business Question | Finding & Exact Metrics |
|---|---|---|
| **Q1** | **Which product generates the highest sales?** | **Cheese** generated the highest sales: **₹27,906.30** (126 units sold across 26 transactions), followed closely by Coffee (₹27,694.87) and Shampoo (₹27,497.48). |
| **Q2** | **Which branch performs best?** | **Branch C (Mumbai)** performed best with sales of **₹72,469.45** across 143 orders, followed by Branch B (Delhi: ₹64,116.26), Branch D (Bengaluru: ₹55,468.29), and Branch A (Jaipur: ₹52,357.08). |
| **Q3** | **Which category sells the most?** | **Beverages** had the highest sales with **₹56,108.24** (465 units sold across 82 orders), followed by Personal Care (₹45,943.96) and Dairy (₹43,992.00). |
| **Q4** | **What is the most popular payment method?** | **UPI** was the most used payment method with **127 transactions** (generating ₹67,910.33), followed by Net Banking (126), Card (125), and Cash (122). |
| **Q5** | **Do Members spend more than Normal customers?** | **No.** Normal customers have a slightly higher average transaction spend (**₹497.07**) than Members (**₹483.14**). However, Members account for **58.5%** of total sales (**₹143,009.30**) due to higher visit frequency (296 vs 204 orders). |
| **Q6** | **What is the average customer rating?** | The average customer rating across all 500 transactions was **3.99 out of 5.0**. Branch D recorded the highest satisfaction (4.09), while Branch A had the lowest (3.84). |

### Additional Highlights:
* **Total Supermarket Revenue:** ₹244,411.08 across 2,768 units sold.
* **Monthly Peak:** April 2026 was the highest grossing month (₹52,569.77 across 90 transactions).
* **Demographic Parity:** Females generated ₹123,954.12 (50.7%) and Males generated ₹120,456.96 (49.3%), indicating balanced patronage.

---

## Technologies Used
* **Programming Language:** Python 3
* **Data Processing & Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Spreadsheet & Word Automation:** openpyxl, python-docx
* **Execution Environments:** Jupyter Notebook (`.ipynb`), Google Colab

---

## Setup & Execution Instructions

### Option A: Running in Google Colab (Recommended)
1. Open [Google Colab](https://colab.research.google.com).
2. Click **File** → **Upload notebook** and choose `Harsh_Agrawal_SupermarketSalesAnalysis.ipynb`.
3. In the left file explorer sidebar of Colab, upload `SUPER MARKET DATA.xlsx`.
4. In the top menu, click **Runtime** → **Run all** (or press `Ctrl + F9`).
5. All cells will execute in order, printing the summary statistics and rendering the charts inline.

### Option B: Local Environment
1. Clone or download this repository.
2. Open a terminal / command prompt in this directory.
3. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Harsh_Agrawal_SupermarketSalesAnalysis.ipynb
   ```

---

## Repository Structure
```
├── SUPER MARKET DATA.xlsx                           
├── Harsh_Agrawal_SupermarketSalesAnalysis.ipynb   
├── Harsh_Agrawal_ProjectReport.docx                
├── requirements.txt                                 
├── README.md                                        
└── figures/                                         
    ├── top_products_sales.png
    ├── sales_by_branch.png
    ├── sales_by_category.png
    ├── payment_methods.png
    ├── customer_type_comparison.png
    ├── monthly_sales_trend.png
    └── rating_by_branch.png
```

---

## Strategic Recommendations for Supermarket Management
1. **Stock Optimization:** Maintain buffer stocks and automated reorder alerts for top revenue generators: Cheese, Coffee, and Shampoo.
2. **Branch Benchmarking:** Study operational practices, customer engagement, and product display in Branch C (Mumbai) to replicate across Branch A (Jaipur).
3. **Digital Checkout:** Expand dedicated express payment counters for UPI and Net Banking payments, which represent over 50% of orders.
4. **Loyalty Incentives:** Introduce basket-size threshold discounts for Members (e.g., bonus points for orders above ₹600) to raise their average spend.
5. **Branch A Service Quality:** Implement cashier training and customer feedback kiosks at Branch A to elevate its customer satisfaction rating from 3.84 to store network average.

---

## Author
* **Harsh Agrawal**
* IBM SkillsBuild Internship
* Capstone Project Submission — September 2026
