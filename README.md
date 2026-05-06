# HR-Analytics
With a focus on HR analytics, this Power BI project seeks to offer insights into several facets of an organization's human resources. 

## Project Overview
This project analyzes employee attrition trends using HR data and provides insights into workforce distribution, salary trends, and employee turnover.

The dashboard helps HR teams identify departments, job roles, and demographic groups with higher attrition rates.

---

## Problem Statement
Employee attrition impacts hiring costs, productivity, and workforce planning.

The objective of this project was to:
- Analyze employee attrition patterns
- Identify departments with high employee turnover
- Understand job role distribution
- Track salary metrics
- Provide HR recommendations

---

## Tools Used
- Power BI
- Power Query
- DAX
- Excel/CSV dataset

---

## Dataset Information
The dataset includes:

- Employee ID
- Employee number
- Age
- Gender
- Department
- Job Role
- Monthly Income
- Attrition
- Education
- Marital Status
- Standard hours
- Performance Rate
- Daily rate
- Hourly rate
- Monthly rate

---

## Data Cleaning Steps
Performed data cleaning using Power Query:

- Checked missing values
- Verified data types
- Removed duplicates
- Standardized categorical fields
- Validated salary columns

---
## Screenshots Included:
<img width="1086" height="612" alt="image" src="https://github.com/user-attachments/assets/65542fbf-9625-42b6-b6b8-d98f07afb180" />

## Dashboard Insights
# Total Employees
Total workforce: 1,000 employees
# Gender Distribution
Male employees: 60%
Female employees: 40%
# Attrition Rate
Overall attrition rate: 16%
# Department Insights
- Majority employees stayed in the company
- Attrition cases are significantly lower compared to retained employees
# Job Role Insights
Higher employee concentration observed in:
- Sales Executive
- Research Scientist
- Laboratory Technician

# Business Recommendations
-Investigate causes of attrition in high-turnover roles
-Improve employee retention strategies
-Review compensation structures
Enhance employee engagement initiatives

## DAX Measures Created

 Total Employees
```DAX
Total Employees = COUNT(HR_Analytics[EmployeeNumber])
---

Avg Salary = AVERAGE(HR_Analytics[MonthlyIncome])

----
Attrition Rate

Attrition Rate = DIVIDE(CALCULATE(COUNT(HR_Analytics[EmployeeNumber]),HR_Analytics[Attrition] = "Yes"),
    COUNT(HR_Analytics[EmployeeNumber]))



