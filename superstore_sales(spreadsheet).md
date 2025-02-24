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


![image](https://github.com/user-attachments/assets/13344b26-8a2e-4c39-a934-8549ffaa99de)


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


![image](https://github.com/user-attachments/assets/5ae40e2e-4cd5-4301-935d-73e4a5ad772d)



### Pivot Table: Total Sales by Region

This pivot table provides a breakdown of **Total Sales** across different **regions**. Analyzing sales by region allows businesses to understand regional performance and identify areas of strength or weakness in their sales strategy.

Here are the key insights from this analysis:

- **West** region has the highest sales, totaling **$3,425,334.18**, which is a significant portion of the total sales.
- **Ontario** follows closely with **$2,922,364.13** in sales, showing strong performance in this region.
- **Prairie** region contributes **$2,689,118.51** in sales, which is also a notable amount.
- **Atlantic** region accounts for **$1,919,898.24**, making it the fourth highest region by sales.
- **Quebec** and **Northwest Territories** have lower sales of **$1,432,930.96** and **$763,823.31**, respectively.
- **Yukon** and **Nunavut** show the lowest sales, with totals of **$929,822.69** and **$110,291.74**, respectively.

The **Grand Total** for all regions is **$14,193,583.76**, which represents the total sales across all regions.

This analysis reveals that the **West** and **Ontario** regions dominate in terms of sales, while regions like **Nunavut** and **Yukon** have considerably lower sales. This information can help businesses allocate resources, tailor marketing strategies, and focus on high-performing regions.

**Why it’s useful**:  
By analyzing **Total Sales by Region**, businesses can identify which regions are performing well and which may need further attention. This insight can guide regional sales strategies, marketing campaigns, and even expansion efforts in areas with lower sales.


![image](https://github.com/user-attachments/assets/6c9f8ef9-20ea-4065-ab5a-6dd764593503)


### Customer Segmentation Analysis

In this analysis, customers were segmented into four categories: **Consumer**, **Corporate**, **Home Office**, and **Small Business**. The total sales and profit for each segment were calculated to identify the most profitable customer groups.

### Key Insights:
- **Corporate** customers are the highest contributors to both **Total Sales** ($5.22M) and **Profit** ($599.7K), showing that larger business accounts are the primary revenue and profit drivers for the Superstore.
- The **Home Office** and **Consumer** segments contribute significant sales, with **Home Office** having a higher profit margin despite slightly lower sales.
- **Small Business** customers generate substantial sales, but the profit margins are relatively smaller compared to the other segments.

By analyzing these segments, businesses can tailor their marketing and sales strategies to target the most profitable customer groups.


![image](https://github.com/user-attachments/assets/a685c222-ab99-4d7b-8da3-bd0ada86b157)

### Monthly Sales and Profit Analysis

This analysis examines the **Total Sales** and **Profit** for each month across all years in the dataset. The data reveals trends in sales performance and profitability on a month-to-month basis.

### Key Insights:
- **Highest Sales:** The month with the highest total sales is **June** ($1.34M), followed by **March** ($1.27M). These months saw significant contributions from the Superstore's sales efforts.
- **Highest Profit:** **March** also saw the highest profit ($185.3K), showing strong profitability during this month, followed by **June** ($180.8K).
- **Lowest Performance:** The **December** month reported the lowest profit ($70.4K), though total sales were still strong at $1.14M.
- **Seasonal Trends:** The sales performance shows steady growth throughout the year, with a slight dip in **December**, possibly indicating seasonal fluctuations or year-end discounting.

This analysis can help identify patterns that businesses can leverage to optimize sales strategies across different times of the year.


![image](https://github.com/user-attachments/assets/5d7ee1f4-f8a5-4b1d-a190-e361aa24892c)
![image](https://github.com/user-attachments/assets/cd1c2e96-1b8c-42e0-85f2-c002b82d2d4d)

## Order Analysis

### Average Order Value

The **Average Order Value (AOV)** is calculated by dividing the total sales by the number of unique orders. To calculate the number of unique orders, I used the `COUNTUNIQUE` formula on the **Order ID** column, which gives the number of distinct orders. The formula for AOV is:

**Average Order Value (AOV) = Total Sales / Unique Orders**  
**AOV = 14,193,583.76 / 5,498 ≈ 2,578.67**

Thus, the **Average Order Value (AOV)** across all orders is approximately **$2,578.67**.

### Orders per Customer

To calculate the **Orders per Customer**, I again used the `COUNTUNIQUE` formula, but this time on the **Customer Name** column to determine the number of unique customers. Using the formula:

**Orders per Customer = Unique Orders / Unique Customers**  
**Orders per Customer = 5,498 / 797 ≈ 6.9**

This means, on average, each customer places approximately **6.9 orders**.

### Conclusion

By using the `COUNTUNIQUE` formula, I was able to efficiently calculate the number of unique **Order IDs** and **Customer Names**, which were crucial for the **Order Analysis**. These metrics provide valuable insights into customer purchasing behavior and order frequency, which can help inform business strategies such as targeted marketing and inventory management.



# Visualization Analysis

![Sales_profit VS product category](https://github.com/user-attachments/assets/574f9f49-4da2-426b-81ce-9d63a55daf2b)


**Key Observations:**

*   **Technology Leads in Both Sales and Profit:** The Technology category clearly demonstrates the highest performance in both sales and profit. This suggests a strong market demand and effective pricing strategies for technology products.
*   **Furniture Generates High Sales but Low Profit:** While the Furniture category has substantial sales, comparable to Technology, its profit is significantly lower. This indicates potential issues with profitability within this category, possibly due to higher costs, lower margins, or higher return rates.
*   **Office Supplies Shows Moderate Performance:** The Office Supplies category maintains a moderate level of both sales and profit, positioning itself between Technology and Furniture in terms of overall performance.

**Comparison to Pivot Table Analysis:**

This visualization complements the previous pivot table analysis by providing a clear visual representation of the data. While the pivot tables presented the numerical values, this chart facilitates a quicker and more intuitive understanding of the relative performance of each category. Specifically:

*   The chart visually emphasizes the stark contrast in profitability between Furniture and the other two categories, a key insight also highlighted in the profit pivot table.
*   The chart reinforces the pivot table's finding that Technology is the top performer in both sales and profit.
*   The visualization makes it immediately clear that while Furniture has high sales, it has a significantly lower profit than Office Supplies, a point that required more careful examination in the pivot tables.

**Insights:**

*   The significant difference between sales and profit in the Furniture category warrants further investigation. Potential contributing factors include:
    *   **High Shipping Costs:** Furniture is often bulky and expensive to ship, impacting profit margins.
    *   **Competitive Pricing:** The furniture market may be highly competitive, forcing lower prices and reducing profit margins.
    *   **Discounts and Promotions:** Frequent promotional activities could be cutting into profits.
*   The high profitability of the Technology category suggests effective cost management, strong pricing strategies, or a favorable product mix.

**Recommendations:**

*   **Investigate Furniture Profitability:** A detailed cost analysis of the Furniture category is recommended to identify areas for improvement. This should include analysis of shipping costs, pricing strategies, and product mix.
*   **Maintain Focus on Technology:** Given its strong performance, continued investment and focus on the Technology category are advisable.
*   **Explore Opportunities for Office Supplies:** While performing adequately, opportunities to optimize costs or increase sales in the Office Supplies category should be explored.

**Conclusion:**

This visualization effectively communicates the sales and profit performance across product categories, confirming and visually reinforcing insights derived from the pivot table analysis. The stark contrast in profitability within the Furniture category highlights a key area for further investigation and potential improvement. The combined use of pivot tables and visualizations provides a more comprehensive understanding of the data, leading to more informed business decisions.



![image](https://github.com/user-attachments/assets/e8bf3bf5-f43d-431d-bc17-2b3a1265de47)

## Regional Sales Overview Visualization Analysis

This analysis visualizes the distribution of total sales across different regions within the Superstore dataset. The visualization used is a vertical bar chart, which effectively compares sales performance across each region. My main goal was to use a pie chart however it ended up looking overly cluttered, thus the use of this effective and easy to understand vertical bar chart.


**Key Observations:**

*   **West Leads in Sales:** The West region clearly generates the highest sales volume, significantly outpacing other regions.
*   **Ontario and Prairie Contribute Substantially:** Ontario and the Prairie region also demonstrate strong sales performance, though not at the same level as the West.
*   **Nunavut and Yukon Show Lowest Sales:** Nunavut and Yukon have the lowest sales figures, indicating a much smaller market presence or lower sales activity in these regions.
*   **Clear Ranking of Regions:** The bar chart provides an immediate and clear ranking of the regions from highest to lowest sales, facilitating easy comparison.

**Comparison to Pivot Table Analysis:**

This visualization complements the previous pivot table analysis by providing a visual representation of the numerical data. While the pivot table presented precise sales figures for each region, the bar chart allows for a more intuitive and rapid understanding of the relative sales performance across regions. Specifically:

*   The chart visually reinforces the pivot table's finding that the West region is the top performer.
*   The chart makes it immediately apparent that Nunavut and Yukon have significantly lower sales compared to all other regions, a fact that requires more careful examination of the numerical data in the pivot table.
*   The visualization makes it easier to quickly grasp the overall sales hierarchy among the regions.

**Insights:**

*   The dominance of the West region suggests a strong market presence and effective sales strategies in that area. Further investigation into the factors contributing to this success could provide valuable insights for other regions.
*   The low sales in Nunavut and Yukon may be due to factors such as smaller population sizes, limited market demand, or logistical challenges. Further research is needed to understand the specific dynamics of these regions.
*   The mid-range performance of regions like Atlantic and Quebec suggests opportunities for growth. Targeted sales and marketing efforts could potentially increase sales in these areas.

**Recommendations:**

*   **Investigate West Region Success:** Analyze the sales strategies, marketing campaigns, and customer demographics in the West region to understand the factors driving its strong performance.
*   **Assess Challenges in Nunavut and Yukon:** Conduct market research in Nunavut and Yukon to identify the specific challenges hindering sales growth. This could include analyzing market demand, logistical constraints, and customer needs.
*   **Develop Targeted Strategies for Mid-Performing Regions:** Develop tailored sales and marketing strategies for regions like Atlantic and Quebec to capitalize on potential growth opportunities.

**Conclusion:**

This bar chart effectively visualizes the regional sales distribution, confirming and visually reinforcing the insights derived from the pivot table analysis. The visualization provides a clear and intuitive understanding of the relative sales performance of each region, highlighting key areas of strength and weakness. The combined use of pivot tables and visualizations provides a more comprehensive understanding of the data, leading to more informed business decisions and strategic planning.





# Spreadsheet Project Conclusion

This project has demonstrated my proficiency in using spreadsheets like Google Sheets and Excel for data analysis and visualization. By leveraging the Superstore Sales dataset, I have successfully explored various aspects of the sales data, including:

*   **Data cleaning:** Ensuring the data is free from errors and inconsistencies.
*   **Data analysis:** Identifying key trends, patterns, and insights in the sales data.
*   **Visualization:** Creating informative and visually appealing charts and graphs to communicate the analysis effectively.
*   **Advanced spreadsheet functions:** Utilizing functions like `VLOOKUP`, `SUMIFS`, conditional formatting, and data validation to enhance the efficiency and insightfulness of the analysis.

The analysis revealed valuable insights into the Superstore's sales performance across various product categories, customer segments, regions, and time periods. Here's a summary of the key findings:

*   **Technology** emerged as the leading product category in terms of both total sales and profitability.
*   **Furniture** had high sales, but its profit margins were significantly lower, requiring further investigation.
*   **The West region** dominated in sales, followed by Ontario and the Prairie region. Sales in Nunavut and Yukon were considerably lower.
*   **Corporate customers** contributed the most to both sales and profit, highlighting the importance of this segment.
*   **Monthly sales and profits** revealed seasonal trends, with June being the highest month for sales and March showing the highest profit.

**Additional Considerations:**

*   While the pivot tables provided detailed numerical analysis, the visualizations offered a more intuitive and visually compelling view of the data.
*   The use of advanced spreadsheet functions streamlined the analysis process and facilitated more complex calculations.

This project has showcased my ability to translate raw data into actionable insights that can inform strategic decision-making within a business context. By leveraging these skills, I can contribute to optimizing sales strategies, improving profitability, and identifying areas for future growth.

**Future Exploration:**

There are several ways to further expand on this project:

*   **Drill down into specific product subcategories:** Analyze the performance of individual subcategories within each category to identify potential areas for improvement.
*   **Customer lifetime value analysis:** Calculate the customer lifetime value to understand the long-term revenue potential of different customer segments.
*   **Predictive modeling:** Utilize machine learning techniques to predict future sales trends and customer behavior.

By continuing to explore and analyze the Superstore Sales dataset, I can gain even deeper insights that can further enhance the Superstore's overall sales performance.
