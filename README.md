# Salifort Motors Employee Turnover Analysis

## Overview
The goal of this project was to create a machine learning model to predict employee turnover and identify the key feautes that drive turnover in order to increase employee rentention. The project uses fictional data from a company called Salifort Motors. A random forest model was used to predict which employees would leave and which would not. The model performed with a 95.2% AUC score and a 90.7% recall score. The model results combined with findings from EDA showed that satisfactiion levels, number of current projects, evaluation scores, and monthly hours worked were the best predictors for determining whether or not an employee would leave the company.

## Business Understanding
Salifort Motors is experiencing high employee turnover rate. The company wants to create a culture that supports the development and wellbeing of their employees. The high turnover rate also has a negative financial impact on the company. Leadership wants to identify the reasons that employees are leaving so that they can develop a solution.

## Data Understanding
The data is a sample of employees from Salifort Motors and compiled by their HR department. The data has exactly 149,999 rows and 10 columns. Each row contains data on one employee. The features are satisfaction level, last evaluation score, number of current projects, average monthly hours worked, tenure, number of work accidents, whether or not the employee has been promoted in the last 5 years, department, salary, and whether or not the employee has left. Several column names were renamed to correct typos and maintain a consistent naming convention. The bar plot below shows the amount of employees who stayed (83%) and employees who left (17%).

![barplot](https://github.com/J-David-Baxter/Employee-Turnover-Analysis/assets/57837488/c08dcb3d-a3f2-41c4-a1db-6f215a71c8ad)

## Modeling and Evaluation
Our random forest model consisted of 500 trees, each with a max depth of 6. It had an AUC score of 95.2%. It also had 98.1% precision, 90.7% recall, 94.3% F1, and 98.2% accuracy. The model performed well when predicting employees who leave, and was very good at predicting employees who stay. The below plot shows the feature importance for our model.

![features](https://github.com/J-David-Baxter/Employee-Turnover-Analysis/assets/57837488/a791a36a-b1d7-4961-a4e6-9851f77978ee)

The most important features were satisfaction level, evaluation score, number of projects, monthly hours worked, and tenure. 

## Conclusion
The model and EDA showed that employees leave due to being overworked. Certain steps can be taken by Salifort Motors to improve employee retention rate, such as capping the number of projects for each employee, reducing hours worked or rewarding employees who work lots of hours, discussing work expectations within each department, and making sure not to evaluate employees solely on hours worked. The model can help Salifort Motors improve their company culture and reduce the cost of recruiting, training, and upskilling their employees.
