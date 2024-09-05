# Financial Performance and Budget Analysis Using Power BI

## Introduction

This report presents a detailed analysis of a company's financial performance and budget comparisons using Power BI. The analysis focuses on profit and loss, balance sheet, ledgers, and horizontal analysis across multiple years. Additionally, a secondary analysis is conducted to compare actual performance with budgeted values. The data spans multiple financial years and territories, providing a comprehensive view of the company's financial health and growth trends.

## Objectives

The primary objectives of the analysis are to:

- **Profit and Loss (P&L)**: Analyze the company's revenue, expenses, and profits across different accounts, sub-accounts, and regions. Compute key profitability metrics like EBITDA, gross profit margin, and net profit margin.
- **Balance Sheet (BS)**: Assess the company's assets, liabilities, and owner's equity. Evaluate key financial ratios such as current ratio, quick ratio, return on capital employed (ROCE), return on equity (ROE), and gearing ratio.
- **Ledgers**: Track financial performance over time with filters for country, date, and account.
- **Horizontal Analysis**: Analyze the percentage gain or loss in profit and balance sheet accounts over the years.
- **Budget vs Actual**: Compare the actual financial performance to the budgeted figures for sales and P&L on a quarterly basis.

## Data Description
The analysis is based on two primary datasets: **Business Data** and **Budget Data**. Each dataset is organized across multiple sheets providing details on general ledger entries, calendar information, chart of accounts, and territory mapping. These datasets are critical to understanding the financial performance and comparison between actual and budgeted data.

### Dataset 1: Business Data

1. **GL (General Ledger)**:
   - Contains detailed financial records related to various accounts and transactions.
   - **Columns**:
     - `Account_key`: Unique identifier for each account.
     - `Details`: Description of the transaction (e.g., sales, expenses).
     - `Amount`: Monetary value associated with the transaction.

2. **Calendar**:
   - Contains date-related information to link transactions with specific time periods.
   - **Columns**:
     - `Date`: Exact date of the transaction.
     - `Year`: Year in which the transaction took place.
     - `Quarter`: Fiscal quarter.
     - `Month`: Month of the transaction.
     - `Day`: Specific day of the transaction.

3. **Chart of Accounts**:
   - Provides a structured breakdown of all accounts used in the analysis.
   - **Columns**:
     - `Account_key`: Unique identifier for each account, used to map transactions.
     - `Report`: High-level report category.
     - `Class`: General classification (e.g., assets, liabilities, revenue).
     - `SubClass`: More detailed classification within the account.
     - `SubClass2`: Additional classification for further granularity.
     - `Account`: Account name.
     - `SubAccount`: Detailed sub-account name.

4. **Territory**:
   - Contains geographical information for transactions.
   - **Columns**:
     - `Territory_key`: Unique identifier for each geographical region.
     - `Country`: Name of the country associated with the transaction.
     - `Region`: Broader geographical region (e.g., Europe, North America).

### Dataset 2: Budget Data

1. **Budget Entries**:
   - Contains budgeted values structured similarly to the general ledger data for comparison with actual performance.
   - **Columns**:
     - `EntryNo`: Unique identifier for each budget entry.
     - `Date`: Date of the budget entry.
     - `Territory_key`: Links to the territory to identify the region for which the budget was set.
     - `Account_key`: Links to the chart of accounts for the specific budgeted account.
     - `Details`: Description of the budgeted entry.
     - `Amount`: Monetary value of the budgeted entry.
     - `Type`: Indicates whether the entry is related to actuals or budgets.

## Analysis and Commentary

### 1. Profit and Loss (P&L)

- **Sales Revenue Analysis**:
  - A table with yearly sales revenue for different accounts and sub-accounts.
  - Key metrics include sales revenue TTD, FTP, gross profit, EBITDA, operating profit, PBIT, and net profit for each year.
  
- **Profit Margins**:
  - Calculated gross profit margin and net profit margin for each year.
  - A plot displaying the sales revenue, gross profit margin, net profit margin, sales FTP, gross profit, and net profit for each year.

- **Geographical Analysis**:
  - Sales revenue, gross profit, and net profit plotted per country to analyze geographical performance.

- **Marketing and Sales Costs**:
  - A plot showing marketing cost FTP and sales FTP for each year.

### 2. Balance Sheet (BS) Analysis

- **Yearly Breakdown**:
  - A table displaying current assets, non-current assets, liabilities (current and long-term), and owner's equity (retained earnings, share capital) for each year.

- **Balance Sheet Plots**:
  - Various visualizations showing the breakdown of the balance sheet by account.

- **Financial Ratios**:
  - Key ratios calculated for each year:
    - Current ratio
    - Quick ratio
    - Return on capital employed (ROCE)
    - Return on equity (ROE)
    - Asset turnover
    - Gearing ratio
    - Receivable days
    - Payable days
    - Inventory turnover
    - Interest cover

### 3. Ledgers

- **Ledger Table**:
  - A table with dates, subaccounts, details, and total FTP, which can be filtered by country, date, class, and account.
  
- **Plots**:
  - A plot showing total FTP per date.
  - A plot showing total TTD per date.

### 4. Profit & Loss (P&L) Horizontal Analysis

- **Yearly Comparison**:
  - A table presenting the percentage gain or loss for each sub-account (trading, operating, non-operating, interest & tax) over the years (2018, 2019, and 2020), compared to previous years.

### 5. Balance Sheet (BS) Horizontal Analysis

- **Balance Sheet Comparison**:
  - A table showing the percentage gain or loss for each balance sheet item (current assets, non-current assets, liabilities, and owner's equity) over multiple years.

### 6. Sales Budget vs Actual

- **Comparison Table**:
  - A table comparing total FTP budget, total FTP actual, and the variance for each quarter of each year.

- **Plot**:
  - A plot visualizing the comparison between the budget and actual values over time.

### 7. P&L Budget vs Actual

- **P&L Comparison Table**:
  - A table showing the comparison between the total FTP budget, total FTP actual, and the variance for the P&L accounts.

---

## Conclusion

This Power BI analysis provides valuable insights into the company's financial performance across multiple years and territories. The combination of profit and loss analysis, balance sheet evaluation, and budget comparisons highlights key trends and potential areas for improvement. Through horizontal analysis and detailed ledger tracking, the report offers a thorough understanding of the company's financial health and operational efficiency.
