## Spreadsheet Project - Superstore Sales Data Analysis

Welcome to my Superstore Sales Data Analysis project! In this project, I will showcase my expertise in using **Google Sheets** and **Excel** for data analysis and visualization. The dataset I am working with is the **Superstore Sales dataset**, which contains detailed sales transactions, customer information, and product data from a retail store.

### Project Goals:

- **Data Cleaning**: Preparing and cleaning the dataset to ensure accurate analysis and ensuring the data is free from biases that could impact the results.
- **Data Analysis**: Identifying key trends, patterns, and insights in the sales data.
- **Visualization**: Creating dynamic and insightful visualizations, including charts, graphs, and pivot tables, to highlight sales performance, product categories, and customer behaviors.
- **Advanced Spreadsheet Functions**: Demonstrating my proficiency with functions like `VLOOKUP`, `SUMIFS`, conditional formatting, and data validation to make the analysis more efficient and insightful.

As I continue to work on this project, I will be updating my progress regularly and showcasing new techniques and analyses that I apply to this dataset.

![image](https://github.com/user-attachments/assets/113995fe-3e21-4c7f-9067-519dc465a341)

This screenshot provides a snapshot of the data I’m working with, though some columns (such as Product Subcategory, Product Name, Product Container, Product Base Margin, and Ship Date) are not visible here. These columns will be explored in more detail in later stages of the analysis.

Before diving into the analysis, I applied a filter to ensure the data was clean and consistent. This involved removing duplicates, ensuring case sensitivity, and validating the integrity of the dataset. With the data now properly cleaned, we can proceed with the analysis.



![image](https://github.com/user-attachments/assets/0b75156a-29c1-4e0e-a738-672b0ac7942f)

### Pivot Table: Total Sales by Product Category

In this pivot table, I’ve grouped the data by **Product Category** and calculated the **SUM of Total Sales** for each category. This analysis provides a clear overview of how sales are distributed across different product categories.

Here are the key insights from the pivot table:

- **Technology** had the highest total sales, amounting to **$5,693,015.06**.
- **Furniture** generated **$4,933,871.76** in total sales.
- **Office Supplies** contributed **$3,566,696.94** to the total sales.

The **Grand Total** sales amount to **$14,193,583.76**, which represents the overall revenue generated from all product categories in the dataset.

This pivot table helps us understand the performance of each product category, identifying the top-performing categories and the areas where the business has seen the most sales.



![image](https://github.com/user-attachments/assets/6dce94c1-2646-4f2e-b255-ba0d86c4404c)


### Pivot Table: Total Sales by Product Subcategory

In this pivot table, I’ve grouped the data by **Product Subcategory** and calculated the **SUM of Total Sales** for each subcategory. This allows for a more detailed breakdown of sales within the broader product categories.

Here are the key insights from the pivot table:

- **Office Machines** had the highest total sales, amounting to **$2,063,925.38**.
- **Tables** followed closely behind, generating **$1,802,418.27** in total sales.
- **Chairs & Chairmats** contributed **$1,677,969.10** to the total sales, making it one of the top-performing subcategories.

On the lower end, **Rubber Bands** had the smallest sales, with only **$14,268.83** in total sales.

The **Grand Total** sales amount to **$14,193,583.76**, which represents the overall revenue generated from all product subcategories.

This pivot table provides a granular view of how sales are distributed among individual product subcategories, helping to pinpoint high-performing products and identify areas where sales may be lower.

**Why it’s useful**:  
By breaking down sales at the subcategory level, this analysis helps businesses understand which specific products are driving revenue and which may need further attention in terms of marketing or inventory. It also helps in forecasting demand for individual products.






![image](https://github.com/user-attachments/assets/871770c6-bafa-4aec-87be-a37bd7e05126)



### Pivot Table: Total Profit by Product Category

In this pivot table, I’ve grouped the data by **Product Category** and calculated the **SUM of Profit** for each category. This analysis helps in understanding the profitability of each product category, even when total sales might not tell the full story.

Here are the key insights from the pivot table:

- **Technology** had the highest total profit, amounting to **$886,313.52**.
- **Office Supplies** generated **$518,021.46** in profit, despite having lower total sales than **Furniture**.
- **Furniture** had a total profit of **$117,432.99**, which is significantly lower than **Office Supplies** and **Technology**, even though its total sales were higher.

The **Grand Total** profit amounts to **$1,521,767.96**, which represents the overall profit generated from all product categories in the dataset.

This pivot table highlights the importance of not just focusing on sales but also analyzing the **profitability** of different product categories. It demonstrates that higher sales do not always correlate with higher profits, as profit margins and cost structures can vary across categories.

**Why it’s useful**:  
This analysis helps businesses identify which product categories are more profitable and which ones may be consuming more resources, despite having high sales. By focusing on profitability, companies can make more informed decisions about pricing, marketing, and inventory strategies.


![image](https://github.com/user-attachments/assets/23be4121-0bc9-4ff5-bdf8-0d74f0a5e3aa)

### Pivot Table: Total Sales by Product Category and Discount

In this pivot table, I’ve broken down **Total Sales** by **Product Category** and **Discount Percentage**. The table provides insight into how sales vary across different discount levels for each category, helping us understand the impact of discounts on total sales.

Here are the key insights:

- **Furniture** shows a consistent pattern, with the highest sales observed at a **0% discount** (**$463,595.36**), and sales decrease as the discount percentage increases, with a slight increase at higher discounts (e.g., **5%** and **6%**).
- **Office Supplies** also shows high sales at the **0% discount** (**$318,660.00**) but has noticeable fluctuations at higher discount levels. Interestingly, **3%** and **2%** discounts seem to yield the best sales results for this category.
- **Technology** demonstrates the highest sales overall, with the **0% discount** leading to **$711,492.85** in total sales. Similar to Furniture, higher discounts seem to decrease sales, but there are some anomalies, such as higher sales at **6%** and **5%** discounts.

The **Grand Total** for all product categories is **$14,193,583.76**, showing the overall sales across all discount levels.

This analysis reveals how **discounts impact sales** across different categories. It’s essential to note that while **0% discount** typically results in the highest sales, offering a moderate discount (e.g., **3%-5%**) can sometimes lead to increased sales in certain categories, such as **Technology** and **Furniture**.

**Why it’s useful**:  
This table provides valuable insights into the pricing and discount strategies for each product category. It helps businesses understand whether offering discounts boosts sales and identifies the optimal discount percentage for maximizing revenue. By analyzing this data, companies can refine their discount strategies to increase sales and profitability.


![image](https://github.com/user-attachments/assets/0f66ff78-15c3-45d3-b593-3b0623078655)

### Pivot Table: Total Sales by Year

This pivot table summarizes the **Total Sales** for each year in the dataset. Analyzing sales by year helps identify trends and patterns over time, allowing businesses to assess performance and make data-driven decisions.

Here are the key insights from this analysis:

- **2009** had the highest sales, totaling **$4,013,659.73**.
- **2010** followed with **$3,379,388.68**, showing a decrease in sales compared to the previous year.
- **2011** saw a further decline in sales, amounting to **$3,262,760.29**.
- **2012** experienced a slight recovery, with **$3,537,775.06** in total sales.

The **Grand Total** for all years is **$14,193,583.76**, which represents the overall sales across all four years.

This analysis highlights a downward trend in sales from 2009 to 2011, followed by a modest recovery in 2012. This trend could be useful for identifying seasonal effects, market conditions, or external factors that influenced sales during this period.

**Why it’s useful**:  
By analyzing **Total Sales by Year**, businesses can track their sales performance and identify periods of growth or decline. This insight is valuable for making strategic decisions regarding marketing, inventory, and future planning.
