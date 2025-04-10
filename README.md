# SQL Advanced: Top Customers, Products, and Markets

This project showcases advanced SQL techniques to analyze and optimize sales data. It focuses on identifying top customers, products, and markets while accounting for pre-invoice and post-invoice discounts. The project includes performance improvements, reusable database views, and stored procedures to enable dynamic and scalable reporting.

---

## Problem Statement

**Objective:**  
Generate a detailed net sales report for each customer, product, and market by incorporating both pre-invoice and post-invoice discounts. Optimize performance and create modular SQL components for reuse.

---

## Project Structure

### 1. Pre-Invoice Discount Reporting
- Calculate gross sales and apply pre-invoice discounts.
- Generate reports for individual customers and all customers.

### 2. Performance Improvements
- Removed use of `get_fiscal_year()` function.
- Joined with `dim_date` and added `fiscal_year` to `fact_sales_monthly`.

### 3. Database Views
- Created reusable views:
  - `sales_preinv_discount`
  - `sales_postinv_discount`
  - `net_sales`

### 4. Stored Procedures
- `get_top_n_markets_by_net_sales`
- `get_top_n_customers_by_net_sales`
- `get_top_n_products_per_division_by_qty_sold`

### 5. Window Functions
- Percent of total and category-wise expenses
- Running totals
- Top-N ranking per category/division

---

## Concepts Used

- CTEs (Common Table Expressions)
- Views for modular SQL design
- Window Functions (`ROW_NUMBER`, `_
