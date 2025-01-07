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
