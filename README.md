Financial Expense Optimization Analysis – Power BI
---------------------

This project is a complete **Power BI dashboard** built to analyze and optimize organizational expenses across departments, expense categories, and time periods. It includes data cleaning, DAX calculations, interactive visuals, and advanced analytics to support data-driven financial and budgeting decisions.

Project Overview
---------------------

The goal of this project is to understand:

* Department-wise expense distribution
* Monthly spending patterns and trends
* Expense categories contributing to overspending
* Budget utilization and variance
* Factors driving cost overruns

 What’s Included
 ---------------------

* Cleaned & validated Financial Expense dataset
* Single-table optimized data model
* DAX measures for Expenses, Budget, Variance, and Averages
* 6-page interactive Power BI dashboard
* Advanced visuals Decomposition Tree & Q&A
* Final business insights & cost-control recommendations

Data Cleaning
---------------------

Performed in Power Query

* Identified and handled missing or null expense values
* Removed inconsistent records (zero/negative expenses)
* Validated Actual Expense and Budget fields
* Standardized department and expense type names
* Ensured proper Date, Month, Quarter, and Year formats

Data Model
---------------------

Fact Table:
---------------------

* Financial Expense Data (Actual Expense, Budget, Variance)

Attributes:
---------------------

* Department
* Expense Type
* Category (Fixed / Variable)
* Date, Month, Quarter, Year

A simplified model was used to improve performance and ease of analysis

Dashboard Pages (6 Pages)
---------------------

1. Executive Overview
   
* KPIs: Total Expenses, Total Budget, Budget Variance, Monthly Avg Expense
* Monthly expense trend
* Department-wise expense summary

2. Department Analysis

* Expense comparison across HR, IT, Finance, and Operations
* High-spending department identification
* Manager-wise accountability

3. Expense Type Analysis

* Fixed vs Variable expense distribution
* Expense type contribution to total spend
* Overspending category identification

4. Budget vs Actual Analysis

* Actual vs Budget comparison by department
* Budget variance analysis
* Over-budget department detection

5. Decomposition Tree

* Root cause analysis of total expenses
* Drill-down by Department, Expense Type, Category, and Month

6. Q&A Dashboard

* Natural language queries for self-service financial insights

Key DAX Measures
---------------------

DAX
Total Expenses = SUM(Financial_Expense_Optimization[ActualExpense])

Total Budget = SUM(Financial_Expense_Optimization[BudgetAmount])

Budget Variance = [Total Expenses] - [Total Budget]

Monthly Avg Expense =
AVERAGEX(
    VALUES(Financial_Expense_Optimization[Month]),
    [Total Expenses]
)

Key Insights
---------------------

* IT and Operations departments incur the highest expenses
* Salaries and Infrastructure are the primary cost drivers
* Variable expenses show higher fluctuation and risk
* Certain departments consistently exceed budget limits
* Monthly expense trends indicate increasing operational costs


Recommendations
---------------------

* Introduce budget alerts for high-spending departments
* Monitor and control variable expenses like travel and marketing
* Optimize vendor and infrastructure contracts
* Conduct monthly expense reviews
* Allocate budgets based on data-driven insights


Tools Used
---------------------

* Power BI Desktop
* Power Query
* DAX
* CSV Dataset

