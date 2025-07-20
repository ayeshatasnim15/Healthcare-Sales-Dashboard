# 🏥 Healthcare Sales Dashboard

> **A comprehensive Power BI dashboard analyzing pharmaceutical sales performance and customer insights**

**Developed by:** [Ayesha Tasnim](https://www.linkedin.com/in/tasnimayesha/)  
**Location:** Bhubaneswar, Odisha, India  
**Project Type:** Data Analytics & Business Intelligence

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Dashboard Pages](#dashboard-pages)
- [Data Architecture](#data-architecture)
- [Key Insights](#key-insights)
- [Technical Implementation](#technical-implementation)
- [Business Impact](#business-impact)
- [Getting Started](#getting-started)
- [Contact](#contact)

---

## 🎯 Project Overview

This Healthcare Sales Dashboard is a comprehensive Power BI solution designed to transform pharmaceutical sales data into actionable business intelligence. The dashboard provides real-time insights into sales performance, customer demographics, product performance, and market trends across multiple dimensions.

### **Business Objectives**
- 📊 Monitor key performance indicators (KPIs) in real-time
- 👥 Analyze customer behavior and demographics
- 💊 Track product performance and profitability
- 🌍 Understand geographical sales distribution
- 📈 Identify growth opportunities and trends

---

## ✨ Key Features

### **📱 Interactive Dashboard**
- **Real-time KPI monitoring** with year-over-year comparisons
- **Dynamic filtering** across multiple dimensions
- **Responsive design** optimized for various screen sizes
- **Drill-down capabilities** for detailed analysis

### **📊 Advanced Analytics**
- **Predictive insights** based on historical trends
- **Customer segmentation** analysis
- **Product performance** benchmarking
- **Geographic performance** mapping

### **🎨 Modern UI/UX**
- **Clean, professional interface** with healthcare-themed design
- **Intuitive navigation** with sidebar menu
- **Color-coded metrics** for quick interpretation
- **Mobile-responsive** layout

---

## 📄 Dashboard Pages

### **🏠 Home Dashboard**

![Home Dashboard](./Healthcare%20Sales%20Dashboard_Home.jpg)

**Core KPIs & Performance Metrics:**

| Metric | Current Value | YoY Growth |
|--------|---------------|------------|
| **Total Revenue** | $64.7M | +1,961% |
| **Total Profit** | $53.0M | +1,949% |
| **Quantity Sold** | 245K units | +1,951% |
| **Total COGS** | $11.7M | +2,019% |

**Key Visualizations:**
- **Revenue by Drug Name** (Top 5 & Bottom 5 performers)
- **Revenue by Customer** (Top 5 & Bottom 5 customers)
- **Revenue Distribution** by Buyer Type and Gender
- **Interactive filters** for different metrics

### **🔍 Insights Dashboard**

![Insights Dashboard](./Healthcare%20Sales%20Dashboard_Insights.jpg)

**Customer & Market Analysis:**

| Metric | Value |
|--------|-------|
| **Total Customers** | 200 |
| **Average Revenue per Customer** | $323.37K |
| **Total Transactions** | 15.44K |
| **Average Revenue per Transaction** | $4.19K |

**Demographic Insights:**
- **Age Group Performance:** 51+ age group leads with $34M revenue
- **Gender Distribution:** Male customers generate $30M vs Female $21M
- **Geographic Performance:** North America shows highest revenue concentration

**Temporal Analysis:**
- **Monthly Trends:** Peak performance in March-May and September-October
- **Quarterly Performance:** Consistent revenue across all quarters
- **Daily Patterns:** Day-of-week analysis for each drug category

---

## 🗄️ Data Architecture

### **Data Sources**
The dashboard integrates three primary datasets:

#### **1. Customers Table**
```sql
- CustomerID (Primary Key)
- FirstName, LastName
- Age, Gender, Country
- OtherCustomerInfo (Tags)
```

#### **2. Drugs Lookup Table**
```sql
- DrugID (Primary Key)
- DrugName, UnitSalesPrice
- CostOfProduction, Treats
- RegulatoryComplianceID
```

#### **3. Sales Transactions Table**
```sql
- SaleID (Primary Key)
- DrugID, CustomerID (Foreign Keys)
- UnitsSold, SaleDate
- BuyerType
```

### **Data Relationships**
- **One-to-Many:** Customer → Sales Transactions
- **One-to-Many:** Drug → Sales Transactions
- **Star Schema:** Centralized fact table with dimension tables

---

## 💡 Key Insights

### **🏆 Top Performers**
- **Best-Selling Drug:** Lisinopril ($3.2M revenue)
- **Top Customer:** David Johnson ($3.6M revenue)
- **Most Profitable Segment:** 51+ age group ($34M)

### **📈 Growth Opportunities**
- **Underrepresented Demographics:** 0-20 age group ($3M)
- **Geographic Expansion:** Focus on high-potential regions
- **Product Diversification:** Leverage top-performing drug categories

### **🎯 Strategic Recommendations**
1. **Customer Retention:** Implement loyalty programs for top customers
2. **Market Expansion:** Target underrepresented age groups and regions
3. **Product Strategy:** Increase focus on high-performing drugs
4. **Seasonal Planning:** Align marketing with peak performance periods

---

## ⚙️ Technical Implementation

### **Tools & Technologies**
- **Power BI Desktop** - Primary dashboard development
- **DAX (Data Analysis Expressions)** - Advanced calculations
- **Power Query** - Data transformation and cleaning
- **M Language** - Data modeling

### **Key DAX Measures**
```dax
// Revenue Calculation
Total Revenue = SUMX(Sales, Sales[UnitsSold] * RELATED(Drugs[UnitSalesPrice]))

// Year-over-Year Growth
YoY Growth = 
VAR CurrentYear = [Current Year Revenue]
VAR PreviousYear = [Previous Year Revenue]
RETURN DIVIDE(CurrentYear - PreviousYear, PreviousYear, 0)
```

### **Performance Optimizations**
- **Incremental refresh** for large datasets
- **Optimized DAX measures** for faster calculations
- **Efficient data model** with proper relationships

---

## 📊 Business Impact

### **Quantifiable Benefits**
- **1,961% revenue growth** year-over-year
- **Real-time monitoring** of 200+ customers
- **15,000+ transactions** analyzed
- **$64.7M total revenue** tracked

### **Operational Improvements**
- **Faster decision-making** with real-time insights
- **Improved customer targeting** based on demographics
- **Optimized inventory management** through product analysis
- **Enhanced marketing ROI** with performance tracking

---

## 🚀 Getting Started

### **Prerequisites**
- Power BI Desktop (latest version)
- Access to the source datasets
- Basic understanding of DAX and Power Query

### **Installation Steps**
1. **Clone the repository**
   ```bash
   git clone git@github.com:ayeshatasnim15/Healthcare-Sales-Dashboard.git
   ```

2. **Open the Power BI file**
   - Launch Power BI Desktop

3. **Connect to data sources**
   - Update data source paths if needed
   - Refresh data connections

4. **Explore the dashboard**
   - Navigate between Home and Insights pages
   - Use interactive filters and drill-downs

### **Customization**
- **Modify data sources** in Power Query Editor
- **Adjust visualizations** in Report View
- **Update DAX measures** in Data View
- **Customize themes** in Format pane

---

## 📞 Contact

**Ayesha Tasnim**  
📧 [LinkedIn](https://www.linkedin.com/in/tasnimayesha/)  
🌐 [GitHub Profile](https://github.com/ayeshatasnim15/)  
📍 Bhubaneswar, Odisha, India

---

## 📄 License

This project is created for educational and portfolio purposes. All rights reserved.

---

**⭐ If you find this project helpful, please give it a star!**

