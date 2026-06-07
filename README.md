# FP&A Reporting & Forecasting Tool

## Overview

This project demonstrates how Python can be applied to automate common FP&A (Financial Planning & Analysis) activities including data validation, variance analysis, management reporting, and driver-based forecasting.

The objective is to automate a typical FP&A reporting workflow by transforming Actual and Budget financial data into management-ready reporting outputs and driver-based forecasts.

---

## Business Problem

Finance teams often spend significant time manually:

- Validating financial data
- Investigating budget variances
- Preparing management reports
- Building forecast files
- Identifying key performance issues

Manual processes increase the risk of errors, reduce consistency across reporting cycles, and limit the time available for analysis and decision support.

This project demonstrates how Python can automate key FP&A reporting activities while improving transparency and repeatability.

---

## Key Features

### Data Quality Validation

- Missing value detection
- Non-numeric financial value checks
- Invalid date identification
- Automated data quality issue reporting

### Variance Analysis

- Actual vs Budget comparison
- Variance calculations
- Variance percentage calculations
- Favorable / Unfavorable classification

### Management Reporting

- Executive Summary generation
- Account-level variance reporting
- Business Unit variance reporting
- Monthly performance analysis

### Issue Identification

- Severity scoring based on variance thresholds
- High and medium-risk issue identification
- Largest favorable variance reporting
- Largest unfavorable variance reporting

### Driver-Based Forecasting

The forecasting approach uses a simplified FP&A driver-based model built around key business drivers and configurable assumptions.

---

## Technologies Used

- Python
- Pandas
- NumPy
- XlsxWriter

---

## Repository Structure

```text
fpna-reporting-tool/
│
├── FP&A_Reporting_Tool.ipynb
├── sample_financials_FPA.xlsx
├── fpna_report_v1.xlsx
└── README.md
```

## Output Reports

The tool automatically generates:

| Report | Purpose |
|----------|----------|
| Executive Summary | High-level management overview |
| Summary | Variance analysis by account |
| Summary_BU | Variance analysis by business unit |
| Monthly Breakdown | Monthly performance review |
| Driver Forecast | Forecast output by business unit and account |
| Forecast Methodology | Forecast assumptions and logic |
| Three Month Forecast | Complete forecast breakdown |
| Data Quality Issues | Data validation findings |

---

## Sample Output

### Sample Input Dataset

The sample dataset intentionally contains inconsistent date formats, missing values and non-numeric entries to demonstrate the tool's data quality validation capabilities.

<img width="384" height="592" alt="FPA_Tool Sample_Input" src="https://github.com/user-attachments/assets/dd61a8db-e84c-418a-a3d2-4452ba5c992e" />

### Executive Summary

Management-level summary highlighting key variances, issue counts and forecast metrics.

<img width="375" height="333" alt="FPA_Tool Executive_Summary" src="https://github.com/user-attachments/assets/fd87c8af-da47-4031-8b37-6dfe660dd20c" />

### Driver-Based Forecast

Three-month forecast generated using configurable business drivers and assumptions.

<img width="380" height="365" alt="FPA_Tool Driver_Forecast" src="https://github.com/user-attachments/assets/ec8efcfe-bf7c-4020-b327-f369e8ddf86a" />

---

## Forecast Methodology

The forecasting approach uses a simplified FP&A driver-based model.

| Driver | Method |
|----------|----------|
| Revenue | 3-Month Historical Average × Growth Assumption |
| COGS | Fixed Percentage of Forecast Revenue |
| Salaries | Latest Actual × Growth Assumption |
| Other Accounts | Historical Average |

---

## Business Value

| Process Area | Traditional Workflow | Automated Workflow |
|-------------|---------------------|-------------------|
| Data Validation | Manual review of missing values, date formats and input errors | Automated detection and reporting of data quality issues |
| Variance Analysis | Spreadsheet formulas and manual investigation | Automated variance calculations and severity classification |
| Management Reporting | Manual report preparation and consolidation | Automated generation of executive reporting outputs |
| Forecast Preparation | Manual maintenance of forecast files | Driver-based forecast generation using configurable assumptions |
| Auditability | Risk of manual overwrites and inconsistent calculations | Transparent and repeatable calculation logic |

---

## Future Enhancements

- Scenario modelling (Base / Upside / Downside)
- Forecast vs Actual tracking
- Dynamic forecast assumptions
- Forecast accuracy metrics
- Interactive visualizations and trend reporting

---

