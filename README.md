# FinTech Loan Application Funnel Analysis

End-to-End Business Intelligence project exploring customer behavior throughout a loan application funnel to identify conversion bottlenecks and evaluate portfolio risk.

## Executive Summary
Lending institutions must balance customer acquisition, conversion and portfolio quality while maintaining sustainable growth. This project presents an end-to-end business intelligence case study for a hypothetical FinTech lender, analyzing the complete loan application journey to identify conversion bottlenecks, understand customer behavior and evaluate portfolio performance. To simulate a realistic business environment, I generated four synthetic datasets representing customers, loan applications, application events and loan outcomes. The analysis combines SQL for data cleaning, preparation, validation and analysis, with Power BI for interactive business dashboards to deliver actionable business insights and support data driven decision-making.

------

## Business Objectives
I assumed that the product management team would like to:

- Explore customer demographics and borrowing behavior
- Analyze application outcomes across customer segments
- Identify conversion bottlenecks throughout the application funnel
- Evaluate portfolio quality using charge-off metrics
- Build an interactive Power BI dashboard for business monitoring


## Skills & Tools
Analytics: Funnel Analysis, Exploratory Analysis, KPI development, business insight generation

SQL: PostgreSQL, CTEs, Window functions, Joins, Case statements, Aggregations, data cleaning

Power BI: data modeling, DAX measures, interactive dashboards, data visualization

Claude: generation of synthetic datasets, brainstorming support


## Methodology
1. Data cleaning and preparation: SQL queries that extract, clean and transform data from the database.
2. Exploratory Business Analysis: SQL queries that select specific data to answer business questions.
3. Funnel Analysis:
4. Dashboard development: Power BI dashboards that display performance and risk, funnel analysis and overview insights through cards, charts and interactive filtering.


## Data Workflow
Raw Data
 
↓

Data Cleaning

↓

Data Validation

↓

Exploratory Business Analysis
 
↓

Funnel Analysis

↓

Power BI Dashboard

↓

Business Insights & Recommendations


## Data Validation Checks
- Verified every application belongs to an existing customer.
- Ensured loan outcomes matched the final application status.
- Confirmed refusal reasons exist only for rejected applications.
- Verified interest rates are recorded only for granted loans.
- Checked consistency between loan status, charge-off flags and charge-off dates.
- Removed duplicate records and handled missing values.


## Data Model
Users

↓

Loan Applications

↓

Application Events

↓

Loan Outcomes


## Datasets
The datasets used in this project are synthetically generated and do not contain real information. They were created with the assistance of Anthropic's Claude specifically for portfolio purposes to mimic realistic financial and users data, including intentional inconsistencies, missing values, duplicate records and formatting issues to support a complete data cleaning and funnel analysis workflow. 
I used AI to generate fictional data for analysis. All SQL queries, data cleaning decisions, business logics, dashboard design, DAX measures, analysis and final interpretations were independently designed, reviewed, adapted and implemented by myself.

- Users table: Customer demographic information
- Loan Applications table:	Loan requests and application outcomes
- Application Events table: Status changes throughout the application process
- Loan Outcomes	table: Funded loan details and repayment performance


## Key Business Insights & Results 
- The largest reduction in applicant volume occurs before document submission.
- Acquisition channels differ considerably in both approval rate and portfolio quality.
- Higher estimated credit scores are associated with stronger approval rates and lower interest rates.
- Charge-off rates vary across customer segments, highlighting differences in portfolio risk.
- Improving conversion at the largest funnel bottleneck could materially increase funded lending.


## Business Recommendations
- Simplify the document submission process to reduce applicant attrition.
- Increase investment in acquisition channels that combine high approval rates with low charge-off rates.
- Continue monitoring portfolio quality across credit score bands.
- Review underwriting criteria for borderline applicants to balance growth and credit risk.


## Project Files
- Data: Original synthetic datasets and cleaned tables ready for analysis

- SQL notebooks: Data cleaning and analysis notebooks, including code and notes

- Power BI: Interactive dashboards analyzing funnel, performance and risk

- Screenshots: Preview of the interactive Power BI dashboards
