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
docker run -d -p 3000:3000 --name metabase -v $(pwd)/metabase.db:/metabase.db metabase/metabase
```
After running this, you can access Metabase via http://localhost:3000 to create the dashboard and configure the necessary data visualizations.

## Business Dashboard

Attrition Rate by Gender and Marital Status:
* Employees with a single marital status show the highest attrition rate, both for men and women.
* Attrition rates tend to be lower among married and divorced employees.
* Married employees have a slightly higher attrition rate compared to divorced employees, but it is still lower than that of single employees.

Overall, attrition rates between men and women in each marital status category do not differ significantly.

## Conclusion

Jelaskan konklusi dari proyek yang dikerjakan.

### Rekomendasi Action Items (Optional)

Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.

- action item 1
- action item 2
