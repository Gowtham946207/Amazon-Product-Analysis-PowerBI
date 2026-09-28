# 📊 Amazon Product Value & Performance Analysis

A Power BI data analysis project focused on analyzing Amazon product data using **Microsoft Power BI, DAX, and Microsoft Excel**.

The dashboard provides an interactive view of product value, pricing, product categories, customer reviews, and order-date trends.

---

## 📌 Project Overview

The objective of this project is to analyze Amazon product data and transform it into meaningful business insights through **data preparation, DAX calculations, data visualization, and interactive Power BI reporting**.

The project focuses on:

- Product value analysis
- Product pricing
- Product category performance
- Product-level analysis
- Customer review analysis
- Monthly trends
- Weekly trends
- Interactive filtering

---

## 📁 Dataset

The project uses the following Excel dataset:

```text
Amazon_Combined_Data.xlsx
```

The main dataset contains information such as:

- Product Category
- Product Description
- Price (Dollar)
- Number of Reviews
- Order Date
- Shipment

The dataset is used for educational and portfolio purposes.

---

## 🛠️ Technologies Used

- **Microsoft Power BI**
- **DAX**
- **Microsoft Excel**
- **Data Visualization**
- **Data Analysis**
- **Git & GitHub**

---

## 🔄 Project Workflow

```text
Excel Dataset
      ↓
Data Preparation
      ↓
Power BI Data Loading
      ↓
Data Modeling
      ↓
DAX Measures
      ↓
Data Visualization
      ↓
Interactive Dashboard
      ↓
Business Analysis
```

---

## 📊 Power BI Dashboard

The dashboard provides an interactive analysis of Amazon product data.

### Key KPIs

- **Total Product Value**
- **Average Product Price**
- **Total Products**
- **Total Reviews**

### Dashboard Visualizations

- Product Value by Month
- Product Value by Week
- Product Value by Category
- Product Value by Product
- Reviews by Product
- Product Category slicer
- Quarter slicer

---

## 📐 Data Model

The Power BI model uses the Amazon product dataset together with a Date Table for time-based analysis.

```text
┌──────────────────┐
│    Date Table    │
└────────┬─────────┘
         │
         │ 1 : *
         ▼
┌──────────────────┐
│   Amazon_Data    │
└──────────────────┘
```

The Date Table is connected to:

```text
Date Table[Date]
        ↓
Amazon_Data[Order Date]
```

---

## 📏 DAX Measures

### Total Product Value

```DAX
Total Product Value =
SUM('Amazon_Data'[Price(Dollar)])
```

### Average Product Price

```DAX
Average Product Price =
AVERAGE('Amazon_Data'[Price(Dollar)])
```

### Total Products

```DAX
Total Products =
DISTINCTCOUNT('Amazon_Data'[Product Description])
```

### Total Reviews

```DAX
Total Reviews =
SUM('Amazon_Data'[Number of reviews])
```

These measures are used to create the main KPI cards and dashboard analysis.

---

## 🔍 Business Questions

This project is designed to answer questions such as:

1. What is the total product value?
2. What is the average product price?
3. How many unique products are available?
4. Which product categories have higher product value?
5. Which products have higher prices?
6. Which products receive the most reviews?
7. How does product value change over time?
8. How does product value vary across weeks?
9. How does product category affect overall product value?
10. How do reviews vary between products?

---

## 📈 Key Analysis Areas

### Product Category Analysis

The dashboard compares product value across categories such as:

- Audio Video
- Camera
- Car Accessories
- Laptop
- Men Clothes
- Men Shoes
- Mobile & Accessories
- Toys

### Product Analysis

The dashboard provides product-level analysis based on:

- Product value
- Product price
- Customer reviews

### Time Analysis

The dashboard analyzes product value using:

- Month
- Week
- Quarter
- Order Date

---

## 🎛️ Interactive Filters

The dashboard includes interactive filters for:

### Product Category

Users can select individual categories such as:

- Camera
- Laptop
- Car Accessories
- Mobile & Accessories
- Toys
- Men Shoes
- Men Clothes
- Audio Video

### Quarter

Users can filter the dashboard by:

- Qtr 1
- Qtr 2
- Qtr 3
- Qtr 4

Selecting a category or quarter dynamically updates the dashboard visuals and KPI cards.

---

## 📸 Dashboard Preview

![Amazon Product Analysis Dashboard](screenshots/amazon_product_analysis_dashboard.png)

---

## 📂 Project Structure

```text
Amazon-Product-Analysis/
│
├── Amazon_Combined_Data.xlsx
│
├── Amazon_Product_Analysis.pbix
│
├── amazon_product_analysis_dashboard.png
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## 🚀 How to Use

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate to the project:

```bash
cd Amazon-Product-Analysis
```

### 2. Open the Power BI Dashboard

Open:

```text
powerbi/Amazon_Product_Analysis.pbix
```

### 3. Refresh the Dataset

If Power BI asks for the data source, select:

```text
data/Amazon_Combined_Data.xlsx
```

Then select **Refresh**.

### 4. Interact With the Dashboard

Use the:

- Product Category slicer
- Quarter slicer
- Charts
- KPI cards

to explore the data.

---

## 📊 Project Outputs

The project provides:

- Interactive Power BI dashboard
- Product category analysis
- Product-level analysis
- Product value analysis
- Price analysis
- Review analysis
- Monthly trend analysis
- Weekly trend analysis
- Interactive filtering

---

## ⚠️ Data Note

The dataset contains a **Price (Dollar)** field rather than a clearly defined transaction-level revenue or quantity-sold field.

Therefore, this project uses the term **Total Product Value** instead of claiming that the calculated value represents actual revenue or sales.

This distinction is maintained to ensure that the dashboard calculations accurately represent the available dataset.

---

## 👨‍💻 Author

**Gowtham S**

**Aspiring Data Analyst**

### Skills Demonstrated

- Power BI
- DAX
- Microsoft Excel
- Data Analysis
- Data Visualization
- Data Modeling
- KPI Development
- Business Intelligence

---

## 🎯 Portfolio Purpose

This project demonstrates practical skills in **Power BI, DAX, data visualization, data modeling, KPI development, and business analysis**.

The project shows how raw Excel data can be transformed into an interactive business intelligence dashboard.

---
