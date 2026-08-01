# HR-Data-Analysis
Overview

This project explores an employee-level HR dataset to understand attrition (employee turnover) and the factors associated with it. Exploratory data analysis (EDA) was performed on the raw data, and the findings were built into an interactive Power BI dashboard (HR_data_analysis.pbix) with two report pages: an Overview page and a Deep-Dive / Attrition Drivers page.

Dataset

The data model contains a single table, HR_Analytics, with employee-level records. Fields used across the dashboard include:

Category	Columns
Demographics	Age, AgeGroup, Gender, MaritalStatus, DistanceFromHome
Job Info	Department, JobRole, First JobRole, OverTime
Tenure	YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion
Compensation	MonthlyIncome
Satisfaction	JobSatisfaction, WorkLifeBalance, EnvironmentSatisfaction
Target / Outcome	Attrition (Yes/No)

Key measures (DAX):

Total Employees
Active Employees
Attrition Count
Attrition Rate
Average Salary
Average Age
Count of Attrition
Count of OverTime
Exploratory Data Analysis (EDA)

Before building the dashboard, EDA was carried out on the dataset to:

Check data quality (missing values, duplicates, data types) across demographic, job, tenure, and compensation fields
Understand the distribution of employees by department, job role, gender, marital status, and age group
Calculate headline KPIs — total employees, active employees, average age, average salary, and overall attrition rate
Identify variables that appear to correlate with attrition (e.g., overtime, income, tenure, satisfaction scores, distance from home) to shortlist the "key drivers" surfaced in the dashboard
Dashboard Structure
Page 1 — Overview
KPI cards: Total Employees, Average Salary, Average Age, Attrition Rate, Active Employees, Attrition Count
Attrition by Department (bar chart)
Attrition by Job Role (bar chart)
Attrition by Age Group (clustered column chart)
OverTime vs Attrition (donut chart)
Gender split (donut chart)
Slicers: Gender, Department, Marital Status
Page 2 — Attrition Drivers (Deep Dive)
Key Drivers visual: analyzes Attrition against Age, OverTime, JobSatisfaction, WorkLifeBalance, MonthlyIncome, YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion, EnvironmentSatisfaction, and DistanceFromHome to automatically surface the strongest predictors of attrition
Decomposition Tree: breaks down Attrition Count by Department, Gender, Job Role, Age Group, OverTime, and Marital Status for root-cause drill-down
Monthly Income vs Years at Company (scatter plot, colored by Attrition)
Attrition by Years Since Last Promotion (clustered column chart)
Slicer: First Job Role
Key Insights

(Fill in with your specific findings once reviewed — suggested talking points based on the visuals built)

Which department/job role has the highest attrition rate
Whether employees working overtime attrite at a noticeably higher rate
Whether low job satisfaction / work-life balance correlates with attrition
Whether attrition is concentrated among employees with fewer years since their last promotion or shorter tenure
Any pattern between monthly income and attrition risk
How to Use the Dashboard
Open HR_data_analysis.pbix in Power BI Desktop.
Use the slicers (Gender, Department, Marital Status, First Job Role) to filter the views.
Start on Page 1 for a high-level snapshot, then move to Page 2 for driver analysis and drill-downs via the Decomposition Tree.
Hover over the Key Drivers visual to see the relative influence of each factor on attrition.
Tools Used
Power BI Desktop — data modeling, DAX measures, and dashboard visuals
Exploratory Data Analysis performed on the source HR dataset prior to dashboard development
File
HR_data_analysis.pbix — Power BI report file containing the data model, measures, and both report pages
