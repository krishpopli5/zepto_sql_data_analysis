# Zepto Inventory & Pricing Data Analysis (SQL)

## Project Overview
An end-to-end SQL analysis of Zepto's product inventory, pricing strategies, stock availability, and revenue potential. This project includes database schema design, data cleaning, exploratory data analysis (EDA), and business intelligence querying using PostgreSQL.

## Dataset Schema
The primary table `zepto` contains product-level attributes:
- **SKU Metadata:** `sku_id`, `name`, `category`, `weightInGms`
- **Pricing & Discounts:** `mrp`, `discountPercent`, `discountedSellingPrice`
- **Inventory Tracking:** `availableQuantity`, `outOfStock`, `quantity`

## Key Business Insights & SQL Highlights
1. **Revenue Estimation:** Evaluated category-level total potential revenue (`discountedSellingPrice * availableQuantity`).
2. **Unit Value Optimization:** Calculated price-per-gram ratios across weight brackets to identify high-value consumer products.
3. **Out-of-Stock Impact:** Highlighted high-ticket items (`MRP > ₹300`) experiencing stockouts to optimize inventory reordering.
4. **Discount Dynamics:** Identified categories offering the highest average discounts to analyze promotional strategies.
