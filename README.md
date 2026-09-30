# JCars Logistics Sales & Operations Analytics

## Project Overview

This project uses **Power BI** to analyse JCars Logistics' vehicle sales and operational data.

The analysis focuses on:

* Sales and revenue performance
* Profitability and costs
* Vehicle performance
* Regional and branch performance
* Customer behaviour
* Delivery and logistics
* Payment and transaction exceptions

## Dataset

The dataset contains **276 records and 32 columns**, with each row representing one vehicle sales transaction.

Key areas include:

* Customer information
* Vehicle details
* Sales and financial data
* Location information
* Payment and delivery data
* Customer ratings and returns

## Data Preparation

The dataset was cleaned and validated to address issues such as:

* Inconsistent dates and IDs
* Multiple currencies
* Invalid ages and vehicle years
* Inconsistent categories
* Missing and unreliable financial values
* Conflicting payment and delivery statuses

All monetary values were standardised to **KES** using the applicable exchange rates.

## Data Model

The cleaned dataset was transformed into a **Star Schema**.

### Fact Table

`FactSales`

### Dimension Tables

* `DimDate`
* `DimCustomer`
* `DimVehicle`
* `DimLocation`
* `DimSalesRep`
* `DimPayment`
* `DimLeadSource`
* `DimDeliveryStatus`

```text
DimCustomer ──┐
DimVehicle ───┤
DimDate ──────┤
DimLocation ──┤
DimSalesRep ──┼── FactSales
DimPayment ───┤
DimLeadSource ┤
DimDelivery ──┘
```

## Key Business Questions

* Which vehicle categories generate the most revenue?
* Which categories are profitable?
* Which regions and branches perform best?
* Where are delivery and logistics challenges occurring?
* How concentrated is revenue among high-value customers?
* Which transactions require further investigation?

## Power BI Report

The dashboard contains five main sections:

1. **Business Overview**
2. **Product & Sales Performance**
3. **Regional & Branch Analysis**
4. **Customers & Sales Channels**
5. **Operations & Exceptions**

## Key Findings

* Total revenue was approximately **KSh 1.48 billion**.
* The top 10 customers contributed approximately **KSh 299.3 million**.
* Some vehicle categories recorded negative gross profit margins.
* Nairobi recorded an average delivery time of **26.29 days**, compared with **15.18 days** overall.
* **14 payment and delivery inconsistencies** were identified.

## Tools Used

* Microsoft Power BI
* Power Query
* GitHub
  

## Key Learning

The project strengthened my skills in data cleaning, Power Query, data modelling, DAX, dashboard development, data validation and business-focused analysis.

> **Good analytics starts with understanding and validating the data before building the dashboard.**


Data Science & Analytics | Power BI | Data Analytics
