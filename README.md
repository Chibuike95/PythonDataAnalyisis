# CreditSwitch_TakeHome
Transaction analytics project evaluating customer performance, product reliability, and operational efficiency. Computes KPIs such as success rate, failure rate, gross profit, value contribution, and response time. Identifies top customers, least performers per product, and generates a summary table for business insights and decision-making.

Overview

This project analyzes transaction-level data to evaluate customer performance via product engaggement as well as guage operational efficiency across multiple vending products such as Airtime, Data, CableTV, and Electricity.

The analysis focuses on identifying:

- Key performance indicators (KPIs)
- Average response time per product
- Top customer activity trends
- Least performing customers
- Customer-level performance summary table

Dataset Description

Column| Description
Customer ID| Unique Customer ID
Recipient| Beneficiary
Amount| Face value sold
Tranx_Date| Transaction request date
Tranx ID| Unique transaction ID
Updated Time| Fulfilment timestamp
Buying Price| Supply unit cost
Transaction Gateway| Fulfilment channel
Seller Name| Supplier code
Vending Channel| Vending process
Account Type| Customer account type
Location| Source of request
Product| Airtime / Data / CableTV / Electricity
Status|


Question 1 — Identify Key KPIs

Key metrics tracked:

- Transaction Success Rate by Product and Location
- Failure Rate
- Estimated Gross Profit
- Average Response Time

These help measure:

- Customer performance
- Revenue contribution
- System reliability
- Product stability
- Operational efficiency


Question 2 — Average Response Time per Product

Response time is calculated as:

Response Time = Updated Time − Tranx_Date

This helps identify: Slow product fulfilment and Operational Lag


Question 3 — Daily Trend Chart (Top 5 Customers)

Top 5 customers are selected based on total transaction value. the daily trend chart visualizes:

- Usage patterns
- Volume spikes
- Customer drop-off


Question 4 — Top 10 Least Performing Customers per Product

Customers are ranked by highest failure rate per product:

- Airtime
- Data
- CableTV
- Electricity
- Startimes: which was only perculiar to Nigeria Market

This could help to identify:

- Integration issues
- Poor retry logic
- Faulty customer configurations


Question 5 — Customer Summary Table

The final output includes:

Column
Customer ID
Successful Facevalue
Failed FaceValue
Estimated Gross Profit
Successful Count
% Value Contribution
Failure Rate
Airtime Failure Rate
Data Failure Rate
CableTV Failure Rate
Electricity Failure Rate
Pin Failure Rate
Startimes Failure Rate

Calculated Metrics

Gross Profit

Gross Profit = Amount − Buying Price

Failure Rate

Failure Rate = Failed Transactions / Total Transactions

Value Contribution

% Contribution = Customer Value / Total Value


Stack Used:

- Python
- Pandas
- NumPy
- Matplotlib / Plotly
- Jupyter Notebook


Business Value:
This analysis enables: Customer and Product performance monitoring, Revenue contribution tracking, Product stability analysis, Failure diagnostics, Profitability insights and Location Performance
