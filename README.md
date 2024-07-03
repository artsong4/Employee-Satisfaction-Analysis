# Employee Satisfaction Analysis

## Project Overview
This repository contains the final project from the IST 687 Introduction to Data Science course. This project analyzes employee satisfaction data to provide actionable insights for improving satisfaction and retention in a European company.

## Team Members
- Tibaria Al Nouri
- Katherine Martinez
- Stephen Price
- Yesul Song

## Introduction
In the rapidly evolving landscape of today's corporate world, employee satisfaction stands as a linchpin to organizational success. A satisfied workforce not only bolsters productivity but also strengthens brand reputation, ultimately impacting the bottom line. Our independent data science team was commissioned by the HR department of a notable European company to unravel the intricacies behind their troublingly low employee satisfaction rates. This report chronicles our approach, findings, and the invaluable insights gleaned, which we hope will pave the way for enhanced employee satisfaction and, by extension, company success.

## Business Questions
1. Is satisfaction linked to departments?
2. Is there a geographic component to job satisfaction?
3. Did promotion affect retention?
4. Did job injury affect retention?
5. What was the duration of employment before leaving?

## Methodology
1. **Defining the Question:** Framing analysis with precise questions to provide direction.
2. **Data Collection:** Procuring the dataset from the HR department.
3. **Data Cleansing:** Formatting data types for consistency and addressing missing or null values.
4. **Data Analysis:** Grouping data for visualizations, geographical plotting, and executing regression analysis to identify potential correlations.
5. **Sharing Results:** Compiling findings into a comprehensive report.

## Analysis

### Reasons for Leaving
- The primary reasons cited for departing were remuneration, better opportunities at competing firms, lack of encouragement, and issues with immediate supervisors.

### Attrition by Department
- Departments with the highest attrition rates were Sales, Technical Support, and IT.

### Satisfaction by Salary Bracket
- Low and medium salary brackets showed significant impact on satisfaction.

### Regression Analysis
- **Number of Projects undertaken:** Negative impact on satisfaction.
- **Monthly work hours:** Minimal positive impact on satisfaction.
- **No of Years spent in company:** Negative impact on satisfaction.
- **Salary bracket (low and medium):** Negative impact on satisfaction.

## Results and Next Steps
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
