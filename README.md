# Flipkart Order Issue Resolution & Customer Support Analytics

## Project Overview

This project focuses on analyzing e-commerce order issues, including delayed deliveries, refund problems, and customer complaints.

The objective is to combine order, refund, and customer complaint datasets into a single order-level investigation report to help customer support teams identify issues and prioritize orders that require attention.

The project was developed using Python, Pandas, and Google Colab.

## Business Problem

Order details, refund records, and customer complaints are maintained in separate datasets. This makes it difficult for customer support teams to investigate customer issues efficiently.

This project integrates these datasets, identifies potential order-related problems, and assigns support priorities using predefined business rules.

## Project Objectives

- Clean and validate order, refund, and customer complaint datasets.
- Identify duplicate records, missing values, and inconsistent data.
- Analyze delivery delays and refund issues.
- Identify repeated customer complaints.
- Combine multiple datasets into a consolidated order-level report.
- Classify orders into High, Medium, and Low support priorities.
- Generate CSV and Excel reports for further analysis.

## Tools & Technologies

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy
- **Environment:** Google Colab
- **Data Formats:** CSV, Excel, JSON
- **Techniques:** Data Cleaning, Data Validation, Data Aggregation, Data Integration, Rule-Based Classification

## Project Workflow

1. **Data Loading and Inspection** – Loaded and inspected orders, refunds, and customer complaint datasets.
2. **Data Cleaning and Validation** – Removed duplicates, standardized status values, converted data types, and checked missing values.
3. **Delivery Delay Analysis** – Calculated delivery delays using actual and promised delivery dates.
4. **Refund Analysis** – Aggregated refund counts, refund amounts, and pending or failed refunds.
5. **Complaint Analysis** – Analyzed complaint counts and open complaints for each order.
6. **Data Integration** – Combined the cleaned datasets using the common `order_id`.
7. **Issue Identification** – Created indicators for delivery delays, refund issues, and repeated complaints.
8. **Priority Classification** – Assigned High, Medium, and Low priorities based on the number of issue indicators.
9. **Report Generation** – Created a final order investigation report and priority summary.
10. **Exporting Results** – Exported the final outputs into CSV and Excel formats.

## Priority Classification

| Priority | Business Rule |
|---|---|
| High | Two or more issue indicators |
| Medium | Exactly one issue indicator |
| Low | No issue indicators |

The classification is rule-based and is intended to support customer support investigations.

## Key Findings

- **1,600** unique orders analyzed.
- **234** high-priority orders identified.
- **234** orders delivered more than three days late.
- **540** orders had pending or failed refunds.
- **405** orders had multiple complaints.
- **487** orders had missing actual delivery dates.

*Note: Issue categories can overlap, so their counts should not be added together.*

## Final Deliverables

- Consolidated order-level investigation report.
- Support priority summary.
- CSV report: `flipkart_order_issue_report.csv`
- Excel summary: `flipkart_issue_summary.xlsx`

## Repository Contents

- `Flipkart_Order_Issue_Resolution_Analytics.ipynb` – Complete project notebook.
- `README.md` – Project documentation.

The original input datasets are not included in this repository.

## How to Run the Project

1. Open the project notebook in Google Colab.
2. Upload the required input datasets:
   - `orders.csv`
   - `refunds.xlsx`
   - `customer_complaints.json`
3. Execute the notebook cells in sequence.
4. Review the cleaned datasets, analysis results, and priority classification.
5. Generate the final CSV and Excel reports.

## Learning Outcomes

Through this project, I gained practical experience in:

- Data cleaning and preprocessing using Pandas.
- Data validation and handling missing values.
- Grouping and aggregating datasets.
- Merging multiple datasets using common keys.
- Applying business rules to identify and classify issues.
- Generating analytical reports using Python.
