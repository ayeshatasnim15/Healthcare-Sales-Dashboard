# 🏥 Healthcare Sales Dashboard

**Developed by: [Ayesha Tasnim](https://www.linkedin.com/in/tasnimayesha/)**  
📍 Bhubaneswar, Odisha, India

---

## 📌 Project Objective

The goal of this project is to create a **comprehensive and interactive Power BI dashboard** analyzing **medicine sales data from 2022 and 2023**. This dashboard enables stakeholders to understand key performance metrics, customer demographics, and sales trends to support **strategic decision-making**.

---

## 📂 Dataset Overview

The analysis is based on three primary datasets in CSV format:

### 🔸 1. Customers Table

| Column             | Data Type | Description                                        |
|--------------------|-----------|----------------------------------------------------|
| `CustomerID`       | Integer   | Unique identifier for each customer               |
| `FirstName` / `LastName` | String | Customer’s name                                |
| `Age`              | Integer   | Age of the customer                               |
| `Gender`           | String    | Gender identity                                   |
| `Country`          | String    | Customer’s country of residence                   |
| `OtherCustomerInfo`| String    | Additional tags (e.g., New Customer, Frequent Buyer) |

### 🔸 2. Drugs Lookup Table

| Column                  | Data Type | Description                                |
|-------------------------|-----------|--------------------------------------------|
| `DrugID`                | Integer   | Unique identifier for each drug           |
| `RegulatoryComplianceID`| Integer  | Compliance category ID                     |
| `DrugName`              | String    | Name of the drug                          |
| `UnitSalesPrice`        | Float     | Selling price per unit                    |
| `CostOfProduction`      | Float     | Production cost per unit                  |
| `Treats`                | String    | Medical condition treated                 |

### 🔸 3. Sales Transactions Table

| Column       | Data Type | Description                          |
|--------------|-----------|--------------------------------------|
| `SaleID`     | Integer   | Unique ID for each transaction       |
| `DrugID`     | Integer   | Drug sold                            |
| `CustomerID` | Integer   | Customer who made the purchase       |
| `UnitsSold`  | Integer   | Quantity sold                        |
| `SaleDate`   | Date      | Date of sale                         |
| `BuyerType`  | String    | Type of buyer (e.g., Seller, User)   |

---

## 📊 Dashboard Overview

The Power BI dashboard is divided into **two key pages**:

### 📄 Page 1: Home

![Home Dashboard](./Healthcare%20Sales%20Dashboard_Home.jpg)

**Highlights:**

- **KPIs:**  
  - Total Quantity Sold: `245,000` units  
  - Revenue: `$65M`  
  - Profit: `$53M`  
  - Total COGS: `$11.69M`

- **Visuals:**  
  - **Top Revenue-Generating Drug:** Lisinopril (`$3.2M`)  
  - **Top Customer:** David Johnson (`$3.6M`)  
  - **Profit by Buyer Type:** Sellers contribute `87.75%` of total profit

---

### 📄 Page 2: Insights

![Insights Dashboard](./Healthcare%20Sales%20Dashboard_Insights.jpg)

**Demographic & Regional Insights:**

- **Total Customers:** 200  
- **Avg Revenue per Customer:** `$323,000`  
- **Total Transactions:** `15,000`  
- **Avg Revenue per Transaction:** `$4,200`

- **Sales by Country:**  
  - Top: 🇨🇦 Canada (`$29M`)  
  - Lowest: 🇫🇷 France (`$5M`)

- **Sales by Gender:**  
  - Male: `$30M`, Female: `$21M`, Others: `$12M`

- **Sales by Age Group:**  
  - Highest: `51+` (`$34M`)  
  - Lowest: `0–20` (`$3M`)

- **Year-over-Year Growth:**  
  - 2022: `$3M` → 2023: `$62M`

- **Quarterly Sales Trends:**  
  - Q1: `$15.86M`, Q2: `$15.35M`, Q3: `$16.40M`, Q4: `$16.06M`

---

## 💡 Key Recommendations

1. **Prioritize Lisinopril** in future campaigns.
2. **Engage top customers** like David Johnson with loyalty programs.
3. **Expand outreach to underrepresented groups**, especially young and female customers.
4. **Boost presence in high-revenue countries** such as Canada and Australia.
5. **Align promotions with seasonal trends** based on quarterly performance.

---

## 🚀 Key Learnings

- Gained expertise in **Power BI, DAX, and data storytelling**.
- Enhanced skills in **ETL (Extract, Transform, Load)** and dashboard design.
- Learned how to convert raw data into **actionable business insights**.

---

## 🤝 Let’s Connect

I’ve completed **10+ Power BI projects** and am currently looking for **internships or full-time roles** in **Data Analytics / Business Intelligence**.

📫 Reach out via [LinkedIn](https://www.linkedin.com/in/tasnimayesha/)  
📬 Or connect via GitHub Issues for feedback and collaboration!

---

> **© 2025 Ayesha Tasnim** — All rights reserved.
