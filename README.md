# Mortgage Trading & Profitability Analysis using Power BI

### Project Overview

This project presents a comprehensive analysis of a mortgage loan portfolio designed to support the trading of these assets in the capital markets. The goal is to streamline the process from identifying trade-ready loans to executing sales and analyzing profitability. This Power BI dashboard provides a multi-faceted view of the loan data, enabling data-driven decisions for loan officers, trade managers, and executives.

The analysis leverages loan-level data, including status, balances, and bids from various investors, to provide actionable insights across five key areas: **Loan Status Tracking**, **Loan Balance Forecasting**, **Trade Analysis**, **Trade Execution**, and **Profitability Analysis**.

###  Key Features & Analyses

The dashboard is structured into five distinct report pages, each serving a specific purpose in the mortgage trading lifecycle.

#### 1.  Loan Status Dashboard
This section provides a high-level overview of the loan pipeline to quickly identify which loans are ready for trading.
* **Purpose:** To monitor the operational readiness of the loan portfolio and quantify the volume of tradable assets.
* **Visuals:** Key Performance Indicators (KPIs) showing the count of loans in different stages (e.g., "Closed - Ready to Trade", "File Sent to Custodian") and a detailed table view for individual loan tracking.

#### 2.  Loan Balance & Amortization
This page forecasts the future principal balance of each loan, which is critical for accurate trade pricing.
* **Purpose:** To calculate the scheduled principal balance for the upcoming month. This is achieved by calculating the principal portion of the next payment using the **PPMT (Principal Payment) DAX function** in Power BI.
* **Analysis:** An amortization schedule is generated for each loan, providing a precise forward-looking balance for trade settlement.

#### 3.  Trade Analysis
Here, bids from various investors are analyzed to determine the optimal trade strategy.
* **Purpose:** To evaluate investor bids, calculate potential trade amounts, and determine the weighted average price and trade premium for the loan pool.
* **Calculations:**
    * **Trade Amount:** Calculated based on the loan's outstanding balance.
    * **Trade Premium:** The amount offered by an investor above the loan's face value, indicating strong demand.
    * **Weighted Price:** The average price of the loans, weighted by their outstanding balance, providing a key metric for overall portfolio valuation.

#### 4.  Trade Execution Summary
This is an executive-level dashboard designed to facilitate the final trade decision.
* **Purpose:** To present a clear, concise summary of the proposed trade for management approval.
* **Visuals:** Summarizes the total **Trade Amount** and **Trade Premium** for each bidding investor. Bar charts and tables are used to compare bids and highlight the most profitable opportunities.

#### 5.  Profitability & Key Influencer Analysis
This final section dives into the drivers of profitability to inform future loan origination strategies.
* **Purpose:** To analyze the factors influencing the profitability of the loans being sold.
* **Metrics:**
    * **Loan Profit Margin:** The actual profit made on the sale of the loan.
    * **Target Profit Margin:** The expected profit margin.
* **Advanced Analytics:** The **Key Influencers** visual in Power BI is used to identify the primary drivers of price. The analysis revealed that **Origination Charges**, **Loan-to-Value (LTV) Ratio**, and **Debt-to-Income (DTI) Ratio** are significant factors influencing the final trade price.

### Tools Used
* **Data Analysis & Calculations:** Microsoft Power BI (DAX)
* **Data Source:** CSV files containing loan data, status, balances, and investor bids.
