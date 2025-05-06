# Final Project: Solving Edutech Company Problems

## Business Understanding

Jaya Jaya Maju is a multinational company that has been operating since 2000. With more than 1,000 employees across the country, the company has grown to become one of the larger businesses in its industry.
However, the company still faces some serious challenges in managing its employees.
One of the main problems is the high attrition rate, which is now over 10%. This high turnover could affect daily operations and overall performance. Because of this, the HR department manager has asked for help to find out the reasons behind the high attrition rate.

### Business Problems

* High Attrition Rate: Currently, more than 10% of employees are leaving the company. This shows there may be underlying issues that need to be explored further, such as company culture, job satisfaction, or other factors.

* Difficulty Identifying Causes of Attrition: The HR manager is having trouble understanding the main reasons why employees decide to leave. Because of this, it's hard to take the right steps to fix the problem.

* Limited Employee Performance Monitoring: The HR department needs a better system to track and analyze employee data in real-time, so they can spot issues earlier and make better decisions based on the data.

### Project Scope

This project aims to:
* Analyze the dataset provided by the company to identify the factors that influence employee attrition.
* Create a business dashboard that the HR department can use to monitor various factors contributing to the high attrition rate.
* Provide data-based recommendations to the HR manager on steps that can be taken to reduce the attrition rate.

### Persiapan

Data source: https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee

Setup environment:
Before starting the project, make sure you have a development environment ready to use, such as:
Python Environment with libraries like Pandas, Numpy, Matplotlib, Scikit-learn, etc.

Metabase for creating the dashboard.

To set up Metabase locally using Docker, you can use the following command:

```
docker run -p 3000:3000 --name metabase metabase/metabase
```
After running this, you can access Metabase via http://localhost:3000 to create the dashboard and configure the necessary data visualizations.

## Business Dashboard

### Attrition Rate by Gender and Marital Status:
* Employees with a single marital status show the highest attrition rate, both for men and women.
* Attrition rates tend to be lower among married and divorced employees.
* Married employees have a slightly higher attrition rate compared to divorced employees, but it is still lower than that of single employees.
* Overall, attrition rates between men and women in each marital status category do not differ significantly.

### Attrition Rate by Gender and Age:
* Employees under 25 years old have the highest attrition rate compared to other age groups, especially among women.
* Attrition rates tend to decrease as employees age.
* The age group of 35-44 shows the lowest attrition rate for men, while for women, it is in the 45-54 age group.
* In the 25-34 age group, the attrition rate is relatively similar between men and women.

### Attrition Rate by Department and Monthly Income:
* The Sales department has the highest attrition rate across most income groups.
* The Research & Development department shows the lowest attrition rate.
* In the Human Resources department, attrition is higher in the middle-income group (7-9k).
* Overall, there is a varied pattern of attrition across different income levels and departments, but the Sales department consistently has a higher attrition rate.

### Attrition Rate by Overtime and Environment Satisfaction:
* Employees who work overtime have a significantly higher attrition rate compared to those who do not.
* The lower the job environment satisfaction, the higher the attrition rate. This difference is especially significant among employees who work overtime.

### Attrition Rate by Overtime and Work-Life Balance:
* Similar to job environment satisfaction, employees who work overtime have a significantly higher attrition rate, regardless of their work-life balance.
* The lower the work-life balance, the higher the attrition rate. However, attrition rates are not very different across the three work-life balance categories (Good, Excellent, and Outstanding).

### Attrition Rate by Work-Life Balance and Environment Satisfaction:
* The combination of low Environment Satisfaction and low Work-Life Balance results in the highest attrition rate.
* When Environment Satisfaction is low, attrition remains high even if Work-Life Balance is rated as excellent or outstanding. This suggests that an unsatisfactory work environment is a major factor driving employee turnover.
* Improving Work-Life Balance tends to reduce attrition, especially when Environment Satisfaction is also high or very high.
* The lowest attrition rate occurs when employees have excellent Work-Life Balance and very high Environment Satisfaction.

### Attrition Rate by Performance Rating and Environment Satisfaction:
* Employees with an excellent performance rating have a high attrition rate at several levels of Environment Satisfaction.
* Low Environment Satisfaction increases attrition, particularly among employees with an outstanding performance rating.
* Employees with an outstanding performance rating have a low attrition rate at several levels of Environment Satisfaction, although attrition slightly increases when Environment Satisfaction is at a low level. This may suggest that high-performing employees have more career options outside the company.

### Attrition Rate by Performance Rating and Percent Salary Hike:
* Attrition tends to be lower among employees who receive a moderate Percent Salary Hike.
* Employees with an outstanding performance rating and a high Percent Salary Hike have the highest attrition rate.
* Higher salary increases seem to help retain employees with good performance ratings (Outstanding), although attrition still increases in both the lowest and highest salary hike groups.

### Attrition Rate by Job Level and Years at Company:
* Employees with less than 10 years at the company, especially those at Job Level 1, have a high attrition rate. This might indicate problems with onboarding, role expectations, or integration of new employees.
* Attrition tends to decrease as employees stay longer, especially after 10-19 years.
* There is a rise in attrition for employees with 30-39 years at the company, across all job levels. This could be because employees are nearing retirement or looking for a career change after many years.
* Employees with 40+ years at the company have a very high attrition rate, likely due to approaching retirement.

### Attrition Rate by Job Level and Years in Current Role:
* The highest attrition rate is seen among employees at Job Level 1 with less than 5 years in their current role. This might indicate that employees feel mismatched with their role or lack support in their new position.
* There is an increase in attrition among employees with 14-17 years in their current role, almost across all job levels. This may suggest burnout or a lack of career development opportunities in their role.
* Employees with very long tenures (18+ years) in their current role show a very low attrition rate.

### Attrition Rate by Years at Company and Years in Current Role:
* The highest attrition rate is seen in employees who have been with the company for 30-39 years, across almost all job roles, except for those with 18+ years in their current role. This may mean they feel unhappy in their role or don’t have enough support.
* Employees who have been in their current role for 18+ years, regardless of how long they’ve been at the company, show a very low attrition rate.

## Conclusion
* Age and Marital Status: Younger employees and those who are single tend to have higher attrition rates. Employees in the Sales department also show higher turnover.
* Overtime and Job Satisfaction: Employees who work overtime and are dissatisfied with their work environment or work-life balance are more likely to leave the company.
* Performance and Salary: High-performing employees with high salary hikes have a higher attrition rate. However, moderate salary increases help keep employees with good performance.
* Job Level and Years at the Company: Employees with less experience or at lower job levels (Job Level 1) show higher attrition, especially those who’ve been in the company for less than 10 years. Attrition decreases as employees stay longer, especially after 10-19 years.
* Work Role Experience: Employees who are new to their role or have been in the same role for many years tend to stay longer. However, employees who have been in the same role for 14-17 years often experience burnout and may leave.

### Recommendation Action Items
* Adjust Salaries: Review employee salaries and make sure they match industry standards and employee expectations to improve satisfaction and reduce attrition.
* Improve Employee Experience: Improve training programs and support for new employees, and create a more inclusive work environment that supports their well-being.
* Career Flexibility: Offer more career development opportunities, like internal promotions and job rotation programs, to keep employees with the right skills.
* Strengthen Company Culture: Regularly conduct employee satisfaction surveys and address any issues so employees feel valued and connected to the company.
