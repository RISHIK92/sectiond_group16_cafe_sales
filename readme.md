Cafe Sales Performance & Customer Behaviour Analysis

Capstone Project | Food & Beverage / Retail Analytics
Newton School of Technology | Faculty Mentor: Archit Raj


Project Overview
This project analyzes café sales transaction data to uncover revenue drivers, customer behaviour patterns, and operational improvement opportunities. The analysis was conducted using Google Sheets (pivot tables, formulas, and interactive filters) as the primary tool.

Team — Group 16
Ananya Narang
2401020087
PPT & Quality Lead
Divy Kumar Jain
2401010157
Project Lead
Hrishabh Prajapati
2401020027
Analysis Lead
Preet Vardhan
2401010352
Strategy Lead
Rishik
2401010381
Dashboard Lead
Shubham Jain
2401010452
Data Lead

Problem Statement
The café lacked clarity on:

Seasonal demand patterns
Top revenue-generating items
Customer purchase behaviour
Payment & channel preferences
Order delivery type

This limited the ability to make data-driven decisions for pricing, marketing, and operations.

Dataset

Source: Cafe Sales – Dirty Data for Cleaning Training (Kaggle)
Total Transactions: 7,773
Product Categories: 8
Time Span: 12 months

Key Columns
ColumnDescriptionTransaction IDUnique identifier per transactionMonthMonth of transactionItemProduct purchasedQuantityUnits soldPrice Per UnitUnit price of itemTotal SpentRevenue per transactionLocationIn-store / Takeaway / UnknownPayment MethodCash / Credit Card / Digital Wallet / Unknown
Data Limitations

Location unknown: 39.78% of records
Payment method unknown: 31.12% of records


Data Cleaning & Preparation

Replaced blank Location and Payment Method fields with "Unknown"
Created Month Number field for correct time-series sorting
Standardized Location into three categories: In-store, Takeaway, Unknown
Checked for extreme/negative transaction values — no major anomalies found
Assumption: Unknown values are valid but missing entries; prices remain constant across months


KPI Framework
KPIFormulaPurposeTotal RevenueSUM(Total Spent)Overall business performanceTotal TransactionsCOUNT(Transaction ID)Demand volumeAvg Order ValueAVG(Total Spent) ≈ $8.94Spending behaviourTotal QuantitySUM(Quantity)Menu optimizationAvg Items Per TransactionAvg(Quantity / Transactions)Real demand indicator

Key Insights

Overall revenue is stable throughout the year — consistent customer demand with no sharp seasonal spikes.
October and June record marginally higher sales, suggesting mild seasonal peaks.
Salad is the highest revenue-contributing item — key product for profitability.
Coffee and Juice drive transaction volume but generate lower revenue per unit.
In-store purchases show slightly higher average spend ($8.94) vs. Takeaway ($8.88).
Revenue is evenly distributed across Cash, Credit Card, and Digital Wallet payment methods.
~40% of location data and ~31% of payment data is untracked — a critical operational gap.
Monthly demand ranges from 1,852 units (February) to 2,072 units (October) — highly stable.


Recommendations
InsightRecommendationExpected ImpactSalad leads revenuePromote premium & healthy combo offerings+8–12% revenue upliftIn-store higher spendImprove seating, ambience, dine-in experience+3–5% increase in AOVMissing data highFix POS data tracking, enforce mandatory fields+25–30% decision accuracyPeak months knownRun seasonal promotional campaigns in June & October+4–6% sales increase

Advanced Analysis

Demand Stability: Monthly units sold range of only ~220 units across the year — demand is consistent with no sharp peaks.
Channel Spending: In-store AOV ($8.94) marginally exceeds Takeaway ($8.88); in-store offers greater upselling opportunity.


Dashboard
Built in Google Sheets using pivot tables, summary charts, and interactive filters.
Filters Available: Month | Item | Location | Payment Method
Dashboard Views:

KPI summary (Revenue, Transactions, Quantity, AOV)
Monthly revenue trend
Product-level revenue and volume comparison
Location and payment method distribution


Limitations

High 'Unknown' values in Location and Payment Method restrict channel-level analysis
No cost or margin data — profitability analysis not possible
No customer identifiers — repeat purchase and segmentation analysis not possible
External factors (promotions, holidays, price changes) not accounted for
Findings depend on accuracy of POS data entry


Future Scope

Incorporate cost/margin data for profitability analysis
Capture customer IDs for segmentation and repeat behaviour analysis
Improve POS validation to eliminate missing data
Integrate promotions and pricing data to measure campaign effectiveness
Apply forecasting models for inventory and staffing planning
Migrate to advanced BI tools (Power BI / Tableau) for scalability


Conclusion
This project demonstrates how simple spreadsheet analytics using Google Sheets can reveal meaningful business insights from transactional data, support data-driven decision-making across products, channels, and payments, and identify opportunities to improve revenue and operational efficiency.

Submitted as part of the DVA Capstone 1 Project | Newton School of Technology

