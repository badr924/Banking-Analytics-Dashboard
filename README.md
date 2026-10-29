# 🏦 Banking Customer & Operations Analytics Dashboard

An interactive **Power BI** dashboard that turns raw banking data into clear, actionable insights across customers, accounts, transactions, loans, cards, and support operations.

## 📌 Project Overview

The goal of this project is to help a bank monitor its performance and spot opportunities for improvement. The report is built on a star-schema data model and is split into five pages with page navigation buttons and slicers for **Year**, **Loan Status**, and **Account Type**.

## 📊 Dashboard Pages

| Page | What it shows |
|------|---------------|
| **Overview** | A high-level snapshot of customers, transactions, balances, and loans, with monthly transaction trends, loan status split, balance by account type, support issue resolution, and loan amount by state |
| **Customers** | Account holders, active vs. dormant accounts, accounts per customer, transaction frequency distribution, and customer growth by year |
| **Transactions** | Average transaction amount by account type, transaction value by quarter, balance vs. number of transactions, and transaction type breakdown |
| **Loans** | Loan portfolio by type and status, interest rate metrics, card types, and quarterly loan trends |
| **Support Calls** | Issue volume, solved vs. unsolved rate, issue types, daily trend, and geographic distribution by state |

## 🖼️ Screenshots

![Overview](screenshots/overview.png)
![Customers](screenshots/customers.png)
![Transactions](screenshots/transactions.png)
![Loans](screenshots/loans.png)
![Support Calls](screenshots/support_calls.png)

## 🗄️ Data Model

The model follows a star schema with **customers** as the central dimension:

- **customers**: customer details and join date
- **Accounts**: account type, balance, and creation date
- **Banking_Analytics_Transactions**: transaction amount, type, date, and season
- **Loans**: loan amount, type, interest rate, start/end date, and status
- **Cards**: card type, issue and expiration dates
- **SupportCalls**: issue type, call date, and resolution status
- **Calendar**: date dimension for time intelligence (Year, Quarter, Month, Day)

## 💡 Key Insights

- A large share of accounts are dormant, which points to a strong opportunity for re-engagement campaigns.
- Most of the loan portfolio is still active.
- Only about half of support issues are resolved, so support operations need attention.
- Transaction volume shows a steady upward trend through the year.

## 🛠️ Tools & Skills

- **Power BI Desktop**
- **DAX** (measures, KPIs, time intelligence)
- **Data modeling** (star schema, relationships)
- **Data visualization** (KPI cards, combo charts, donut/pie charts, maps, slicers, navigation buttons)
