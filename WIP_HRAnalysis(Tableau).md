# HR Analytics Tableau Project

This project visualizes HR data to provide insights into employee trends, attrition, satisfaction, and more. Using Tableau, I created various interactive visualizations to help HR managers and decision-makers better understand their workforce. The project uses a dataset with multiple attributes such as employee age, salary, performance, and work-life balance, enabling a deeper analysis of employee behavior.

## Data Cleaning Process

Before creating the visualizations, I performed necessary data cleaning in SQL to ensure the dataset was accurate and ready for analysis. Below are the key steps I took to clean the data:

### 1. Handling NULL Values:
   - I checked for missing values (NULLs) across the dataset and replaced them with appropriate values. For example, I replaced NULLs in the "Monthly Income" column with the average income.
   
   **Query:**
   ```sql
   UPDATE "HR_Data" 
   SET "Monthly Income" = (SELECT AVG("Monthly Income") FROM "HR_Data") 
   WHERE "Monthly Income" IS NULL;
```

 ### 2. Checking for Negative Values:
   - I ensured there were no negative values in the dataset for columns where negative values were not meaningful, such as "Daily Rate," "Hourly Rate," and "Age."

   **Query:**
   ```sql
   SELECT * FROM "HR_Data" 
   WHERE "Daily Rate" < 0 OR "Hourly Rate" < 0 OR "Age" < 0;
  ```

There were no negative values found, so the dataset was clean in this regard.

### 3. Handling Duplicates:
   - I checked for duplicate records to ensure each employee had a unique entry and there were no redundant data points.

   **Query:**
   ```sql
   SELECT "Emp ID", COUNT(*) 
   FROM "HR_Data" 
   GROUP BY "Emp ID" 
   HAVING COUNT(*) > 1;
```

There were no duplicates so we can proceed

### 4. Standardizing Categorical Data:
   - Columns like "Education" and "Job Level" were standardized for consistency, converting all values into a uniform format to ensure uniformity across the dataset.

   **Query:**
   ```sql
   UPDATE "HR_Data"
   SET "Education" = 'Bachelor' 
   WHERE "Education" IN ('Bachelors', 'Bach');
 ```


5. Handling Outliers:

    I checked for any outliers in numeric columns such as "Years at Company" and "Monthly Income" and handled them by replacing extreme values with realistic thresholds.

Query:

```sql
UPDATE "HR_Data"
SET "Years at Company" = 20 
WHERE "Years at Company" > 40;
```

## Visualizations

With the cleaned data, I created several key visualizations in Tableau to explore different aspects of the dataset:

- **Gender Distribution:** A bar chart showing the count of male and female employees.
- **Attrition Analysis:** A pie chart showing the distribution of employees who have left the company vs those who have stayed.
- **Satisfaction vs. Job Role:** A heatmap to explore how job satisfaction correlates with different job roles.
- **Income vs. Education:** A scatter plot showing the relationship between monthly income and education level.

This project demonstrates my ability to clean, transform, and visualize complex HR datasets using Tableau, providing insights that can drive decisions in employee retention, satisfaction, and performance.




