# 📊 Flipkart Order Issue Resolution & Customer Support Analytics

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Processing-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Google%20Colab-Development%20Environment-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" />
  <img src="https://img.shields.io/badge/Domain-Data%20Analytics-00897B?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Completed-2E8B57?style=for-the-badge" />
</p>

---

## 📌 Project Overview

**Flipkart Order Issue Resolution & Customer Support Analytics** is a Python-based data analytics project focused on identifying and analyzing e-commerce order issues, including delivery delays, refund problems, and customer complaints.

The project integrates order, refund, and customer complaint records into a consolidated order-level investigation report. It applies predefined business rules to identify problematic orders and classify them into support priority levels.

The objective is to help customer support teams investigate order-related issues more efficiently and identify cases that require attention.

## 🎯 Business Problem

E-commerce support teams often need to examine multiple datasets to understand customer issues. Order details, refund records, and customer complaints are maintained separately, making investigation time-consuming.

This project addresses the problem by:

- Combining information from multiple datasets.
- Identifying delivery, refund, and complaint-related issues.
- Highlighting orders that require further investigation.
- Assigning support priority levels based on identified issues.
- Providing consolidated reports for support operations.

## 🚀 Project Objectives

- Load and inspect order, refund, and customer complaint datasets.
- Clean and validate records by handling duplicates, inconsistent values, and missing data.
- Calculate delivery delays using promised and actual delivery dates.
- Analyze refund amounts, refund counts, and pending or failed refunds.
- Identify repeated and open customer complaints.
- Integrate the cleaned datasets using a common order identifier.
- Identify issue indicators and classify support priorities.
- Generate final analytical reports in CSV and Excel formats.

## 🛠️ Tools & Technologies

| Technology | Application |
|---|---|
| Python | Data processing and analysis |
| Pandas | Data cleaning, transformation, aggregation, and merging |
| NumPy | Numerical operations |
| Google Colab | Notebook development and execution |
| CSV | Order-level report export |
| Excel | Priority summary export |
| JSON | Customer complaint data input |

## ⚙️ Project Workflow

**1. Data Loading & Inspection**
- Loaded orders, refunds, and customer complaint datasets.
- Inspected dataset dimensions, columns, data types, and missing values.

**2. Data Cleaning & Validation**
- Identified and removed duplicate records.
- Standardized inconsistent status values.
- Converted date and numerical columns into appropriate data types.
- Validated records and identified unmatched order IDs.

**3. Delivery Delay Analysis**
- Calculated delivery delay days using actual and promised delivery dates.
- Identified orders delivered more than three days late.

**4. Refund Analysis**
- Aggregated refund records at the order level.
- Calculated refund counts and total refund amounts.
- Identified orders with pending or failed refunds.

**5. Customer Complaint Analysis**
- Aggregated complaint records by order.
- Calculated complaint counts and open complaint counts.
- Identified orders with repeated complaints.

**6. Data Integration**
- Combined cleaned order, refund, and complaint information.
- Created a consolidated order-level investigation dataset.

**7. Issue Identification**
- Created indicators for delayed deliveries, refund issues, and repeated complaints.
- Calculated the total number of issue indicators for each order.

**8. Support Priority Classification**
- Assigned High, Medium, and Low priorities using predefined business rules.

**9. Report Generation**
- Prepared the final order investigation report.
- Generated a summary of support priority levels.

**10. Exporting Results**
- Exported the final analytical outputs into CSV and Excel formats.

## 📊 Support Priority Classification

Orders are classified based on the number of identified issue indicators.

| Priority | Classification Rule |
|---|---|
| 🔴 High | Two or more issue indicators |
| 🟡 Medium | Exactly one issue indicator |
| 🟢 Low | No issue indicators |

This is a rule-based classification approach designed to help support teams identify orders requiring attention. It does not use a machine learning classification model.

## 📈 Key Findings

The analysis identified the following results across 1,600 unique orders:

| Business Metric | Result |
|---|---:|
| Total Unique Orders | 1,600 |
| High-Priority Orders | 234 |
| Orders Delayed by More Than 3 Days | 234 |
| Orders with Pending or Failed Refunds | 540 |
| Orders with Multiple Complaints | 405 |
| Missing Actual Delivery Dates | 487 |

**Business Insight:** Delivery delays, refund issues, and repeated complaints highlight different areas requiring customer support attention. The priority classification helps organize orders for further investigation.

*Note: These issue categories can overlap, so their counts should not be added together.*

## 📁 Repository Structure

```text
Flipkart-Order-Issue-Resolution-Customer-Support-Analytics/
│
├── Flipkart_Order_Issue_Resolution_Analytics.ipynb
│
├── outputs/
│   ├── flipkart_order_issue_report.csv
│   └── flipkart_issue_summary.xlsx
│
└── README.md
```

## 📦 Project Deliverables

The repository includes the following final analytical outputs:

| File | Description |
|---|---|
| `Flipkart_Order_Issue_Resolution_Analytics.ipynb` | Complete project implementation and analysis |
| `flipkart_order_issue_report.csv` | Consolidated order-level investigation report |
| `flipkart_issue_summary.xlsx` | Support priority summary in Excel format |

### View Project Outputs

- 📄 [View Final Order Issue Report (CSV)](outputs/flipkart_order_issue_report.csv)
- 📊 [Download Priority Summary (Excel)](outputs/flipkart_issue_summary.xlsx)
- 📓 [Open Project Notebook](Flipkart_Order_Issue_Resolution_Analytics.ipynb)

*GitHub can preview the CSV report directly. The Excel file can be downloaded and opened in Microsoft Excel.*

## 📂 Dataset Availability

The original input datasets are not included in this repository:

- `orders.csv`
- `refunds.xlsx`
- `customer_complaints.json`

Only the final analytical output files are provided in the `outputs` folder.

The datasets used in this project contain fictional training records and do not represent actual Flipkart customer transactions.

To reproduce the analysis, the required input datasets must be obtained separately and uploaded to the Google Colab environment.

## ▶️ How to Run the Project

1. Open the project notebook using Google Colab.
2. Obtain the three required input datasets.
3. Upload the datasets to the Colab environment using their original filenames.
4. Execute the notebook cells in the given sequence.
5. Review the data cleaning, validation, analysis, and priority classification results.
6. Generate the final CSV and Excel reports.

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Data cleaning and preprocessing using Python and Pandas.
- Data validation and handling missing values.
- Data aggregation using grouping operations.
- Integrating multiple datasets using common keys.
- Applying business rules to identify order-related issues.
- Creating rule-based support priority classifications.
- Generating structured analytical reports using CSV and Excel.

---

<p align="center">
  <b>Thank you for visiting my project!</b>
  <br/>
  <i>Building practical data analytics solutions to support better business decisions.</i>
</p>
