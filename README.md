# Project Background

The goal of this project is to analyze and predict employee attrition using a fictional dataset created by IBM data scientists. This dataset contains various features that may influence employee turnover, such as job roles, monthly income, education, and distance from home. By conducting an exploratory data analysis (EDA), we aim to uncover key factors that contribute to attrition, including insights like job role distribution and how distance from home correlates with attrition.

After the data cleaning process, which involves handling missing values, outliers, and inconsistent data entries, we proceed with feature engineering and visualization to better understand the dataset. The ultimate objective is to build and evaluate a predictive model using classification algorithms to determine whether an employee is likely to leave the company. This can be leveraged by HR teams to create targeted retention strategies and improve employee satisfaction.

Insights and recommendations are provided on the following key areas:
```
* Insights on the impact of monthly income on attrition.
* Insights on the effect of Age on the attrition of employees.
* Insights on whether particular job roles increase likihood of attiriton by employees in those roles.
* The impact of overtime and lack of a work-life balance has on the attrition rate of employees.
* Recommendations on compensation structure
* Targeted Retention Strategies for At-Risk Job Roles
* Work-Life Balance Initiatives
```

The Jupyter Notebook used to inspect and clean the data for this analysis can be found here [link]().

The Jupyter Notebook regarding various business questions and visualizations can be found here [link]().

An interactive Power BI dashboard used to report and explore sales trends can be found here [link](https://app.powerbi.com/view?r=eyJrIjoiMzk1YjI0NTUtMTFjZi00MzRhLThkOGMtOGZkMDFiMGU1OWQxIiwidCI6IjVjMjAwZWZhLTZiZDAtNDVkZi05ZDMxLTg3MTgxZjY0NzhiYyJ9&embedImagePlaceholder=true).

# Data Structure & Initial Checks
The datacard describiing this dataset can be found at [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset/data) A short summary of the features is described below:

| Feature | Data Type | Description | 
| ------- | --------- | ----------- |
| Age | Integer | The age of the employee. |
| Attrition | String | Whether the employee has left the organisation or not. |
| BusinessTravel | String | Frequency which an employee travels. |
| DailyRate | Integer | Daily rate of the employee. |
| Department | String | Name of the department the employee works in. |
| DistanceFromHome | Integer | Distance the employee has to travel to work. |
| Education | Integer | The education level of the employee. |
| EducationField | String | What the employee studied during their education. |
| EmployeeCOunt | Integer | A binary count of all the employees in the organisation. |
| EmployeeNumber | ID | Identification number for each employee. |
| EnvironmentalSatisfaction | Integer | Satisfaction rating of the work enviornment on a scale of 1 to 4. |
| Gender | String | The gender of the employee. | 
| HourlyRate | Integer | The employees rate per hour. |
| JobInvolvement | Integer | Involvement rating of the work required for role, on a scale of 1 to 4. |
| JobLevel | Integer | The hierachial level of the job responsibilities of the employee, from a scale of 1 to 4. |
| JobRole | String | The job the employee does within the organisation. |
| JobSatisfaction | Integer | The level of satisfaction in the work the employee does in their role on a scale of 1 to 4. |
| MaritalStatus | String | The employee's marital status. |
| MonthlyIncome | Integer | The monthly income of the employee. |
| MonthlyRate | Integer | The rate of the employee per month. | 
| NumOfCompaniesWorked | Integer | The total number of companies the employee has worked for before. |
| Over18 | String | Whether the employee is over the age of 18 or not. |
| OverTime | String | Whether the employee has worked overtime or not. | 
| PercentSalaryHike | Integer | The percentage increase an employee received from their previous monthly income. |
| PerformanceRating | Integer | The rating of the employees performance within the organisation, on a scale of 1 to 4. |
| RelationshipSatisfaction | Integer | The rating of the relationship the employee has with other staff memebers within the organisation. |
| StadardHours | Integer | The standard working hours of the employee. |
| StockOptionLevel | Integer | Whether the employee has stock level options, and what level the stick level option is. Value greater than 0 is represents stock option for the employee. |
| TotalWorkingYears | Integer | The total working years for the employee. | 
| TrainingTimesLastYear | Integer | The total number of times the employee received training the previous year. | 
| WorkLifeBalance | Integer | A rating of the work-life balance of the employee from a scale of 1 to 4. |
| YearsAtCompany | Integer | The total  number of years the employee has been in the organisation. |
| YearsInCurrentRole | Integer | The total number of years the employee has been in their current job role. |
| YearsSinceLastPromotion | Integer | The total number of years since the employees last promotion. | 
| YearsWithCurrManager | Integer | The total number of years spent with their current manager. |

# Executive Summary
