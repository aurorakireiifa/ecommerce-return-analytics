# E-Commerce Return Analytics

### Financial, Operational & ESG Insights

An exploratory data analytics project focused on e-commerce return patterns, financial impact, operational factors, customer demographics, and environmental indicators using Microsoft Excel, Power Query, Power BI, and DAX.

---

## 📌 Project Overview

This project analyzes e-commerce transaction data to identify return patterns and explore their potential financial, operational, customer-related, and environmental implications.

The analysis uses a synthetic e-commerce returns dataset containing **5,000 transactions**. The project demonstrates a data analytics workflow, from data preparation and transformation to interactive dashboard development and business recommendations.

## 🎯 Business Objectives

This project aims to answer the following business questions:

1. Which product category has the highest return rate and total return cost?
2. Are higher discount levels and shipping methods associated with different return rates?
3. What are the most common return reasons across product categories?
4. What environmental indicators are associated with returned orders?
5. How do return rates vary across customer demographic groups?
6. What environmental indicators are recorded for non-returned orders?

## 🗂️ Dataset

The project uses a **Synthetic E-Commerce Returns Dataset** containing:

- **5,000 transactions**
- **23 main columns**
- Transaction, product, customer, return, financial, and environmental indicator data

Key variables include:

- Order ID
- Product Category
- Product Price
- Order Quantity
- Discount Applied
- Shipping Method
- User Age
- User Gender
- User Location
- Return Status
- Return Reason
- Return Cost
- Profit/Loss
- CO₂ Emissions
- Packaging Waste
- CO₂ Saved
- Waste Avoided

## 🛠️ Tools & Technologies

- **Microsoft Excel** — Data inspection, cleaning, and exploratory analysis
- **Power Query** — Data transformation and numeric format correction
- **Power BI** — Interactive dashboard development and data visualization
- **DAX** — Measures and calculated columns for analytical metrics

## 🔄 Data Preparation & Analysis Process

### 1. Data Cleaning

Data quality checks and preparation included:

- Checking missing values
- Checking duplicate Order IDs
- Reviewing data types
- Correcting numeric formats and decimal separators
- Validating date formats

### 2. Data Preparation

Additional analytical variables were created to support segmentation and reporting:

- Age Group
- Discount Band
- Month
- Return Flag

### 3. Data Analysis

The analysis explored return patterns across:

- Product Category
- Discount Band
- Shipping Method
- Return Reason
- Customer Demographics
- Financial Impact
- Environmental Impact

### 4. Dashboard Development

An interactive Power BI dashboard was developed with three pages.

**Page 1 — Executive Overview**

- Total Orders
- Returned Orders
- Return Rate
- Total Return Cost
- Total Profit/Loss
- Monthly Order Value
- Return Rate by Product Category
- Returned vs. Not Returned

**Page 2 — Return & Financial Analysis**

- Return Rate by Discount Band
- Return Rate by Shipping Method
- Return Reason by Product Category
- Interactive filters

**Page 3 — Customer & ESG Analysis**

- Return Rate by Age Group
- Return Rate by Gender
- Top 10 Locations by Return Rate
- CO₂ Emissions
- Packaging Waste
- CO₂ Saved
- Waste Avoided

## 📊 Dashboard Preview

The dashboard provides an overview of return performance, financial metrics, operational patterns, customer demographics, and environmental indicators.

### Page 1 — Executive Overview

Provides a high-level view of transaction performance, including order volume, return rate, return costs, profit/loss metrics, monthly order value, and return rates by product category.

![Executive Overview Dashboard](images/overview-dashboard.png)

### Page 2 — Return & Financial Analysis

Explores return rates by discount band and shipping method, and compares return reasons across product categories to identify areas for further operational investigation.

![Return and Financial Analysis Dashboard](images/return-drivers.png)

### Page 3 — Customer & ESG Analysis

Examines return patterns by age group, gender, and customer location, alongside environmental indicators for returned and non-returned orders.

![Customer and ESG Analysis Dashboard](images/customer-esg.png)

## 🔍 Key Insights

### 1. Overall Return Performance

