## TastyBytes: Pricing & Profitability Analysis (2023–2025)

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-4CAF50?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

> An end-to-end **Power BI case study** analyzing pricing strategies, product profitability, and discount effectiveness for TastyBytes — a fictional food & beverage brand — across a 2-year period (Jul 2023 – Jul 2025).

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Problem Statement](#-problem-statement)
- [Dataset](#-dataset)
- [Dashboard Preview](#-dashboard-preview)
- [Tools & Technologies](#-tools--technologies)
- [Key KPIs & Metrics](#-key-kpis--metrics)
- [Key Insights](#-key-insights)
- [Recommendations](#-recommendations)

---

## 🎯 Project Overview

TastyBytes operates across three product categories — **Beverages, Meals, and Snacks** — with 15 unique products. This project analyzes **₹1.41M in revenue** across 2 years to answer critical business questions around **pricing efficiency, discount effectiveness, and category-level profitability**.

The final deliverable is a **4-page interactive Power BI dashboard** designed for executive decision-making.

---

## ❓ Problem Statement

TastyBytes' leadership team needs data-driven answers to:

1. **Which products and categories drive the most profit?**
2. **Are discounts actually helping sales, or eroding margins?**
3. **How stable is profitability across time?**
4. **Which products are underpriced or overpriced?**
5. **Where should the company focus to maximize profit?**

---

## 📊 Dataset

| Attribute | Details |
|-----------|---------|
| **Time Period** | July 2023 – July 2025 |
| **Records** | ~9,600+ transactions |
| **Categories** | Beverages, Meals, Snacks |
| **Products** | 15 unique items |
| **Key Fields** | Date, Product, Category, Price, Cost, Discount, Units Sold, Revenue |

---

## Dashboard Preview 

<img width="1257" height="702" alt="Screenshot 2026-08-21 160921" src="https://github.com/user-attachments/assets/289e7b22-e156-4e93-9daa-c4236d45cde1" />

<img width="1241" height="702" alt="Screenshot 2026-08-21 161052" src="https://github.com/user-attachments/assets/9cf13a70-98e7-422d-ad89-dd217b9e8e6b" />

<img width="1251" height="685" alt="Screenshot 2026-08-21 161219" src="https://github.com/user-attachments/assets/66bee61e-b41c-49ca-88cd-5762f331ab8a" />

<img width="1243" height="699" alt="Screenshot 2026-08-21 161354" src="https://github.com/user-attachments/assets/045e8299-5c14-47b2-b739-026bc651027e" />


## 🛠️ Tools & Technologies

- **Power BI Desktop** — Dashboard development & visualization
- **Power Query (M)** — Data cleaning & transformation
- **DAX** — Custom measures & calculated columns
- **Excel / CSV** — Data source
- **GitHub** — Version control & portfolio hosting

---

## 📈 Key KPIs & Metrics

| KPI | Value | Purpose |
|-----|-------|---------|
| **Total Revenue** | ₹1.41M | Overall top-line performance |
| **Total Cost** | ₹618K | Cost of goods sold |
| **Profit Margin** | 56.20% | Net profitability |
| **Gross Profit Margin** | 58.87% | Pre-discount profitability |
| **Average Order Value** | ₹282.39 | Customer spending pattern |
| **Average Discount** | 6.23% | Pricing strategy indicator |
| **Discount Impact** | 2.67% | Revenue erosion due to discounts |
| **Units Sold** | 9,672 | Sales volume |

### 🧮 Sample DAX Measures

```DAX
Total Revenue = SUMX(Sales, Sales[Units Sold] * Sales[Selling Price])

Profit Margin = 
DIVIDE([Total Revenue] - [Total Cost], [Total Revenue], 0)

Discount Impact = 
DIVIDE([Total Gross Revenue] - [Total Revenue], [Total Gross Revenue], 0)

```

**Key Insights**

1. Discount resulted in 2.67% decrease in profit margin.
2. Chicken Biriyani, Butter Chicken and Chicken Nuggets generates high revenue (500K) but low profit
3. Green Tea, Masala Chai and Samosa generates higher profit even with higher discount due to low cost of production (<15K)
4. Chicken products suffer low profit due to the higher cost of production
5. French Fries and Lemonade generate moderate revenue with higher profit
6. Sales of majority of the products (except 5) do not rise with discount indicates price-inelastic demand


**Business Recommendations**
1. Introduce exclusive combo offers for Chicken Biriyani, Butter Chicken and Chicken Nuggets which reduce the average discount indirectly by 1-2%, thereby increase profit margin by 2-3%
2. Increase the price of the products whose sales is independent of increased discounts by 10% to increase profit by 5-10%
3. Launch bundle offers with French Fries and Lemonade to reduce average discount by 1-2%, thereby increase profit margin by 1-2%
4. Investigate the factors which contributes to the rising cost of products involving chicken which in turn reduces profit margin of Chicken Biriyani, Butter Chicken and Chicken Nuggets. Take actions to reduce cost by 8-10% via supplier negotiation and portion optimization which increase profit by 2-3%
5. Launch bundle offers for Beverage products which indirectly reduce average discount by 1-2%, thereby increase profit margin by 1-2%
6. Increase the price of the products whose sales marginally depend on increased discount by 6-8% to increase profit by 3-6% 
