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


