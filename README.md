# Project Background

This project aims to analyze and predict employee attrition using a fictional dataset created by IBM data scientists. This dataset contains various features that may influence employee turnover, such as job roles, monthly income, education, and distance from home. By conducting exploratory data analysis (EDA), we aim to uncover key factors contributing to attrition, including insights like job role distribution and how distance from home correlates with attrition.

After the data cleaning process, which involves handling missing values, outliers, and inconsistent data entries, we proceed with feature engineering and visualization to better understand the dataset. The ultimate objective is to build and evaluate a predictive model using classification algorithms to determine whether an employee is likely to leave the company. HR teams can leverage this to create targeted retention strategies and improve employee satisfaction.

# Key Insights
* Top Influencers of Attrition:
  1. Monthly Income
  2. Age
  3. Total Working Years
  4. Years at Company
  5. Overtime (Yes)

* **Early-Career Professional Cluster**:
  * Employees in this category, clustered by *MonthlyIncome*, *TotalWorkingYears*, and *YearsAtCompany*, exhibit the highest churn rates, with a retention rate of just **3:1**.

* **Attrition and Age**:
  * Younger employees, are most likely to leave, closely aligning with the early-career group averaging **31.14** years for **males** and **30.61** for **females**.

* **Income Disparities**:
  * **Early-career professionals** earn an average of **3459.08**, significantly below the **organisational average** of **6502.93**.

* **Job Level and Retention**:
  * Attrition is notably higher in entry-level roles. **Job Level 1** employees have a retention rate of **3:1**, with an **average income** of **2786.92**, while **Job Level 5** sees a retention rate of **13:1**, with **average earnings** of **19191.83**.

* **Overtime and Attrition Impact**:
  * Overtime work is consistent across clusters, with only **4.5%** rating their work-life balance **poorly**. This indicates that attrition is driven by a combination of factors, where financial compensation alongside overtime plays a significant role.

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
The analysis identifies key drivers of employee attrition, with compensation, career stage, and job level emerging as critical factors. Early-career professionals and entry-level employees show the highest churn rates, driven by lower earnings and limited progression opportunities. Notably, younger employees, especially those in early-career clusters, exhibit a strong tendency toward attrition, with those aged around 30 earning well below the organisational average.

Additionally, while overtime rates are consistent across clusters, their impact on attrition varies based on financial compensation, underscoring the importance of aligning work-life balance initiatives with competitive remuneration.

# Insights Deep Dive
### Retention rate per Clusters
The retention rates of each cluster can be found below. Based on the data in the graph, we can see that the employee clusters with the worst retention rates are the Early-career professionals and Veteran Professionals.

![output](https://github.com/user-attachments/assets/a17a43ee-b652-4dc6-bbca-1643e990d95f)

### Average MonthlyIncome per Employee Clustering
The monthly income of early-career employees is well below that of the organisation's mean income value. Knowing that income is a strong indicator for attrition, it brings further understanding on why early-career employees have the worst retention rate within the organisation. 

![output](https://github.com/user-attachments/assets/cab0c2dc-d033-47e2-bd66-e911b80c14d8)

### Total Attrition per Job Level
Based on the barplot, we can see that job roles in job level 1 have the worst retention rate. This further reiterates the inference that early-career professionals are the group of employees most likely to churn. This can be seen with how all he job roles of the early-career professionals are level 1 and level 2 job levels. 




