# Loan Application Scoring & Data Cleaning with Python

## Project Overview

This project focuses on cleaning loan application data, enriching it with industry-based scores, and calculating an application score based on predefined business rules.

The goal is to transform raw application data into a clean, structured, and analyzable dataset, then evaluate applicants using a rule-based scoring model.

## Business Context

Financial institutions often evaluate loan applications using multiple applicant-related criteria.  
This project simulates a simplified scoring system that helps assess applicants and monitor trends in accepted applications over time.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Key Steps

1. Loaded and explored the application and industry datasets
2. Removed duplicate applicant records
3. Handled missing values based on business rules
4. Merged industry-level score data into the application dataset
5. Built a rule-based application scoring system
6. Filtered accepted applications
7. Analyzed weekly average scores of accepted applicants
8. Visualized applicant quality trends over time

## Scoring Logic

The application score was calculated based on the following rules:

- Age between 35 and 55: +20 points
- Weekday application: +20 points
- Married applicant: +20 points
- Applicant located in or around Kyiv: +10 points
- Industry score: 0 to 20 points
- External Rating 7 or higher: +20 points
- External Rating 2 or lower: -20 points
- Missing Amount or External Rating equal to 0: final score = 0

## Key Insights

- Duplicate records were removed to avoid biased analysis.
- Missing values were handled according to business logic instead of applying one generic method to all columns.
- Industry scores helped enrich the dataset and improve the scoring model.
- The acceptance rate was relatively high due to the simplified scoring rules used in this project.
- Weekly score trends showed fluctuations in applicant quality over time.

## Visualization

The project includes a line chart showing the weekly average score of accepted applications.

This helps monitor changes in applicant quality across different time periods.

## Files

- `loan_application_scoring_analysis.ipynb`
- `applications.csv`
- `industries.csv`

## Conclusion

This project demonstrates how raw application data can be cleaned, enriched, scored, and analyzed using Python.

It shows practical data analysis skills including data cleaning, merging datasets, rule-based scoring, aggregation, and visualization.
