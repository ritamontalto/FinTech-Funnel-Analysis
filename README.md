# FinTech Loan Application Funnel Analysis

End-to-End Business Intelligence project analyzing customer behavior, funnel conversion and portfolio risk within a digital lending platform.

## Executive Summary
Lending institutions must balance customer acquisition, conversion and portfolio quality while maintaining sustainable growth. This project presents an end-to-end business intelligence case study for a hypothetical FinTech lender, analyzing the complete loan application journey to identify conversion bottlenecks, understand customer behavior and evaluate portfolio performance. To simulate a realistic business environment, 4 synthetic datasets were created representing customers, loan applications, application events and loan outcomes. The analysis combines SQL-based data preparation and business analysis with Power BI interactive reporting to deliver actionable business insights and support data driven decision-making.


## Business Problem
A FinTech lender wants to improve the performance of its digital loan application process while maintaining a healthy loan portfolio. The Product Management team observed that many applicants abandon the application journey before funding, but the reasons behind this behavior are unclear. At the same time, the Risk team wants to ensure that increasing loan approvals doesn't negatively impact portfolio quality through higher charge-off rates. This project investigates the complete loan application journey to identify opportunities for improving customer conversion while balancing credit risk and business performance. The analysis aims to answer the following questions:

- Which customer segments achieve the highest approval rates?
- Where do applicants drop out of the loan application funnel?
- Which refusal reasons contribute most to lost applications?
- Which acquisition channels generate the best balance between conversion and portfolio quality?
- How does portfolio performance vary across customer segments?
- Which business opportunities could improve both conversion and portfolio quality?


## Datasets
As no publicly available dataset fully represented the required business scenario, I created 4 synthetic datasets to simulate operations of a digital lending platform. The data was generated with AI assistance and intentionally includes missing values, inconsistent formatting and data quality issues to support a realistic end-to-end analytics workflow. While AI was used exclusively to generate the fictional data, all data cleaning, validation, SQL development, business analysis, DAX measures, dashboard design, visualizations, insights and recommendations were independently designed, reviewed and implemented by me.


## Data Model
The analysis follows a relational data model centered around the loan application lifecycle:

```
Users
  │
  │ 1 : Many
  ▼
Loan Applications
  │
  │ 1 : Many
  ├──────────────► Application Events (multiple status updates)
  │                   
  │ 1 : 1
  ▼
Loan Outcomes
```

- Users table contains customer demographic information
- Loan Applications table stores application details and estimated credit risk
- Application Events table records each stage reached during the application journey
- Loan Outcomes table contains funded loan information and portfolio performance metrics

## Methodology
This project follows an end-to-end business intelligence workflow, from raw data preparation to business recommendations:

```
Raw Data
   ↓
Data Cleaning & Validation
   ↓
Exploratory Business Analysis
   ↓
Funnel Analysis
   ↓
Interactive Power BI Dashboard
   ↓
Business Insights & Recommendations
```

Each stage of the workflow is summarized below.

**Data Cleaning & Validation** 

Raw datasets were cleaned, standardized and validated before analysis to ensure consistency and reliability. Validation checks included:

- Verify that every application belongs to an existing customer
- Ensure that loan outcomes matched the final application status
- Confirm that refusal reasons exist only for rejected applications
- Verify that interest rates are recorded only for granted loans
- Check consistency between loan status, charge-off flags and charge-off dates
- Remove duplicate records and handle missing values

**Exploratory Business Analysis**
- Analyzed customer demographics and borrowing behavior
- Investigated application outcomes across customer segments
- Evaluated acquisition channel performance, credit risk and portfolio quality

**Funnel Analysis**
- Mapped the complete application journey from submission to funding
- Measured conversion rates at each stage
- Identified the largest drop-off points and compared funnel performance across customer segments

**Interactive Dashboard Development**
- Built an interactive Power BI dashboard to monitor operational performance and portfolio health
- Designed three reporting pages covering executive KPIs, funnel performance and risk analysis

**Business Insights & Recommendations**
- Summarized the analytical findings into actionable business recommendations
- Highlighted opportunities to improve conversion while maintaining portfolio quality


## Key Findings

#### Where are applicants dropping out of the loan application funnel?
The largest reduction in applicant volume occurs before the document submission stage, making it the primary conversion bottleneck in the customer journey.

#### Which customer segments are most likely to be approved?
Applicants with stronger estimated credit scores achieve substantially higher approval rates, while approval patterns also vary across income groups and acquisition channels.

#### Which acquisition channels perform best?
Acquisition channels differ considerably in both application volume and approval rate. Comparing conversion alongside portfolio quality highlights the channels that generate the highest business value.

#### Which customer segments present the greatest portfolio risk?
Charge-off rates vary across customer segments and acquisition channels, demonstrating that high loan volumes don't always translate into better portfolio performance.

#### How is credit risk reflected in pricing?
Applicants with lower estimated credit scores receive higher average interest rates, indicating that lending decisions follow a risk-based pricing strategy.

#### What opportunities exist to improve lending performance?
Funnel inefficiencies represent a potential opportunity to increase funded loan volume and lending revenue by improving conversion at key stages of the customer journey.

#### How can the business improve performance?
Improving applicant conversion at the largest funnel bottleneck represents the greatest opportunity to increase funded loans while maintaining portfolio quality.


## Business Recommendations
- **Reduce applicant drop-off before document submission** by simplifying the document upload experience and identifying friction points in the application journey
- **Prioritize acquisition channels** that consistently combine high approval rates with low charge-off rates to maximize portfolio performance
- **Monitor portfolio quality continuously** across customer segments and credit score bands to detect changes in lending risk early
- **Refine underwriting strategies** for borderline applicants by balancing approval rates with expected portfolio performance rather than relying solely on application volume
- **Track funnel conversion and portfolio KPIs** through interactive dashboards to support data driven decision-making and continuous process improvement


## Skills Demonstrated

**Business Analysis**
- Exploratory Business Analysis 
- Funnel analysis
- Customer segmentation
- Credit risk analysis
- KPI definition and performance monitoring
- Business insight generation

**SQL (PostgreSQL)**
- Data cleaning
- Data validation
- Data quality checks
- CTEs
- Window functions
- Joins
- Aggregations
- CASE statements
- Business oriented analytical queries

**Power BI**
- Data modeling
- DAX measures
- Interactive dashboards
- KPI cards and visualizations
- Slicers and cross-filtering

**AI Assisted Development**
- Synthetic dataset generation (Claude)
- Brainstorming and workflow support


## Project Files
- Data: Original synthetic datasets and cleaned tables ready for analysis

- SQL notebooks: Data cleaning and analysis notebooks, including code and notes

- Power BI: Interactive dashboards analyzing funnel, performance and risk

- Screenshots: Preview of the interactive Power BI dashboards
