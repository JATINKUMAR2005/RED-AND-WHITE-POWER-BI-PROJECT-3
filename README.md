# 📊 DAX Depo – Advanced Calculations Using DAX in Power BI

## 🧠 Project Overview
The **DAX Depo** project is an advanced Power BI analytics initiative focused on building a strong backend data model and implementing **complex DAX calculations** to analyze sales, profitability, customer behavior, and return trends.

The project emphasizes **data modeling, DAX logic, and matrix-based reporting**, avoiding traditional visual-heavy dashboards. This approach mirrors real-world enterprise BI solutions where accuracy, performance, and scalability are critical.

---

## 🎯 Project Objectives
- Build a **robust Star Schema data model**
- Perform **advanced analytical calculations using DAX**
- Implement **time intelligence functions**
- Analyze **sales, profit, and returns**
- Understand **filter context and DAX behavior**
- Display results using **Matrix visuals only**

---

## 🗂️ Dataset Description

### Fact Tables
- **Sales_Fact**
  - Transaction-level sales data
  - Sales Amount, Cost, Quantity, Date, Product, Customer, Region
- **Returns_Fact**
  - Returned item details
  - Return Quantity, Return Date, Reason

### Dimension Tables
- **Customer_Dim** – Customer details and segments  
- **Product_Dim** – Product categories and SKUs  
- **Region_Dim** – Geographic hierarchy (Region, State, City)  
- **Date_Dim** – Calendar table for time intelligence  

---

## 🏗️ Data Modeling Approach
A **Star Schema** was implemented to ensure:
- Faster query performance
- Clear filter propagation
- Scalable analytical design

### Relationships
- One-to-many relationships between dimensions and `Sales_Fact`
- `Returns_Fact` connected separately due to different analytical grain
- **Inactive relationship** between `Date_Dim` and `Returns_Fact` to avoid ambiguity

---

## 🧮 Calculated Columns
The following calculated columns were created:

- **Profit**  
  `Sales Amount – Cost`

- **Return Flag**  
  Identifies whether a transaction was *Returned* or *Not Returned*

- **Customer Full Name**  
  Concatenation of first and last names for reporting clarity

---

## 📐 Measure Management
A **dedicated Measure Table** was created to organize all DAX measures, improving:
- Readability
- Maintainability
- Professional modeling standards

---

## 📊 Key Measures Implemented
- **Total Sales**
- **Total Cost**
- **Total Profit**
- **Return Rate (%)**
- **Average Sale per Transaction**
- **Total Returns**

Iterator functions like `SUMX` and `AVERAGEX` were used where row-level context was required.

---

## ⏳ Time Intelligence Analysis
Advanced time-based metrics were implemented using DAX:

- **Year-to-Date (YTD) Sales**
- **Running Total Sales**
- **Year-over-Year (YoY) Sales Growth**
- **Month-over-Month (MoM) Sales Difference**

These metrics enable trend analysis, performance comparison, and growth tracking.

---

## 🎛️ Filter Context & DAX Behavior
Key DAX functions used:
- `CALCULATE`
- `ALL`
- `FILTER`

These functions were used to:
- Compare filtered vs unfiltered sales
- Analyze high-value transactions
- Demonstrate filter context manipulation

---

## 🔀 Sales Categorization
Sales values were categorized into:
- **Low**
- **Medium**
- **High**

Using the `SWITCH` function, enabling simplified business interpretation.

---

## 📈 Reporting Strategy
✔ **Only Matrix visuals were used**, as per project requirements.

### Matrix Reports Included:
- Sales and Profit by Region and Month
- Time Intelligence metrics (YTD, Running Total, YoY)
- Customer Segment analysis with Average Sales

---

## 💼 Business Value
This project demonstrates how advanced DAX and proper data modeling can:
- Transform raw transactional data into actionable insights
- Support enterprise-level reporting
- Improve decision-making through accurate analytics

---

## 🧩 Tools & Technologies
- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Star Schema Data Modeling**
- **Matrix-Based Analytics**

---

## ✅ Project Deliverables
- `.pbix` Power BI file
- Advanced DAX calculations
- Clean data model
- Matrix-based analytical output
- Professional documentation

---

## 📌 Conclusion
The **DAX Depo project** showcases a complete Power BI analytical workflow—from data modeling to advanced DAX calculations and business insights. It reflects real-world BI practices and demonstrates strong command over Power BI, DAX, and analytical thinking.

---

## 🚀 Author
**Jaden**  
Data Analyst | Power BI & DAX Enthusiast  

---

> *“Bring on your coding attitude.”*
