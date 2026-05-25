# Epic Healthcare Revenue Dashboard

## Overview
This project analyzes healthcare operational and financial performance using Tableau. The dashboard focuses on reimbursement trends, insurance performance, claims status, and operational efficiency.

## Tools Used
- Tableau
- Excel
- Google Sheets
- SQL (basic)

## KPIs
- Total Claims
- Total Reimbursement
- Average Claim Amount

## Key Insights
- Orthopedics generated the highest reimbursement totals
- Medicaid had the highest average claim amount
- Self-pay insurance produced the lowest average claim amount
- Medicaid claims required the longest processing time

## Recommendations
- Improve Medicaid processing workflows
- Investigate denial trends in Orthopedics and Pediatrics
- Expand successful approval strategies from Primary Care

## Project Files
- Tableau Dashboard PDF
- Healthcare Dataset
- Dashboard Screenshots<img width="488" height="345" alt="KPI_Summary_Table" src="https://github.com/user-attachments/assets/b1924063-621e-4e83-b48b-c19798144c3e" />
<img width="622" height="519" alt="Screenshot 2026-05-25 at 5 03 58 AM" src="https://github.com/user-attachments/assets/d43733a7-4f8a-4cbd-a3b0-ff235e0cb9af" />

## Basic SQL Queries
```sql
-- Total number of claims
SELECT COUNT(*) AS total_claims
FROM healthcare_claims;

-- Average claim amount by insurance type
SELECT insurance_type,
       AVG(claim_amount) AS avg_claim_amount
FROM healthcare_claims
GROUP BY insurance_type;

-- Total reimbursement by department
SELECT department,
       SUM(reimbursement_amount) AS total_reimbursement
FROM healthcare_claims
GROUP BY department;

-- Average processing time by insurance type
SELECT insurance_type,
       AVG(days_to_process) AS avg_processing_days
FROM healthcare_claims
GROUP BY insurance_type;
```

## Scheduling Operations Dashboard

### Overview
This project analyzes hospital scheduling operations using Tableau. 
The dashboard focuses on appointment trends, provider utilization, cancellation analysis, and no-show tracking.

### Tools Used
- Tableau
- Excel
- Google Sheets

### KPIs
- Total Appointments
- No Show Rate
- Provider Utilization %
- Average Wait Time

### Key Insights
- Primary Care had the highest provider utilization
- Orthopedics showed longer patient wait times
- No-show rates were highest among follow-up visits
- Completed appointments represented the majority of visits

### Recommendations
- Reduce wait times in Orthopedics
- Implement appointment reminders to reduce no-shows
- Improve provider scheduling balance across departments
- Monitor cancellation trends weekly
- <img width="560" height="389" alt="Appointments Dashboard" src="https://github.com/user-attachments/assets/bb8f8615-418e-41b3-b4d1-eb6632614fdd" />
<img width="479" height="223" alt="KPI Summary Table" src="https://github.com/user-attachments/assets/4a035a93-b798-4c7f-ae3c-32416ec5bdbc" />


