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

## DAX Calculations

### Paid Spend

```dax
Paid Spend =
CALCULATE(
    [Total Spend],
    PurchasingData[Status] = "Paid"
)
```

This measure uses `CALCULATE()` to filter purchasing transactions and calculate the total amount associated with Paid status.

Additional measures were developed to analyze spending, budget utilization, and purchase order activity.

## Dashboard Visualizations

### 1. Purchasing Performance KPIs

Created KPI cards to summarize purchasing expenditures, budget variance, and purchase order counts.

### 2. Budget vs. Actual Spend by Department

Developed a comparison chart to evaluate purchasing expenditures against departmental budgets.

**Purpose:** Identify spending differences and support departmental budget monitoring.

### 3. Monthly Spending Trends

Created a line chart to visualize purchasing expenditures over time.

**Purpose:** Examine spending fluctuations and purchasing trends.

### 4. Spending by Vendor

Developed a bar chart comparing purchasing expenditures across vendors.

**Purpose:** Identify vendors representing larger portions of total purchasing expenses.

## Business Questions Explored

1. How much has been spent on purchasing activities?
2. Which departments have the highest purchasing expenditures?
3. How does actual spending compare with allocated budgets?
4. Which vendors account for the largest purchasing expenses?
5. How does purchasing activity change over time?
6. How many purchase orders are represented in the dataset?

## Skills Demonstrated

- Power BI Dashboard Development
- DAX Measures and Calculations
- Business Intelligence Reporting
- KPI Development
- Budget Variance Analysis
- Procurement Analytics
- Financial Data Visualization
- Purchasing Trend Analysis

## Project Takeaways

Through this project, I strengthened my ability to use Power BI and DAX to transform purchasing transaction data into meaningful financial insights.

I practiced developing reusable calculations, analyzing departmental spending, comparing expenditures against budgets, and creating visualizations to communicate purchasing performance.

This project demonstrates how business intelligence tools can support financial transparency and data-driven decision-making.

## Future Improvements

- Develop vendor-level drill-through analysis
- Expand monthly and quarterly purchasing trends
- Incorporate payment processing performance metrics
- Add additional budget monitoring indicators
- Explore automated data refresh capabilities

## Author

**Holly Lam**

MBA Candidate | Business Analytics Concentration

[GitHub Portfolio](https://github.com/honguyen-lgtm)