![image](https://github.com/user-attachments/assets/9da59c1d-f565-49ee-b54e-06147dcfad36)

## Gender Distribution of Employees

This bar chart visually represents the gender distribution of employees within the dataset. The y-axis displays the count of employees, while the x-axis categorizes them into 'Female' and 'Male'. 

**Key Insights:**

* The chart reveals a significant gender imbalance, with a higher proportion of male employees (889) compared to female employees (591).
* This visualization provides a clear and concise overview of the gender composition of the workforce.



![image](https://github.com/user-attachments/assets/8f9dcca8-a463-4372-b277-81e53d44dcbe)


## Analysis of Attrition Rate by Employee Count

This pie chart visualizes the attrition rate within the organization, highlighting the proportion of employees who have left (Yes) versus those who remain (No). The data reveals that a significant majority of employees, represented by the larger green slice, have not left the organization. However, the red slice indicates that a notable number of employees have experienced attrition. 

**Key Insights:**

* **Attrition Rate:** The pie chart provides a clear visual representation of the overall attrition rate within the organization. 
* **Employee Count Distribution:** The relative sizes of the slices show the distribution of employees between those who have left and those who remain.
* **Focus Area:** The larger red slice emphasizes the need for further analysis and potential interventions to address the factors contributing to employee attrition. 

**Further Analysis:**

To gain deeper insights into the drivers of attrition, further analysis could be conducted. This might involve:

* **Segmenting the data:** Examining attrition rates across different departments, job roles, tenure levels, or other relevant dimensions.
* **Identifying risk factors:** Analyzing data to identify factors associated with higher attrition rates, such as employee engagement scores, compensation levels, or performance reviews.
* **Trend analysis:** Tracking attrition rates over time to identify any trends or patterns. 

By conducting further analysis and taking appropriate actions, the organization can strive to improve employee retention and reduce the impact of attrition on its overall performance.




![image](https://github.com/user-attachments/assets/9a33058d-59b0-474a-b391-7935f36af3c5)


## Analysis of Average Monthly Income by Education Level and Field of Study

This table visualizes the average monthly income across different education levels (1-5) and fields of study. The color gradient indicates the level of income, with darker shades representing higher average incomes.

**Key Observations:**

* **Impact of Education:** In general, higher education levels tend to be associated with higher average monthly incomes. This is evident across most fields of study, with some exceptions.

* **Field of Study Variation:** The average monthly income varies significantly across different fields of study, even within the same education level. For instance, at the highest education level (5), Life Sciences and Medical fields show notably higher average incomes compared to other fields.

* **Specific Observations:** 
    - **Education Level 4:** In this level, Human Resources stands out with a significantly higher average income compared to other fields.
    - **Education Level 5:** Life Sciences and Medical fields demonstrate the highest average incomes, while Human Resources shows a lower average income.

**Possible Interpretations:**

* **Field-Specific Demand:** The variation in income across fields likely reflects differences in market demand, skill requirements, and career opportunities within each field.
* **Education Premium:** The positive correlation between education level and income suggests that higher education generally leads to better earning potential.
* **Field-Specific Factors:** Factors such as experience, industry trends, and individual skills can further influence income within each field and education level.

**Further Analysis:**

To gain deeper insights, further analysis could be conducted:

* **Segmenting the data:** Examining income variations within each field by factors such as experience, gender, or location.
* **Trend analysis:** Tracking income trends over time to identify changes in income patterns across different fields and education levels.
* **Identifying factors:** Analyzing data to identify specific factors that contribute to higher or lower incomes within each field.

By analyzing and understanding these trends, individuals can make informed career decisions and organizations can gain insights into the labor market and compensation strategies.


![image](https://github.com/user-attachments/assets/c80c3f28-ec49-49b2-9d01-9caed6072f40)


## Job Satisfaction Across Job Roles

This bar chart visualizes the average job satisfaction scores across different job roles within an organization. The color gradient of each bar represents the employee count within each role, with darker shades indicating a higher number of employees.

**Key Observations:**

* **Overall Job Satisfaction:** The chart shows a moderate level of job satisfaction across most roles, with scores generally ranging between 2.5 and 2.8 on a presumed scale (likely 1-5).

* **Highest Satisfaction:** Healthcare Representatives and Research Scientists appear to have the highest average job satisfaction scores.

* **Lowest Satisfaction:** Human Resources personnel seem to have the lowest average job satisfaction score.

* **Employee Count Impact:** 
    - Roles with higher employee counts, such as **Sales Executive** and **Research Scientists**, tend to have a darker color gradient, indicating a larger number of employees compared to roles like **Human Resources**.
    - It's important to note that higher employee count does not necessarily correlate with lower satisfaction in this case. 

**Possible Interpretations:**

* **Role-Specific Factors:** The variations in job satisfaction across roles may be influenced by factors such as job responsibilities, work environment, compensation, opportunities for growth, and work-life balance.

* **Employee Engagement:** Higher levels of job satisfaction may be associated with increased employee engagement, productivity, and retention.

* **Focus Areas:** The lower satisfaction scores for certain roles (e.g., Human Resources) suggest areas for improvement in terms of employee experience and engagement.

**Further Analysis:**

To gain deeper insights into the drivers of job satisfaction, further analysis could be conducted:

* **Segmenting the data:** Examining job satisfaction scores within each role by factors such as tenure, department, or location.
* **Identifying root causes:** Conducting employee surveys or focus groups to identify specific reasons for lower satisfaction in certain roles.
* **Implementing interventions:** Developing and implementing strategies to improve job satisfaction, such as targeted training programs, performance recognition initiatives, or improvements in work-life balance policies.

By analyzing and addressing the factors influencing job satisfaction, the organization can create a more positive and fulfilling work environment for its employees.



![image](https://github.com/user-attachments/assets/da20e028-e5d2-4baa-b48b-dea4ae3780ac)

## Work-Life Balance vs. Job Involvement: Employee Distribution

**Analysis:**

This area chart illustrates the distribution of employees across different levels of job involvement and work-life balance. The x-axis represents job involvement, ranging from 1 to 4, while the y-axis indicates the employee count. The color gradient represents the work-life balance score, with 1 being the lowest and 4 being the highest.

**Key Observations:**

1. **Peak at Job Involvement 3:** The chart reveals a significant concentration of employees at job involvement level 3, regardless of their work-life balance score. This suggests that a considerable portion of the workforce is highly engaged in their work.

2. **Work-Life Balance Impact:**
    - **Lower Work-Life Balance (1, 2):** Employees with lower work-life balance scores are more likely to be concentrated at higher job involvement levels (3 and 4). This could indicate that individuals with lower work-life balance may be more dedicated to their work, potentially at the expense of their personal life.
    - **Higher Work-Life Balance (3, 4):** As work-life balance improves, the distribution of employees across job involvement levels becomes more balanced. This suggests that employees with a better work-life balance may have more flexibility in their level of engagement.

3. **Employee Count Variation:** The chart also shows a significant variation in employee count across different combinations of job involvement and work-life balance. For instance, there is a considerably higher number of employees with high job involvement and low work-life balance compared to those with low job involvement and high work-life balance.

**Possible Interpretations:**

* The concentration of employees at high job involvement levels might indicate a positive work environment that fosters engagement. However, the association with lower work-life balance scores raises concerns about potential burnout and employee well-being.
* The findings suggest that improving work-life balance could potentially lead to a more balanced distribution of employees across different levels of job involvement, fostering a healthier and more sustainable work environment.

**Further Analysis:**

* Investigating the factors contributing to low work-life balance among highly engaged employees could provide valuable insights for improving employee well-being and retention.
* Analyzing the impact of work-life balance interventions on employee engagement and productivity could help organizations optimize their work environment.

**Note:**

* This analysis is based on the visual representation of the data. A deeper understanding would require access to the raw data and further statistical analysis.

