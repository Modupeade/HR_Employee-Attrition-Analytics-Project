# HR Employee Attrition Analytics Project

## Table of Content
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools and Technologies Used](#tools-and-technologies-used)
- [Data Preparation](#data-preparation)
- [Data Analysis](#data-analysis)
- [Insights Findings](#insights-and-findings)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)

### Project Overview
This data analysis project aims to provide insights into employee attrition at IBM by comparing the characteristics of employees who have left the company with those who remain employed. The goal is to identify key trends, understand factors influencing employee turnover, and make data-driven recommendations that can help improve employee retention and overall company performance.


![HR Employee Attrition Analysis](https://github.com/user-attachments/assets/f49ba507-f401-4485-be7d-d64dbf27b7a9)

### Data Sources
HR Attrition Data: The data was sourced from Kaggle and contains both demographic and job-related attributes of employees.

### Tools and Technologies Used
  - Power BI – For data visualization and report creation.
  - Power Query – For data transformation and cleaning.
  - DAX (Data Analysis Expressions) – For creating custom calculations and measures.
  - Excel – For initial data exploration.

### Data Preparation
1. Data Cleaning: Data has no missing values and duplicates, and data types was formatted using Power Query.
2. Data Transformation: Standardized column names, created calculated columns, and applied data normalization where necessary.

### Data Analysis 
Using DAX Measures & Calculations
Attrition Rate
  ```
  Attrition_Rate =
  DIVIDE(SUM(Employee[AttritionCount]), SUM(Employee[EmployeeCount]))
  ```
  - Calculates the percentage of employees who left the company.
    
Job Role
  ```
  Job_roles =
  DISTINCTCOUNT(Employee[JobRole])
  ```
  - Count distinct job role 

Active Employee
  ```
  CountActives =
  SUM(Employee[EmployeeCount]) - SUM(Employee[AttritionCount])
  ```
  - Counts the number of employees who remain in the company.
    
### Insights and Findings

High Attrition in Life Sciences & Medical Educational Fields: Employees with backgrounds in Life Sciences and Medical education fields are more likely to leave the company, possibly due to job dissatisfaction or workload-related challenges.
Impact of Age Band and Gender: Employees aged between 31-40, particularly males, have the highest attrition rate.
Marital Status Influence: Single males exhibit a significantly higher attrition rate compared to divorced employees.

### Recommendations
Based on the analysis I would recommend the follwing actions:
1. Reduce Attrition in Life Sciences & Medical Fields
- Gather employee feedback to identify job dissatisfaction.
- Provide career development opportunities and training.
- Review workload and compensation for fairness.
- Foster a positive work culture with recognition programs.
 
2. Address High Attrition Among Employees Aged 31-40 (Especially Males)
- Implement leadership development and mentorship programs.
- Improve work-life balance with flexible work options.
- Offer competitive salaries and performance incentives.
     
3. Retain Single Male Employees
- Enhance social engagement through networking and team-building activities.
- Provide financial wellness programs and career growth opportunities.
- Support work-life balance with mental health and wellness initiatives.

### Conclusion
  This Power BI report highlights key factors influencing attrition and provides actionable insights. The findings can help HR teams develop targeted retention strategies,     ultimately reducing employee turnover and improving overall company performance.
  
### References
[Dataset](kaggle.com)

[Flaticons](https://www.flaticon.com/)

Thank you 🙂  
