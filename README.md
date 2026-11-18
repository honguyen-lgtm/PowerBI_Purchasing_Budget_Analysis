# Purchasing & Budget Analysis Dashboard | Power BI

## Project Overview

This project demonstrates the use of Microsoft Power BI to analyze purchasing transactions, monitor expenditures, and evaluate budget performance across departments, vendors, and organizational sites.

I developed an interactive dashboard using DAX (Data Analysis Expressions) to calculate key purchasing metrics, visualize spending patterns, and compare actual expenditures against allocated budgets.

**Objective:** Transform purchasing data into actionable insights to support financial monitoring, budget management, and procurement decision-making.

## Interactive Dashboard

[View Power BI Dashboard](https://app.powerbi.com/groups/me/reports/bafc2287-92f7-470f-b0cb-ac794eb5821e)

*Note: Access may require Power BI permissions.*

## Tools & Technologies

- **Power BI:** Interactive dashboards and reporting
- **DAX:** Custom measures and calculations
- **Data Visualization:** KPI cards, bar charts, and line charts
- **Financial Analysis:** Budget variance and spending analysis
- **Data Analysis:** Purchasing trends and vendor comparisons

## Dataset Overview

The dataset includes purchasing transaction information such as:

- Purchase Order Number
- Purchase Date
- Department and Site
- Vendor and Purchasing Category
- Quantity and Unit Price
- Total Amount and Budget
- Payment Status
- Payment Days

## Key Performance Indicators (KPIs)

I developed DAX measures to calculate and monitor purchasing performance.

| KPI | Description |
|---|---|
| Total Spend | Total purchasing expenditures |
| Paid Spend | Total amount marked as Paid |
| Pending Spend | Total amount marked as Pending |
| Total Budget | Total allocated purchasing budget |
| Budget Variance | Difference between budget and actual expenditures |
| Budget Used % | Percentage of budget utilized |
| PO Count | Number of purchase orders |
| Average PO Amount | Average purchase order amount |
| IT Department Spend | Total purchasing expenses for the IT department |

 DAX Calculations

Paid Spend

```dax
Paid Spend =
CALCULATE(
    [Total Spend],
    PurchasingData[Status] = "Paid"
)
```

This measure
