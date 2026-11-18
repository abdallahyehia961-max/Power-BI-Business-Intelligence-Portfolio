# Power BI Business Intelligence Portfolio

A collection of Power BI dashboards focused on business performance,
sales analytics, customer behavior, order management, and shipping
operations. The Supply Chain Analytics project is supported by a SQL
Server data warehouse with Bronze, Silver, and Gold layers.

## Portfolio Overview

  -----------------------------------------------------------------------
  Dashboard                           Focus
  ----------------------------------- -----------------------------------
  Executive Overview                  Overall sales, profitability,
                                      orders, products, and markets

  Sales & Market Analysis             Market performance, discounts,
                                      profit, departments, and
                                      salespeople

  Customer & Order Analysis           Customer segments, geography, order
                                      value, and order outcomes

  Shipping & Operational Performance  Delivery status, late deliveries,
                                      shipping modes, and shipping
                                      timelines

  Loan Analysis                       Loan portfolio, loan origination,
                                      maturity, and interest rates
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# Project 1 --- Supply Chain Data Warehouse & Power BI Analytics

## Project Overview

This project transforms supply chain data into an analytics-ready
dimensional model and presents business insights through interactive
Power BI dashboards.

### Data Warehouse Layers

-   **Bronze Layer:** source data tables.
-   **Silver Layer:** cleaned and prepared data.
-   **Gold Layer:** dimensional model prepared for reporting and
    analysis.

### Gold Layer Data Model

The reporting model follows a star-schema structure:

  Table            Description
  ---------------- ------------------------------------------------------
  `FactOrders`     Order and order-line metrics used for analysis
  `DimCustomers`   Customer details and customer segments
  `DimProducts`    Product, category, and department attributes
  `DimSalesman`    Salesperson details and commission attributes
  `DimDate`        Calendar and date attributes for time-based analysis

### Data Quality & Validation

SQL validation and reconciliation checks were used during the warehouse
workflow to review row counts, key uniqueness, missing values, invalid
values, and consistency between layers.

## Dashboard 1 --- Executive Overview

Provides a high-level view of the business:

-   Booked Net Sales
-   Gross Sales
-   Profit Margin
-   Total Orders
-   Reported Profit
-   Top 10 Products by Sales
-   Net Sales by Customer Segment
-   Monthly Net Sales Trend
-   Sales by Market
-   Orders by Status
-   Sales by Product Category

![Executive Overview](screenshots/executive-overview.png)

## Dashboard 2 --- Sales & Market Analysis

Analyzes sales performance across markets, regions, departments, and
salespeople:

-   Gross Sales vs. Net Sales by Market
-   Discount Analysis by Market
-   Top 10 Salespeople by Net Sales
-   Profit by Market
-   Sales by Department
-   Net Sales by Region

![Sales & Market Analysis](screenshots/sales-market-analysis.png)

## Dashboard 3 --- Customer & Order Analysis

Explores customer distribution and order behavior:

-   Customer Distribution by Segment
-   Customers by Country
-   Average Order Value by Customer Segment
-   Top 10 Customers by Net Sales
-   Net Sales by Customer State
-   Completed vs. Canceled Orders by Segment

![Customer & Order Analysis](screenshots/customer-order-analysis.png)

## Dashboard 4 --- Shipping & Operational Performance

Evaluates shipping performance and delivery operations:

-   Shipped Orders
-   Eligible Shipping Orders
-   Late Orders
-   Late Delivery Rate
-   Average Shipping Days
-   Orders by Delivery Status
-   Late Delivery Rate by Region
-   Actual vs. Scheduled Shipping Days
-   Average Shipping Days by Shipping Mode
-   On-Time vs. Late Orders by Market
-   Net Sales by Shipping Date Trend

![Shipping & Operational
Performance](screenshots/shipping-operational-performance.png)

------------------------------------------------------------------------

# Project 2 --- Loan Analysis Dashboard

A separate Power BI dashboard focused on loan portfolio composition and
loan performance.

### Key Metrics & Visuals

-   Customers With Loans
-   Total Loans
-   Average Interest Rate
-   Average Loan Duration
-   Total Loan Amount
-   Average Loan Amount
-   Loan Portfolio by Type
-   Loan Origination Trend
-   Loan Maturity Schedule
-   Average Interest Rate by Loan Type

![Loan Analysis](screenshots/loan-analysis.png)

------------------------------------------------------------------------

## Tools & Technologies

-   **Microsoft SQL Server** --- database and data warehouse
-   **T-SQL** --- data preparation, validation, and transformation
-   **Power BI Desktop** --- data modeling and dashboard development
-   **DAX** --- measures and business calculations
-   **Dimensional Modeling** --- Bronze, Silver, and Gold layers;
    star-schema reporting model

## Repository Structure

``` text
Power-BI-Business-Intelligence-Portfolio/
├── README.md
└── screenshots/
    ├── executive-overview.png
    ├── sales-market-analysis.png
    ├── customer-order-analysis.png
    ├── shipping-operational-performance.png
    └── loan-analysis.png
```

## How to Explore

1.  Browse the dashboard screenshots directly in this repository.
2.  Open the corresponding `.pbix` files in Power BI Desktop when the
    report files are added.
3.  Review the SQL scripts when the warehouse scripts are added to the
    repository.

## Notes

This repository currently documents the projects and includes their
dashboard screenshots. The screenshots are previews; interactive Power
BI reports, SQL scripts, and source data should be added separately if
they are intended to be shared.

Before publishing, make sure that no credentials, connection strings,
confidential business data, or personally identifiable information are
included.
