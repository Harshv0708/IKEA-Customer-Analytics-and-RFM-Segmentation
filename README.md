# IKEA - Customer Analytics & RFM Segmentation | SQL, Python & Power BI

An end-to-end data analytics project focused on customer segmentation, purchasing behaviour, revenue analysis, and churn identification for an e-commerce business.

## Project Overview

Customer retention is important for e-commerce businesses, but identifying valuable customers and customers at risk of leaving can be challenging without structured analysis.

This project analyses historical retail transactions to understand customer purchasing patterns, segment customers based on their value, and identify potential churn risks. The workflow combines SQL for data cleaning and exploration, Python for customer analytics, and Power BI for interactive visualisation.

The goal is to turn raw transactional data into actionable insights that can support customer retention strategies and data-driven business decisions.

## Business Objectives

- Identify high-value customers and understand their contribution to revenue.
- Segment customers based on purchasing behaviour and monetary value.
- Identify inactive customers who may be at risk of churning.
- Analyse revenue and customer trends over time.
- Compare customer behaviour across geographic markets.
- Recommend targeted retention strategies for different customer segments.

## Tech Stack

| Technology | Purpose |
|---|---|
| SQL Server | Data cleaning, transformation, deduplication, and exploratory analysis |
| Python | Customer analytics, RFM scoring, segmentation, and churn identification |
| Pandas | Data manipulation and aggregation |
| Jupyter Notebook | Python analysis and experimentation |
| Power BI | Interactive dashboards and business reporting |
| DAX | Calculated measures and KPIs |

## Dataset

**Dataset:** Online Retail II  
**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

The dataset contains transactional records from a UK-based online retailer selling gifts and home-related products.

- **Time period:** December 2009 – December 2011
- **Raw records:** Approximately 1.07 million transactions
- **Key attributes:** Invoice number, product code, product description, quantity, invoice date, unit price, customer ID, and country.

The dataset provides a foundation for analysing customer purchasing patterns, revenue contribution, and retention.

## Project Workflow

### 1. Data Cleaning and Exploration — SQL

Prepared the raw transactional data for analysis by addressing data quality issues.

Key tasks:
- Imported and combined transactional records.
- Standardised inconsistent date formats and data types.
- Identified and removed duplicate records.
- Handled invalid transaction values and missing customer identifiers where appropriate.
- Validated record counts and explored transaction patterns.

### 2. Customer Analytics — Python

Used Pandas to calculate customer-level metrics and identify distinct purchasing patterns.

**RFM Analysis**

RFM stands for:

- **Recency:** How recently a customer made a purchase.
- **Frequency:** How often a customer purchased.
- **Monetary:** How much a customer spent.

Customers were scored across these three dimensions on a scale of 1–5 and assigned to behavioural segments.

The segmentation framework includes:

- Champions
- Loyal Customers
- At Risk
- New Customers
- Needs Attention
- Lost Customers

A 90-day inactivity threshold was also used to flag customers classified as churned under the project's definition.

### 3. Interactive Dashboard — Power BI

Developed a three-page dashboard to present business performance and customer insights.

**Page 1: Home**
- Project introduction and report navigation.
- Definitions of key analytical metrics.

**Page 2: Business Overview**
- Total customers and revenue.
- Customer churn percentage.
- Average customer value.
- Revenue and customer trends over time.
- Customer segment and geographic comparisons.
- Interactive filters for date, country, segment, and churn status.

**Page 3: RFM Analysis**
- Customer distribution across segments.
- Revenue contribution by segment.
- Average RFM scores.
- Average customer value by segment.
- Churn trends over time.

## Key Findings

The existing project analysis reports the following findings:

| Finding | Business Significance |
|---|---|
| Champions represent approximately 22% of customers and generate close to 68% of revenue. | High-value customers are important to overall revenue performance. |
| The reported churn rate is 50.86%, using a 90-day inactivity threshold. | Customer retention deserves focused attention. |
| Customer value varies considerably across segments. | Marketing and retention efforts can be tailored to customer value. |
| Revenue shows seasonal increases during Q4. | Seasonal campaigns and inventory planning may benefit from historical trends. |

> **Validation note:** These figures are based on the existing project's analysis. Validate them against your own results before presenting them as findings from your implementation.

## Business Recommendations

Based on the analytical framework, the business could consider the following actions:

- **Champions:** Encourage repeat purchases through loyalty benefits and personalised offers.
- **Loyal Customers:** Strengthen retention with relevant product recommendations and rewards.
- **At-Risk Customers:** Test targeted re-engagement campaigns to encourage another purchase.
- **New Customers:** Improve the first-time customer experience and encourage repeat orders.
- **Needs Attention:** Investigate changes in purchasing frequency and spending.
- **Lost Customers:** Evaluate whether win-back campaigns are commercially worthwhile.

These are potential actions suggested by the segmentation framework, rather than measured outcomes of campaigns.

## Skills Demonstrated

- SQL querying and data transformation
- Data cleaning and quality validation
- Exploratory data analysis
- Customer segmentation using RFM analysis
- Customer churn identification
- Python and Pandas
- KPI development and DAX
- Interactive dashboard development
- Business insight generation and data storytelling

## Repository Contents

The repository currently includes the following supporting materials:

- `IKEA Gifting BRD.docx` — Business requirements document
- `IKEA Gifting Dataset.zip` — Transactional dataset
- `IKEA Prerequisites Install Guide.pdf` — Setup guide
- `IKEA Project Theme.json` — Power BI theme
- `Ikea Dashboard as PDF.pdf` — Dashboard report
- `Images.zip` — Project images
- `rfm_segmentation.ipynb` — Python notebook for RFM analysis, customer segmentation, and churn identification

For a reproducible portfolio project, the repository should also include the SQL scripts, Python notebook, and Power BI report used to produce the results.

## How to Reproduce the Analysis

Once the implementation files are included:

1. Download the Online Retail II dataset from the UCI Machine Learning Repository.
2. Import the data into SQL Server.
3. Execute the SQL scripts to clean, transform, and validate the data.
4. Export the cleaned data for analysis in Python.
5. Run the Python notebook to calculate RFM scores, assign customer segments, and generate churn flags.
6. Load the resulting data into Power BI.
7. Configure the data source, refresh the report, and explore the dashboard using its filters.

## Project Outcome

This project demonstrates how transactional data can be transformed into customer-level insights using SQL, Python, and Power BI. It connects data preparation and analytical modelling with interactive reporting to support customer segmentation, retention analysis, and business decision-making.

---

**Disclaimer:** IKEA Gifting is a fictional business used for this analytical project. This project is not affiliated with or endorsed by IKEA. The findings relate to the underlying retail dataset and should not be interpreted as actual IKEA business performance.
