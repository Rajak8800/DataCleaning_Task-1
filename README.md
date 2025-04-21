# DataCleaning_Task-1
# 📊 Task 1 – Data Cleaning and Preprocessing

## 🧠 Internship: Elevate Labs – Data Analyst Role  
This repository contains the solution to Task 1 of my internship: cleaning and preprocessing a raw dataset using Python (Pandas).

---

## 📁 Dataset Used:
**Task_1DataCleaning_Elevate_Labs.xlsx**  
The dataset contains order-level transactional data with attributes like order date, ship date, customer name, price, quantity, etc.

---

## 🔧 Data Cleaning Steps:

1. **Handled Missing Values**  
   - Filled missing `Customer Name` and `Region` entries with `'Unknown'`.

2. **Standardized Date Formats**  
   - Converted `Order Date` from inconsistent formats (e.g., `2025-03-08`, `03/07/2025`) to a unified datetime format.

3. **Cleaned Numeric Fields**  
   - Removed symbols like `$` from `Price`, then converted it to `float`.  
   - Converted `Quantity` to `int` and replaced invalid entries with `0`.

4. **Renamed Columns**  
   - All column names were made lowercase and spaces replaced with underscores for consistency.

5. **Removed Duplicates**  
   - Duplicate rows were identified and dropped.

6. Some entries in the Quantity column have negative values. These were retained intentionally, assuming they represent product returns, cancellations,
    or adjustments, which are common in sales and accounting datasets.

---

## ✅ Cleaned Output
- ✅ `cleaned_dataset.csv` – Final cleaned data
- ✅ Preview of first few rows shown below:

| order_id | customer_name | order_date | ship_date | product | quantity | price | total_price | region |
|----------|----------------|------------|-----------|---------|----------|-------|--------------|--------|
| 2001     | Chris Paul     | 2025-03-08 | 2025-03-28| Charger | 3        | 50.0  | -85          | East   |

---

## 🧪 Tools Used:
- Python
- Pandas
- Jupyter Notebook (for processing and documentation)

---

## 🚀 How to Use:
1. Clone the repository.
2. Open the notebook `task_1_data_cleaning.ipynb`.
3. Run the cells to see the data cleaning process.
4. Explore the cleaned dataset in `cleaned_dataset.csv`.

---

## 📜 License:
This project is part of Elevate Labs Internship - April 2025.
