# 🛒 Sales Data Analysis

This repository contains a complete analysis of retail sales data using Python and Pandas. The goal is to clean the dataset, handle missing or incorrect values, and perform insightful data analysis to understand customer behavior, revenue trends, product performance, and country-wise sales distribution.

---

## 📂 Dataset Overview

The dataset (`Sales_Data_Analysis.csv`) includes transaction records with the following key fields:
- `InvoiceNo` – Unique invoice identifier
- `StockCode` – Unique product code
- `Description` – Product name
- `Quantity` – Number of units purchased (can be negative for returns)
- `InvoiceDate` – Date and time of invoice
- `UnitPrice` – Price per unit
- `CustomerID` – Unique identifier for each customer
- `Country` – Customer's country

---

## 🧼 Data Cleaning Steps

- Removed rows with missing values in critical columns like `CustomerID` and `InvoiceNo`.
- Checked and removed duplicate entries.
- Converted `InvoiceDate` to datetime format and extracted `Month`.
- Created new columns such as:
  - `Revenue` = Quantity × UnitPrice
  - `Total Price` for each transaction

---

## 📊 Key Insights and Analyses

- **Total Revenue and Quantity Sold**: Calculated overall sales volume and income.
- **Unique Customers**: Identified number of individual customers.
- **Top-Selling Products**: Ranked products by quantity sold.
- **Customer Purchase Patterns**: Found average number of items bought per invoice.
- **Country-wise Revenue**: Identified countries with highest sales and most unique invoices.
- **Refund Analysis**: Filtered negative quantities to calculate total refunded amount.
- **Monthly Sales Trend**: Analyzed revenue month-wise to identify peak seasons.
- **Statistical Summary**: Used NumPy to calculate mean, median, and standard deviation of unit prices.

---

## 📈 Visualizations

- Bar charts for:
  - Top 10 products based on quantity
  - Top 5 countries by unique invoices
- Line graph for monthly revenue trend

---

## 💾 Output

- Cleaned and processed data is saved as:  
  `Sales_Data_With_TotalPrice.csv`

---

## 🛠️ Tools Used

- Python (Pandas, NumPy, Matplotlib)
- Jupyter Notebook

---

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sales-data-analysis.git
