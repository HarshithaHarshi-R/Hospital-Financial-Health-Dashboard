# Hospital-Financial-Health-Dashboard
Power BI dashboard analyzing hospital billing and payment risk across departments

## Project Overview
An independent Power BI dashboard analysing the financial health 
of a hospital across 5 years (2020–2024), built on a 50,000-row 
hospital management dataset. The dashboard tracks revenue billed 
vs collected, outstanding balances, insurance coverage, and payment 
risk concentration across departments.

## Business Problem
Hospitals often struggle to track where revenue is being lost — 
whether through unpaid bills, insurance gaps, or EMI defaults. 
This dashboard answers: *How much money is owed, how much has been 
collected, and where is the financial risk concentrated?*

<img width="1159" height="656" alt="Page1" src="https://github.com/user-attachments/assets/a24e8c6c-cf56-46b6-8a64-7115601ef78b" />

<img width="1168" height="656" alt="Page 2" src="https://github.com/user-attachments/assets/4d462117-2550-4459-88b0-cb1a6eb21c77" />

### Page 1 — Revenue Overview
- Total billing, collections, pending, and insurance KPIs
- Monthly billing trend from 2020 to 2024
- Department-wise total billing (Oncology highest at ₹236M)
- Room type billing split (General 47%, Private 32%, ICU 20%)

### Page 2 — Payment Risk & Collections
- 25% of net payable (₹354M) remains uncollected
- Paid vs Pending breakdown by all 12 departments
- Payment mode split — Cash, Card, and EMI nearly equal
- Insurance vs out-of-pocket amount by department
- EMI risk table showing pending by 3, 6, and 12 month plans

## Key Insights
- ₹354M (25% of net payable) is outstanding across all departments
- Oncology carries the highest pending risk at ₹45M
- Card and Cash payments account for ~80% of collections
- General ward admissions represent 47% of total billing volume
- Insurance covers ₹473M, leaving significant out-of-pocket exposure

## Tools & Techniques
- **Power BI Desktop** — report building and data modelling
- **Power Query** — data cleaning, type standardisation, 
  null handling, derived columns
- **DAX** — 11 custom measures including CALCULATE, DIVIDE, SUM
- **Data Model** — star schema with Admissions as central fact table, 
  connected to Billing, Treatment, Patients, Doctors, 
  Departments, and Calendar

## Dataset
- Source: Kaggle — Hospital Patient Treatment Management System
- 50,000 admission records across 7 related tables
- Date range: January 2020 to December 2024
