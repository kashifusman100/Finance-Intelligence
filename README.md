# Finance-Intelligence
A complete Power BI dashboard analyzing a company’s general ledger, budget performance, accounts receivable/payable, and cash flow. I built the P&amp;L directly from raw debit and credit transactions, created a galaxy schema for the data model, and wrote DAX measures to analyze profitability, working capital, and cash flow.

## Project Description
The dataset is a general ledger export covering two years of financial activity across 5 related fact tables. GL transactions, budget, AR invoices, AP bills, and cash flow connected to a shared chart of accounts, cost centers, vendors, and customers. It came with several data quality issues.

## Business Challenges & Key Questions
Finance needed a single view connecting raw transaction level data to the metrics leadership actually reviews monthly. This project aims to answer key questions:

- What does the full P&L look like (Revenue, COGS, Gross Profit, Opex, Net Income) when built directly from ledger entries?
- Where is actual spend running over or under budget, by department and by account?
- How much cash is tied up in unpaid customer invoices, and how overdue is it?
- How quickly is the company paying its own vendors compared to collecting from customers?
- What does the company's cash flow look like across operating, investing, and financing activity?

## Tools Used
Power BI Desktop (Power Query, Data Modeling, DAX), Excel (source data)

## Links
[Dashboard Screenshots]()

[Power BI File]()

## Quick Dashboard Demo
https://github.com/user-attachments/assets/f6576610-1e47-4ec8-8748-43f6a8356441

## Model View


## Key Insights & Findings

- Revenue & Profitability: Total revenue is $5.81M with a healthy 53.63% gross margin and 27.13% operating margin. Net income grew 129.96% YoY to $1.34M, the growth is not concentrated in one area either; Digital Marketing ($253,975) and APAC's cost center ($212,629) post the strongest operating income despite not being the top revenue generators, meaning efficiency, not just volume, is driving profit.
- Regional Concentration: North America accounts for 56.9% of total revenue ($3.31M), roughly 2.5x each of APAC and Europe individually. The business is currently North America dependent rather than evenly diversified.
Budget Discipline Is Inconsistent: Overall Opex came in under budget ($1.54M actual vs $1.78M budgeted), but that hides real swings underneath, HR Talent underspent its budget by 48.6%, while Engineering-Product and Marketing-Events both ran over budget.
Collections Risk: Of all AR ever generated, $7M of it (roughly 37%) is sitting in the 90+ day aging bucket against $12M paid, a significant chunk of receivables is seriously overdue. Total AR outstanding ($6.77M) also nearly doubles total AP outstanding ($3.48M), so the company is owed far more than it owes.
- DSO/DPO Volatility: Both DSO (425 days) and DPO (471 days) run high, and neither is stable month to month, DPO spiked to over 1,000 days in isolated months (May 2023, Sept 2024). DPO staying slightly above DSO overall is a mild positive for cash flow, but the volatility itself suggests inconsistent payment timing rather than a controlled cycle.
- Client Credit Risk: Of 70 active clients across 6 industries, BB-rated clients (a lower, non investment grade tier) make up the single largest ratings group at 22 clients, about 31% of the client base. Manufacturing is the largest industry segment (18 clients), giving the business some concentration risk there too.
