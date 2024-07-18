# Employee Satisfaction Analysis

This repository contains the final project from the IST 687 Introduction to Data Science course. The project analyzes employee satisfaction data to provide actionable insights for improving satisfaction and retention in a European company. The independent data science team, consisting of Tibaria Al Nouri, Katherine Martinez, Stephen Price, and Yesul Song, was tasked by the HR department to uncover the factors behind low employee satisfaction.

## Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Skills Demonstrated](#skills-demonstrated)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results and Analysis](#results-and-analysis)
  - [Reasons for Leaving](#reasons-for-leaving)
  - [Attrition by Department](#attrition-by-department)
  - [Satisfaction by Salary Bracket](#satisfaction-by-salary-bracket)
  - [Satisfaction Linked to Projects](#satisfaction-linked-to-projects)
  - [Satisfaction in Relation to Hours Worked](#satisfaction-in-relation-to-hours-worked)
  - [Satisfaction in Relation to Retention](#satisfaction-in-relation-to-retention)
  - [Does Geography Play a Role in Satisfaction?](#does-geography-play-a-role-in-satisfaction)
  - [Regression Analysis](#regression-analysis)
- [Next Steps](#next-steps)
- [Repository Structure](#repository-structure)

## Project Overview

In the rapidly evolving landscape of today's corporate world, employee satisfaction stands as a linchpin to organizational success. A satisfied workforce not only bolsters productivity but also strengthens brand reputation, ultimately impacting the bottom line. It's with this understanding that our independent data science team was commissioned by the HR department of a notable European company. Tasked with the mission of unraveling the intricacies behind their troublingly low employee satisfaction rates, we embarked on a comprehensive exploration of their expansive dataset. This report chronicles our approach, findings, and the invaluable insights gleaned, which we hope will pave the way for enhanced employee satisfaction and, by extension, company success.

## Objectives

- **Identify** key factors contributing to employee dissatisfaction and attrition.
- **Analyze** the relationship between satisfaction and various factors such as salary, projects, and hours worked.
- **Provide** recommendations to the HR department to improve employee satisfaction and retention.

## Skills Demonstrated

- **Data Cleaning and Preprocessing**: Formatting data types for consistency and addressing missing or null values.
- **Exploratory Data Analysis**: Grouping data for visualizations and geographical plotting.
- **Statistical Analysis**: Conducting regression analysis to identify potential correlations.
- **Data Visualization**: Creating insightful visualizations to highlight trends (using ggplot2, plotly).
- **R Programming**: Implementing data analysis and visualization techniques using R.

## Dataset

The dataset provided by the HR department includes detailed information on employee satisfaction, department, salary, projects, and hours worked. The spreadsheet covers 14,999 rows with 18 columns, giving our team 26,982 data points to analyze. The key variables are:

- **Target satisfaction score**: Goal or benchmark for employee satisfaction.
- **DOJ (date of job)**: Employee's joining date.
- **Department**: Division or segment of the company.
- **Employee Code**: Unique identifier for each employee.
- **Employee Status**: Current working status (e.g., Active, Resigned).
- **Employee Satisfaction score (Prior)**: Previous satisfaction rating.
- **Employee Satisfaction score (Latest)**: Most recent satisfaction rating.
- **Monthly work hours**: Hours worked monthly.
- **No of Yrs spent in company**: Duration of employment in years.
- **Number of Projects undertaken**: Total projects handled by the employee.
- **Promotion in the last 5 yrs**: Indicates promotion in the past 5 years.
- **Reason for Leaving**: Explanation for resignation or termination.
- **Salary bracket**: Range indicating pay scale.
- **Sno**: Serial or unique identifier.
- **Work @ accident**: Incidents at work.
- **City**: Employee's city of work or residence.
- **State**: State of work or residence.
- **Country**: Country of work or residence.

## Methodology

To ensure our analysis was robust and comprehensive, we adhered to a methodology that's recognized as a standard across the data analytics landscape. This systematic approach breaks down the analysis into distinct stages, each integral to the success and credibility of the insights derived. The stages are:

1. **Defining the Question**:
    - Framing our analysis with precise questions to provide direction and narrowing our focus, ensuring the data is viewed through a lens relevant to the company's concerns.

2. **Data Collection**:
    - Procuring the necessary dataset from the HR department. The quality and comprehensiveness of this data were crucial, as it formed the backbone of our entire analysis.

3. **Data Cleansing**:
    - Formatting data types for consistency.
    - Identifying and addressing any missing or null values, ensuring the dataset's integrity.

4. **Data Analysis**:
    - Grouping the data for targeted visualizations, such as bar charts and scatterplots.
    - Geographical plotting to visualize employee distribution and satisfaction trends across regions.
    - Executing regression analysis to identify potential correlations between variables.

5. **Sharing Results**:
    - Compiling our findings into a comprehensive report. We prioritized clarity and actionable insights, aiming to provide the HR department with tools they need to address their concerns about employee satisfaction.


## Results and Analysis

### Reasons for Leaving

The primary reasons employees cited for departing the company were related to remuneration, the allure of better opportunities at competing firms, and lack of encouragement and their immediate supervisors. Notably, these last two reasons were closely aligned in terms of their frequency of mention.

![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/1d784fce-66ac-4cb2-b250-c97311e5d93f)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/e7155b5b-71b7-4f3e-b878-09da12f0048d)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/fd5a994a-736a-4f0f-81dd-c34218f62a0b)

Among those top 4 reasons for leaving, when looked at by departments with the highest volume of attrition, it seems all departments struggle in the same way to address these concerns. The ranking becomes pay, better prospects elsewhere, work pressure, and lack of encouragement in that order.

### Attrition by Department

The departments that exhibited the highest attrition rates were Sales, Technical Support, and IT. However, when examining departures in relation to the size of each department, the proportion was consistent, with attrition rates ranging between 25-30%.

![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/87a348a6-414a-43e3-a873-6ca009bde44e)

Among those who left the company, the Accounting department surfaced with the lowest satisfaction score, closely trailed by IT.

### Satisfaction by Salary Bracket

Our initial discussions were to dive into the salary brackets to determine if there is a compensation issue within the organization. Furthermore, our regression analysis showed that low and medium salary brackets were statistically significant. However, more information and data are needed to confidently state that salary brackets are an issue. Benchmarking all job categories and doing geographical benchmarking are necessary to determine if the organization is paying fair market value for the services rendered by employees.

![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/6015abf6-334d-4c3b-9245-e2d661f40297)

When breaking down each salary bracket by department, we recognize that the distribution of average satisfaction is similar across salary brackets. While the same department does not show the lowest satisfaction in each bracket, the value of the low and high department are similar across salary brackets.

### Satisfaction Linked to Projects

The following graphs investigate any correlation between the number of projects employees are assigned, their satisfaction rating, grouped by department, and broken up by those employed and those who left. It becomes clear there is a threshold for the number of projects an employee takes on before their satisfaction score begins to diminish.

Loading employees with 6 or more projects seems to leave them feeling overworked and extremely unsatisfied. Those who left the organization had a low satisfaction of 10% while their peers in the company had 40-50% satisfaction – far below the company target and the average.

![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/9060c658-bf3f-4e43-a4d4-380f576dd4d0)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/03c7a9fa-de4f-419e-8743-e1828474d370)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/c19c0eb9-a962-4462-8d32-218abe1532a5)

Employees who had 3 or fewer projects and left the organization ranked the company around 42% for satisfaction. In contrast, those who left the company but had 4-5 projects ranked around 75% satisfaction. There seems to be a sweet spot between the number of projects assigned and satisfaction. Those under or over-worked at the company show signs of low satisfaction in contrast to those with a healthy workload.

### Satisfaction in Relation to Hours Worked

To further iterate the point made above, the number of projects likely correlates to the hours clocked in an organization. While the results of satisfaction and hours worked are a bit varied for employees currently at the organization, there is still a significant cluster in high satisfaction for employees clocking 150-300 hours.

![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/3635d16b-56a8-4c36-8947-736c9c4f46e2)

These points are made even more obvious by employees who left the organization. To the left of the graph below, employees who left the company and were underutilized (fewer hours worked) also had a very low satisfaction rating circled in red. The employees in the bottom right who left and were highly utilized (overworked) clocking around 250-350 hours a month, had an extremely low satisfaction rating. Interestingly the cluster in the top right shows employees who left the company with a high satisfaction rating. These employees worked 215-275 hours a month. Once again there is a clear middle spot where being underutilized may leave employees listless and uninspired, but those working over 250 hours a month are even more at risk of dissatisfaction with the company.

![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/10cffc36-6cde-412c-a783-f3bbd9d935a2)

### Satisfaction in Relation to Retention

Of the 10,000 points, there is no evidence of a single employee leaving after 6 years with the organization. These employees provide key insight into opportunities for higher retention. Interestingly, their satisfaction is not much higher - it hovers around the target 65-70% range. In contrast, employees with a higher satisfaction rating in their 5th and 6th years still left. There is something to be said about overall satisfaction in unison with longevity and retention.

### Does Geography Play a Role in Satisfaction?

Germany and Portugal had the highest satisfaction rating above 90% while Spain had the lowest below 60%. We cannot say anything definitively about geography in relation to satisfaction as there could be many factors at play such as the departments hosted in these countries, taxes, quality of life, etc. But this data does provide us opportunity to deep dive into these different areas for more insights.

![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/3b5ee827-1450-4e51-85af-2a5486e51013)

### Regression Analysis

The regression analysis provided a lot of insight on the highest correlated factors impacting employee satisfaction. We built a linear regression model predicting ‘Employee Satisfaction (Latest)’ using the following factors:
- Monthly work hours
- No of Years spent in company
- Number of Projects undertaken
- Salary bracket (low)
- Salary bracket (medium)

From the results of the model, we concluded the following for each factor:
1. **Number of Projects undertaken**: The coefficient is -0.03004. This suggests that for each additional project an employee undertakes, their satisfaction score decreases by approximately 0.03004 units. Therefore, having a higher number of projects is associated with lower employee satisfaction.
2. **Monthly work hours**: The coefficient is 0.0002613. This indicates that for each additional hour an employee works per month, their satisfaction score increases by approximately 0.0002613 units. The effect is quite small, suggesting that increased work hours have a minimal positive impact on satisfaction.
3. **No of Years spent in company**: The coefficient is -0.01377. This implies that for each additional year an employee spends in the company, their satisfaction score decreases by approximately 0.01377 units. Longer tenure in the company is associated with slightly lower employee satisfaction.
4. **Salary bracket (low)**: The coefficient is -0.03953. Being in the "low" salary bracket is associated with a decrease of approximately 0.03953 units in employee satisfaction. Lower salary brackets are linked to lower employee satisfaction.
5. **Salary bracket (medium)**: The coefficient is -0.01690. Being in the "medium" salary bracket is associated with a decrease of approximately 0.01690 units in employee satisfaction. Similarly, the "medium" salary bracket is linked to lower employee satisfaction.

![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/f6ae5020-679f-489b-ac55-11e4bfef914a)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/12fa8013-26d3-46fc-aff6-0ad10bef01e4)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/0cbb03d3-a5f2-4031-b62a-775e49fb0aa7)

## Next Steps

This analysis is meant to provide a high-level look for company leaders to make data-driven decisions. Compensation, better opportunities at competing firms, lack of encouragement and immediate supervisors are the top cited reasons for leaving. However, the regression analysis showed salary among other factors only predicted 3% of the satisfaction rating. This analysis highlighted a clear trend in hours worked/projects undertaken and employee satisfaction. The company could address high-risk employees who are either under or over-utilized and bring them in alignment with other more satisfied employees of the company.

Practical next steps include:
- Monitoring the number of projects people are assigned.
- Monitoring the overtime or hours people are working.
- Focusing on opportunities to develop employees.

We look forward to partnering with you and discussing these results further.

## Repository Structure
```plaintext
Employee-Satisfaction-Analysis/
├── data/
│   ├── Employment_data.xlsx
├── Employee_Satisfaction_Analysis.Rmd
├── Employee_Satisfaction_Analysis_report.docx
├── README.md
├── LICENSE
