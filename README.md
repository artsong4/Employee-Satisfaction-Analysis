# Employee Satisfaction Analysis

## Project Overview
This repository contains the final project from the IST 687 Introduction to Data Science course. The project analyzes employee satisfaction data to provide actionable insights for improving satisfaction and retention in a European company. The independent data science team, consisting of Tibaria Al Nouri, Katherine Martinez, Stephen Price, and Yesul Song, was tasked by the HR department to uncover the factors behind low employee satisfaction.

## Methodology
1. **Defining the Question:** Framing analysis with precise questions to provide direction.
2. **Data Collection:** Procuring the dataset from the HR department.
3. **Data Cleansing:** Formatting data types for consistency and addressing missing or null values.
4. **Data Analysis:** Grouping data for visualizations, geographical plotting, and executing regression analysis to identify potential correlations.
5. **Sharing Results:** Compiling findings into a comprehensive report.

## Results and Analysis

### Reasons for Leaving
- Primary reasons: remuneration, better opportunities at competing firms, lack of encouragement, issues with immediate supervisors.
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/1d784fce-66ac-4cb2-b250-c97311e5d93f)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/e7155b5b-71b7-4f3e-b878-09da12f0048d)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/fd5a994a-736a-4f0f-81dd-c34218f62a0b)

### Attrition by Department
- Highest attrition rates: Sales, Technical Support, IT.
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/87a348a6-414a-43e3-a873-6ca009bde44e)

### Satisfaction by Salary Bracket
- Low and medium salary brackets significantly impact satisfaction.
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/6015abf6-334d-4c3b-9245-e2d661f40297)

### Satisfaction Linked to Projects
- 6+ projects: overworked, low satisfaction.
- 3 or fewer projects: 42% satisfaction (left).
- 4-5 projects: 75% satisfaction (left).
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/9060c658-bf3f-4e43-a4d4-380f576dd4d0)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/03c7a9fa-de4f-419e-8743-e1828474d370)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/c19c0eb9-a962-4462-8d32-218abe1532a5)

### Satisfaction in Relation to Hours Worked
- High satisfaction: 150-300 hours.
- Low satisfaction: underutilized (<150 hours) or overworked (250+ hours).
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/3635d16b-56a8-4c36-8947-736c9c4f46e2)

### Satisfaction in Relation to Retention
- No employees left after 6 years.
- Longevity alone does not guarantee higher satisfaction.
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/10cffc36-6cde-412c-a783-f3bbd9d935a2)

### Does Geography Play a Role in Satisfaction?
- Highest satisfaction: Germany and Portugal (above 90%).
- Lowest satisfaction: Spain (below 60%).
- Geography's impact is inconclusive due to various potential factors (departments, taxes, quality of life).
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/3b5ee827-1450-4e51-85af-2a5486e51013)

### Regression Analysis
- **Number of Projects undertaken:** Negative impact on satisfaction.
- **Monthly work hours:** Minimal positive impact on satisfaction.
- **No of Years spent in company:** Negative impact on satisfaction.
- **Salary bracket (low and medium):** Negative impact on satisfaction.
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/f6ae5020-679f-489b-ac55-11e4bfef914a)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/12fa8013-26d3-46fc-aff6-0ad10bef01e4)
![image](https://github.com/artsong4/Employee-Satisfaction-Analysis/assets/125407614/0cbb03d3-a5f2-4031-b62a-775e49fb0aa7)

## Next Steps
- **Monitoring the number of projects people are assigned**
- **Monitoring the overtime or hours people are working**
- **Focus on opportunities to develop employees**

## Skills Demonstrated
- Data Cleaning and Preprocessing
- Exploratory Data Analysis
- Statistical Analysis
- Data Visualization (ggplot2, plotly)
- R Programming

## Repository Structure
```plaintext
Employee-Satisfaction-Analysis/
├── data/
│   ├── Employement_data.xlsx
├── Employee_Satisfaction_Analysis.Rmd
├── README.md
├── LICENSE
