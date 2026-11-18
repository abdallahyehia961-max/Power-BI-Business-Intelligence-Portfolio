# Business Intelligence Portfolio --- Power BI & SQL Server

A portfolio of Business Intelligence work featuring a **Supply Chain
Data Warehouse** and Power BI dashboards for business performance
analysis.

> **Repository note:** The Loan Analysis dashboard is presented as a
> separate report from the Supply Chain Data Warehouse project. The
> screenshots are included in this repository; add the corresponding
> `.pbix` files and SQL scripts if you want visitors to inspect or run
> the full implementation.

## Projects

### 1. Supply Chain Data Warehouse & Analytics

An end-to-end analytical workflow built around a SQL Server data
warehouse and a Power BI semantic model.

#### Data warehouse architecture

The warehouse is organized into three layers:

-   **Bronze** --- raw source tables.
-   **Silver** --- cleaned and prepared data.
-   **Gold** --- analytics-ready dimensional model.

The Gold layer uses a star-schema design with the following tables:

  Table            Role
  ---------------- ----------------------------------------------
  `FactOrders`     Order-level / order-line business metrics
  `DimCustomers`   Customer attributes and segmentation
  `DimProducts`    Product, category, and department attributes
  `DimSalesman`    Salesperson and commission attributes
  `DimDate`        Calendar attributes for time analysis

The SQL workflow also includes validation and reconciliation checks,
with an audit table used to retain ETL run information.

#### Technology

-   Microsoft SQL Server
-   T-SQL
-   Power BI Desktop
-   DAX measures
-   Dimensional modeling / Star Schema
-   ETL validation and reconciliation

#### Dashboard pages

##### Executive Overview

A high-level view of sales and profitability, including:

-   Booked Net Sales
-   Gross Sales
-   Profit Margin
-   Total Orders
-   Reported Profit
-   Top products by sales
-   Net sales by customer segment
-   Monthly net sales trend
-   Sales by market and product category
-   Orders by status

![Executive Overview](screenshots/executive-overview.png)

##### Sales & Market Analysis

A deeper look at market, discount, profit, and salesperson performance:

-   Gross Sales vs. Booked Net Sales by market
-   Discount analysis by market
-   Top 10 salespeople by net sales
-   Profit by market
-   Sales by department
-   Net sales by region

![Sales & Market Analysis](screenshots/sales-market-analysis.png)

##### Customer & Order Analysis

Customer segmentation and order behavior analysis:

-   Customer distribution by segment
-   Customers by country
-   Average Order Value by customer segment
-   Top 10 customers by net sales
-   Net sales by customer state
-   Completed vs. canceled orders by segment
-   Customer and order filters

![Customer & Order Analysis](screenshots/customer-order-analysis.png)


##### Shipping & Operational Performance

An operational view of shipping efficiency, delivery outcomes, and shipping timelines:

- Shipped Orders
- Eligible Shipping Orders
- Late Orders
- Late Delivery Rate
- Average Shipping Days
- Orders by delivery status
- Late delivery rate by region
- Actual vs. scheduled shipping days by shipping mode
- Average shipping days by shipping mode
- On-time vs. late orders by market
- Net sales by shipping date trend

![Shipping & Operational Performance](screenshots/shipping-operational-performance.png)

### 2. Loan Analysis Dashboard

A separate Power BI dashboard focused on loan portfolio composition,
loan origination, maturity, and interest rates.

The supplied report screenshot highlights:

-   Customers with loans
-   Total loans
-   Average interest rate
-   Average loan duration
-   Total loan amount
-   Average loan amount
-   Loan portfolio by type
-   Loan origination trend
-   Loan maturity schedule
-   Average interest rate by loan type

![Loan Analysis](screenshots/loan-analysis.png)

## Suggested repository structure

``` text
.
├── README.md
├── screenshots/
│   ├── executive-overview.png
│   ├── sales-market-analysis.png
│   ├── customer-order-analysis.png
│   └── loan-analysis.png
├── sql/
│   ├── bronze/
│   ├── silver/
│   ├── gold/
│   └── validation/
└── powerbi/
    ├── supply-chain-analytics.pbix
    └── loan-analysis.pbix
```

The `sql/` and `powerbi/` folders are suggested locations for the
implementation files. Add only files that you are comfortable sharing
publicly, and remove credentials, connection strings, private data, and
other sensitive information before publishing.

## How to view

1.  Open the screenshots in the `screenshots/` folder to preview the
    dashboards on GitHub.
2.  To explore the interactive reports, download and open the relevant
    `.pbix` file in Power BI Desktop once it has been added to the
    repository.
3.  To inspect the warehouse implementation, review the SQL scripts
    after they have been added to the suggested `sql/` folders.

## Data and privacy

The repository package currently contains dashboard screenshots and this
README. It does not include the original source dataset, database
backup, SQL scripts, or Power BI report files. Do not publish
confidential or personally identifiable data.
