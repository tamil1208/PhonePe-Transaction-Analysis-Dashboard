# PhonePe Transaction Analysis Dashboard 📊

An interactive Power BI dashboard analyzing digital payment transactions on PhonePe — covering transaction volume, value trends, success rates, user demographics, and payment behavior across services, regions, and time.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/status-complete-brightgreen)

---

## 📌 Overview

This project explores digital payment data to uncover patterns in how users transact on PhonePe — which services drive the most value, when transactions peak, how success rates trend over time, and which age groups are most active. It's designed as a single-page executive dashboard for quick, at-a-glance decision-making.

## 🎯 Objective

- Track overall transaction health (volume, value, and success rate) at a glance
- Identify month-over-month growth or decline in transactions and revenue
- Understand transaction distribution across services, regions, and time
- Analyze user behavior by age segment and weekday vs. weekend activity
- Enable filtering by month and payment status for deeper drill-down

## 🖥️ Dashboard Features

**KPI Cards**
- Total Transaction Value
- Total Transactions
- Success Rate
- Total Users
- Month-over-Month % change for Transactions, Transaction Value, and Success Rate

**Visuals**

| Visual | Insight |
|---|---|
| Line Chart | Monthly trend of transaction value and volume |
| Column Chart | Transaction value by service type |
| Column Chart | Transaction value by region/state |
| Donut Chart | Transaction split — weekday vs. weekend |
| Donut Chart | User count by age segment |

**Interactivity**
- Slicers for **Month** and **Payment Status**
- Cross-filtering across all visuals
- Custom tooltip pages for deeper context on hover

**Key Insight Highlighted**
> On weekdays, the number of transactions is at its maximum — pointing to stronger usage during the work week compared to weekends.

## 🗂️ Data Model

The report is built on a star-schema-style model with four tables:

- `All_Transactions` — fact table with transaction-level records (service, value, status, date)
- `All_Users` — user master data (user ID, age segment)
- `Date_Table` — dedicated date dimension for time intelligence (month, weekend flag)
- `Measures` — centralized DAX measures table

### Key DAX Measures
- `Total_transactions`
- `Total_transaction_value`
- `Success_rate`
- `Total_users`
- `Total_trans_MOM%`
- `Trans_value_MOM%`
- `Success_rate_MOM%`

## 🛠️ Tools & Skills Used

- **Power BI Desktop** — data modeling, DAX, report design
- **DAX** — time intelligence (MoM %), success rate calculations
- **Data Modeling** — star schema with a dedicated date and measures table
- **UX/Report Design** — custom theming, branded layout, KPI-first storytelling

<img width="580" height="327" alt="Screenshot 2026-08-06 144544" src="https://github.com/user-attachments/assets/93eaf4f9-8a2e-4bad-9d85-1cbdb5d7515a" />
