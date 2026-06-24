# Ecommerce Sales Analysis & Visualization Dashboard

## 📋 Project Overview

This project involves a comprehensive **data cleaning, analysis, and visualization** of an Ecommerce sales dataset using Microsoft Excel. The goal was to transform raw transactional and customer data into actionable business insights through descriptive statistics, pivot tables, and an interactive dashboard.

**Author:** Srivatsan  
**Dataset:** `Dataset.xlsx` (Raw data)  
**Processed Workbook:** `Ecommerce Visualisation- Srivatsan.xlsx`

---

## 🗂️ Project Structure

### 1. Raw Dataset (`Dataset.xlsx`)
- **Customer_Dim** sheet: Contains 500+ customer records with attributes like `Customer_ID`, `Name`, `Age`, `Gender`, `City`, `State`, `Country`, and `Loyalty_Level`.
- **Sales Data**: Transaction-level records (approx. 2,000 sales) including `Sale_ID`, `Date`, `Customer_ID`, `Product_ID`, `Store_ID`, `Quantity`, `Unit_Price`, `Discount`, `Payment_Method`, and `Total_Amount`.

### 2. Processed Workbook (`Ecommerce Visualisation- Srivatsan.xlsx`)

#### Key Sheets:
- **Customer_Details_USA**: Cleaned and enhanced customer data.
  - Standardized names, fixed inconsistencies (e.g., titles like "Dr.", "MD").
  - Imputed missing `Loyalty_Level` using state-wise mode (via COUNTIFS + VLOOKUP logic).
  - Added `Type of Customer` (Young Adult / Middle Aged Adult / Old Aged Adult) based on age.
- **Store_Details**: Store master data with `Store_ID`, `Store_Name`, `Region`, `City`, `Store_Type` (Flagship / Outlet / Online).
- **Descriptive Analysis**: Summary statistics for key metrics:
  - Customer Age, Product Cost, Stock Levels, Total Amount.
  - Monthly sales volume trends.
- **Pivots**: Extensive pivot tables covering:
  - Sales by Product, Store, Region, Payment Method.
  - Quantity and Revenue breakdowns.
  - Loyalty level & Gender-based spending analysis.
- **Pivot Charts**: Visual representations of key pivots.
- **Dashboard**: Interactive summary dashboard (screenshots available in dedicated sheet).
- **Data Cleaning ScreenShots** & **DashBoard Screenshots**: Documentation of the ETL process.

---

## 🛠️ Data Cleaning & Transformation Performed

1. **Customer Data Cleaning**:
   - Removed extra spaces and standardized names.
   - Corrected gender/name mismatches.
   - Imputed missing Loyalty Levels using mode by State.
   - Categorized customers by age group.

2. **Sales Data Enhancements**:
   - Calculated `Total_Amount` where missing (`Quantity × Unit_Price × (1 - Discount)`).
   - Standardized dates and payment methods.
   - Added derived columns (e.g., discount flags, region mapping).

3. **Data Validation & Enrichment**:
   - VLOOKUPs to link customers, products, and stores.
   - COUNTIFS for loyalty distribution analysis.

---

## 📊 Key Insights (Extracted from Analysis)

### Customer & Loyalty
- Female Platinum customers significantly outperform males in spending.
- Old-Aged Adults drive nearly 49% of total revenue.
- Bronze tier shows poor performance — opportunity for conversion programs.

### Regional Performance
- **North Region** dominates (64% volume, 63.5% revenue).
- **West** has the highest average transaction value despite lower volume.

### Product & Store Performance
- Top product: PROD37 (87 units).
- High-performing stores: STORE3, STORE12, STORE11.
- Balanced payment method distribution (PayPal slightly leads).

### Seasonal Trends
- Peak sales in March and July.
- Q1 performs strongly; May shows a notable dip.

---

## 🎯 Business Recommendations

- Prioritize retention programs for Old-Aged Platinum customers.
- Develop youth-focused acquisition strategies.
- Scale best practices from top-performing Northern stores to other regions.
- Investigate and address underperformance in the Bronze loyalty tier.
- Leverage gender-specific insights for targeted marketing (especially female Platinum segment).

---

## 📁 Files in Repository

- `Dataset.xlsx` — Original raw data.
- `Ecommerce Visualisation- Srivatsan.xlsx` — Fully processed workbook with analysis, pivots, and dashboard.
- `README.md` — This file.
- (Optional) Screenshots folder with dashboard and cleaning process visuals.

---

## 🛠️ Tools & Techniques Used

- Excel Functions: `VLOOKUP`, `COUNTIFS`, `TEXT`, `TRIM`, `IF`, `DATEDIF`, etc.
- Pivot Tables & Slicers for dynamic analysis.
- Conditional Formatting.
- Descriptive Statistics (Mean, Median, Std Dev, etc.).
- Dashboard design with charts and key metrics.

---

## 🚀 How to Use

1. Download the repository.
2. Open `Ecommerce Visualisation- Srivatsan.xlsx`.
3. Explore the **Dashboard** sheet for high-level KPIs.
4. Use slicers in Pivot sheets to filter dynamically.
5. Review **Descriptive Analysis** and **Pivots** for detailed breakdowns.

---

## 📄 License

This project is for educational/portfolio purposes. Feel free to use as a reference for Excel-based data analysis projects.

---

**Made with ❤️ for data-driven decision making**
