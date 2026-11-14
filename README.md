# Hospital Emergency Room Management Dashboard

![Microsoft Excel](https://img.shields.io/badge/Tool-Microsoft%20Excel-217346?logo=microsoft-excel&logoColor=white)
![Domain](https://img.shields.io/badge/Domain-Healthcare%20Analytics-0A7EA4)
![Project](https://img.shields.io/badge/Project-Data%20Analytics-blue)

An Excel-based healthcare analytics project designed to explore emergency room (ER) patient activity, admission patterns, waiting times, patient satisfaction, and department referrals. The workbook contains a dashboard, a patient-level data sheet, pivot-based summaries, and supporting trend-analysis sheets.

## Table of Contents

- [Project Overview](#project-overview)
- [Business Problem](#business-problem)
- [Project Objectives](#project-objectives)
- [Tools and Techniques](#tools-and-techniques)
- [Dataset Description](#dataset-description)
- [Dashboard Preview](#dashboard-preview)
- [Dashboard and Analysis](#dashboard-and-analysis)
- [Key Metrics in the Pivot Report](#key-metrics-in-the-pivot-report)
- [Data Quality Note](#data-quality-note)
- [Repository Structure](#repository-structure)
- [How to Use](#how-to-use)
- [Skills Demonstrated](#skills-demonstrated)
- [Author](#author)

## Project Overview

Emergency departments need to understand patient volumes, admission outcomes, waiting times, and patient experience to monitor operational performance. This project uses Microsoft Excel to organize and summarize emergency room patient records and present selected metrics through charts and a dashboard.

The workbook includes **608 patient records** in its `DATA` worksheet and 13 fields covering patient demographics, visit information, admission outcomes, waiting time, satisfaction, and attendance status.

## Business Problem

Emergency room teams need visibility into questions such as:

- How many patients are visiting the emergency department?
- What proportion of patients are admitted?
- How long do patients wait?
- How does patient satisfaction vary?
- Which departments receive the most referrals?
- How do patient volumes and operational measures change over time?

This dashboard provides a consolidated view of these measures to support exploration and operational discussion. It is an analytical reporting project and does not establish clinical or causal conclusions.

## Project Objectives

1. Summarize emergency room patient activity.
2. Examine admission and non-admission patterns.
3. Monitor average patient waiting time.
4. Review recorded patient satisfaction scores.
5. Explore patient demographics and age groups.
6. Analyze department referral patterns.
7. Present key summaries and trends in an Excel dashboard.

## Tools and Techniques

**Tool identified in the supplied project file:** Microsoft Excel.

Workbook elements identified during inspection:

- Excel tables / structured patient data
- Pivot-based summary reports
- Charts and dashboard visualizations
- Daily trend worksheets for patient count, waiting time, and satisfaction

> The workbook was inspected as an Excel file. This README does not claim the use of SQL, Python, Power BI, Power Query, or Power Pivot because those workflows are not evidenced in the supplied file.

## Dataset Description

The `DATA` worksheet contains 608 patient records and the following 13 fields:

| Field | Description |
|---|---|
| Patient Id | Unique patient record identifier |
| Patient Admission Date | Date of the ER visit |
| Patient Admission Time | Time of the ER visit |
| Patient Name | Patient name field in the supplied dataset |
| Patient Gender | Recorded gender category |
| Patient Age | Patient age in years |
| Patient Race | Recorded race category |
| Department Referral | Department referral category |
| Patient Admission Flag | Admitted or not admitted |
| Patient Satisfaction Score | Recorded satisfaction score |
| Patient Waittime | Waiting time, in minutes |
| Age Group | Categorized patient age |
| Patient Attend Status | Attendance status recorded in the dataset |

### Dataset snapshot

- Records in `DATA`: **608**
- Fields: **13**
- Unique patient IDs: **608**
- Admission date range in `DATA`: **June 1, 2023 – June 30, 2024**
- Satisfaction scores are missing for many records in the `DATA` sheet; interpret satisfaction metrics with this limitation in mind.

## Dashboard Preview

![Hospital Emergency Room Dashboard](screenshots/dashboard-preview.png)

*Snapshot of the Excel Interactive Dashboard displaying patient counts, waiting times, satisfaction scores, admission status, gender distribution, and department referrals.*

## Dashboard and Analysis

The workbook contains six worksheets:

| Worksheet | Role |
|---|---|
| `Dashboard` | Main dashboard containing seven charts |
| `DATA` | Patient-level source data |
| `PIVOT REPORT` | Pivot-based summaries and KPI calculations |
| `Daily ER No of patient` | Daily patient-volume trend |
| `Avg.Patient WaitTime` | Daily average waiting-time trend |
| `Avg.Patient Satisfaction Score` | Daily average satisfaction trend |

The pivot report includes summaries for:

- Total/distinct patient count
- Average patient waiting time
- Average patient satisfaction score
- Daily patient count
- Daily average waiting time
- Daily average satisfaction score
- Admission status and admission percentage
- Age-group distribution
- Gender distribution
- Department referrals
- Attendance status

## Key Metrics in the Pivot Report

The following values are read from the supplied `PIVOT REPORT` worksheet. They describe the pivot report as currently saved in the workbook; they should not be treated as recalculated metrics for all 608 rows in the `DATA` worksheet.

| Metric | Value shown in Pivot Report |
|---|---:|
| Patient count | 471 |
| Average waiting time | 34.05 minutes |
| Average satisfaction score | 5.312 |
| Admitted patients | 247 |
| Not admitted patients | 224 |
| Admission rate | 52.44% |
| Delayed attendance | 262 |
| On-time attendance | 209 |

## Data Quality Note

**Please review this before using the workbook for portfolio or business reporting.** The supplied workbook contains inconsistencies between the `DATA` worksheet and the saved pivot summaries:

- The `DATA` worksheet contains 608 unique patient records, while the pivot report shows 471 patients.
- The dates in `DATA` range from June 2023 to June 2024, while the daily pivot summaries are labelled October 1–30.
- Every row in the supplied `DATA` worksheet is marked `Delayed`, while the pivot report splits attendance into 262 `Delayed` and 209 `OnTime`.
- The `DATA` worksheet has many blank patient satisfaction scores.

These differences may indicate that the pivot tables/dashboard are based on a different or previously loaded source, or that the workbook has not been refreshed consistently. Before publishing final insights, verify the source range and filters, refresh the pivot tables/charts, and reconcile the dashboard totals with the source data. Do not combine the pivot-report KPIs with raw-data calculations until this is resolved.

## Repository Structure

Suggested GitHub repository layout:

```text
hospital-emergency-room-dashboard/
│
├── README.md
├── Project 1 Excel Hosptial Emergency Room Management Dashboard Excel.xlsx
└── screenshots/
    └── dashboard-preview.png
```

## How to Use

1. Download or clone this repository.
2. Open the Excel workbook in Microsoft Excel.
3. Review the `DATA` worksheet to understand the source fields.
4. Review the `PIVOT REPORT` and supporting trend worksheets.
5. Open the `Dashboard` worksheet to explore the visual summaries.
6. Verify and refresh the source data and pivot reports before relying on the displayed KPIs.

## Skills Demonstrated

- Healthcare data exploration
- Spreadsheet-based data analysis
- Pivot-based reporting
- KPI interpretation
- Trend analysis
- Data visualization
- Dashboard presentation
- Data quality awareness and validation

## Author

**Ashutosh Purkar**

Aspiring Data Analyst | B.Pharm Student

- GitHub: [Aashu18102005](https://github.com/Aashu18102005)
- LinkedIn: [Ashutosh Purkar](https://www.linkedin.com/in/ashutosh-purkar-3a3340270/)

---

*This project is intended for learning and portfolio demonstration. Patient data fields in the supplied workbook should be reviewed for privacy and de-identification before making the workbook publicly accessible.*