# Online Learning Enrollment Analytics Platform

## Project Overview
An end-to-end Data Engineering project built using Databricks to process online learning enrollment data through Bronze, Silver, and Gold layers and create an analytics dashboard.

## Technologies Used
- Databricks
- Python / PySpark
- SQL
- Lakeflow Spark Declarative Pipelines
- Databricks AI/BI Dashboards

## Project Architecture

### Bronze Layer
- Ingested raw enrollment CSV data using Auto Loader.
- Captured ingestion metadata.

### Silver Layer
- Cleaned and standardized data.
- Handled missing and invalid values.
- Removed duplicate enrollment IDs.
- Separated rejected records.
- Derived learner status.

### Gold Layer
Created seven analytical summary tables:
- Monthly enrollments
- Category summary
- Course summary
- Channel summary
- Learner status summary
- Overview summary
- Data quality summary

## Data Quality Results

| Metric | Result |
|---|---:|
| Bronze rows | 1,283 |
| Clean Silver rows | 1,241 |
| Rejected rows | 19 |
| Duplicate extra rows | 23 |
| Unique learners | 553 |

**Reconciliation check:**

1,283 = 1,241 + 19 + 23

**Status: Passed**

## Dashboard Pages
1. Overview – Enrollment KPIs, revenue trends and learner status.
2. Courses & Channels – Course performance, completion rates and channel analysis.
3. Data Quality – Data validation, email cleaning and reconciliation.

## Learning Outcomes
- Built an end-to-end data pipeline.
- Practiced data cleaning and transformation.
- Implemented data quality checks.
- Created analytical tables.
- Developed an interactive dashboard.

## Project Status
Completed – November 2026.
