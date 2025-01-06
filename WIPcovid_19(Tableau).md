# COVID-19 Data Analysis and Visualization Project

In this project, I showcase my ability to clean and visualize a real-world dataset using **Tableau**. The dataset used in this project is related to COVID-19 statistics, providing information about confirmed cases, recoveries, and deaths across different regions and dates. I followed a series of data cleaning steps to ensure the dataset was ready for analysis and visualization.

## Data Cleaning Process

### 1. Replacing NULL Values
I replaced any `NULL` values in the **Confirmed**, **Recovered**, and **Deaths** columns with `0` to prevent gaps in the data.

**SQL Query:**
```sql
UPDATE "Covid 19" SET "Confirmed" = 0 WHERE "Confirmed" IS NULL;
UPDATE "Covid 19" SET "Recovered" = 0 WHERE "Recovered" IS NULL;
UPDATE "Covid 19" SET "Deaths" = 0 WHERE "Deaths" IS NULL;
 ```

## 2. Checking for Negative Values

I ensured that there were no negative values in the **Confirmed**, **Recovered**, and **Deaths** columns, as negative values do not make sense in the context of COVID-19 data.

**SQL Query:**
```sql
SELECT *
FROM "Covid 19"
WHERE "Confirmed" < 0 OR "Recovered" < 0 OR "Deaths" < 0;
```
No negative values were found, so the data was clean in this regard.

## 3. Handling Duplicates

I checked for duplicates to ensure there were no redundant rows for any given date and region. This step was critical to maintaining the integrity of the data.

**SQL Query:**
```sql
SELECT "Date", "Country/Region", "Province/State", COUNT(*) 
FROM "Covid 19" 
GROUP BY "Date", "Country/Region", "Province/State"
HAVING COUNT(*) > 1;
```


## Visualizations and Insights

- **Time-Series Trends**: Analyzing the trends in **Confirmed**, **Recovered**, and **Deaths** over time.
- **Geographical Maps**: Interactive maps to visualize the spread of COVID-19 across different regions.
- **Bar/Column Charts**: Comparison of COVID-19 data across various countries and regions.
- **Filters**: Users can filter the data by specific countries or time periods for more detailed insights.

This project emphasizes my proficiency in transforming raw data into actionable insights and presenti