Of the 5,000 orders in the dataset, 1,450 were returned, resulting in an overall **return rate of 29%**. This means approximately three out of every ten orders were marked as returned.

### 2. Product Category

The **Clothing** category recorded the highest return rate at **37.43%**, with a total return cost of **IDR 132,200**.

This category is a priority for further investigation because of its relatively high return rate and return cost.

### 3. Discount Patterns

Transactions with discounts above 30% had a return rate of **34.22%**, higher than the overall rate of 29%.

This descriptive pattern suggests an association between the highest discount band and a higher return rate in this dataset. However, it does not establish that higher discounts cause returns.

### 4. Shipping Method

Return rates across shipping methods were relatively similar:

- Standard: **29.41%**
- Express: **29.09%**
- Next-Day: **28.50%**

The differences were relatively small, and the descriptive results do not indicate a substantial variation in return rates across shipping methods.

### 5. Return Reasons

The most frequently recorded return reasons were:

- Defective: **382 orders**
- Changed Mind: **379 orders**
- Wrong Item: **348 orders**
- Size Issue: **341 orders**

Defective and Changed Mind were the two most common reasons. These findings suggest areas for further investigation, including product quality, product information, and customer expectations.

### 6. Customer Demographics

Return rates across age groups were relatively stable, generally ranging from approximately 28% to 30%.

By gender:

- Female: **30.20%**
- Male: **27.72%**

These differences are descriptive and do not establish gender as a cause of product returns.

### 7. Environmental Indicators

The dashboard reports the following environmental indicators.

**Returned orders:**

- CO₂ Emissions: **2,167.50**
- Packaging Waste: **864.20**

**Non-returned orders:**

- CO₂ Saved: **5,333.00**
- Waste Avoided: **2,133.40**

These values represent the environmental indicators available in the dataset. Their interpretation depends on the underlying definitions, units, and calculation methods. They should not be interpreted as verified real-world environmental measurements without further validation.

## 💡 Business Recommendations

Based on the findings, the following actions could be considered:

1. **Investigate the Clothing category.** Review product quality, sizing information, product images, descriptions, and return patterns to identify potential improvement areas.
2. **Examine high-discount transactions.** Analyze transactions with discounts above 30% by product category, return reason, and other relevant characteristics to better understand the observed pattern.
3. **Strengthen quality control.** Since Defective was the most frequently recorded return reason, review product inspection procedures before shipment.
4. **Improve order fulfillment accuracy.** Examine picking, packing, and shipping processes to investigate potential issues associated with Wrong Item returns.
5. **Explore customer segments further.** Combine demographic information with product categories and return reasons before developing targeted actions.
6. **Monitor environmental indicators.** Track the available CO₂ and packaging waste metrics after validating their definitions and units.

## ⚠️ Interpretation & Limitations

This project is a descriptive analysis designed to identify patterns within a synthetic dataset. The findings do not establish causal relationships.

The environmental metrics depend on the definitions and assumptions embedded in the dataset. Further validation would be required before using them to make real-world sustainability claims.

The recommendations are proposed next steps and should be evaluated against additional data and relevant business context.

## 📂 Project Files

- **[Power BI Dashboard (.pbix)](powerbi/Return_Analytics.pbix)** — Interactive dashboard file for Microsoft Power BI Desktop.
- **[Cleaned Dataset (.xlsx)](data/returns_cleaned.xlsx)** — Prepared transaction dataset used in the analysis.
- **[Dataset in CSV Format](data/returns_sustainability_dataset.csv)** — CSV dataset supporting the analysis.

## 📁 Project Structure

```text
ecommerce-return-analytics/
├── README.md
├── data/
│   ├── returns_cleaned.xlsx
│   └── returns_sustainability_dataset.csv
├── documentation/
│   └── PORTOFOLIO AURORA 2026.pdf
├── images/
│   ├── overview-dashboard.png
│   ├── return-drivers.png
│   └── customer-esg.png
└── powerbi/
    └── Return_Analytics.pbix
```

---

*This project was developed for learning and portfolio purposes to demonstrate data preparation, exploratory analysis, dashboard development, and business-oriented interpretation.*
