# Olist Data Analysis Project

## Project Background

Olist founded in 2015 is the largest department store in Brazilian marketplaces, it connects small business and allows sellers offer their products while Olist is in charge of logistics.
This project analyzes sales from 2016 - 2018. The company has significant amount of records (100k) in orders, customers, sellers, products, locations and payments details. This project throughly analyzes and sythezises the data in order to obtain meaningful insights that will lead to improve performance in sales and different areas of the company.

**Insights and recommendations focus on the following key analytical areas:**

- **Category 1 Historical Sales Performance:**
Comprehensive evaluation of historical sales behavior across orders, sellers, states, and product categories to identify trends and seasonal patterns.

- **Category 2 Product and Category Performance:** 
In-depth analysis of product and category-level performance to determine which categories drive the highest sales for both individual sellers and the company overall.

- **Category 3 Customer Behavior and Segmentation:**
Detailed customer analysis aimed at understanding purchasing behavior, identifying customer segments, and evaluating how each segment contributes to total sales and profitability.

- **Category 4 Geographic Sales Distribution:**
Assessment of sales performance across states and cities, including identification of top-performing sellers and regions with growth opportunities.

- **Category 5 Review Score and Service Quality Analysis:**
Examination of review scores across categories and sellers to uncover service issues, category logistics problems, and improvement opportunities.

- **Category 6 Order payments type Analysis:**
Detailed analysis of payment type and number of installments per order value, state, sellers and categories

- **Category 7 Strategic Recommendations:** 
Development of data-driven guidance to support business decisions aimed at enhancing customer satisfaction, strengthening seller engagement, and increasing overall sales performance.


The python code to make exploratory analysis and cleaning the data can be found here:  
[Python Cleaning and Exploration Code](https://github.com/Emma922/Olist-Project/blob/302c4819153578439040c44af7a7dab13978ef14/Olist_EDA_cleaning.ipynb)

Targeted SQL queries for various business questions can be found here:  
[SQL Business Questions Queries](https://github.com/Emma922/Olist-Project/tree/ab7fa770a9f45d0e2c80d9a230c366801487e88e/SQL%20queries)

Olist Dataset:
![Olist Dataset](https://github.com/user-attachments/assets/16cada77-7551-48b8-bac7-af613f819bec)



Interactive Tableau dashboards for business perormance analysis are available here:  
- [Business Performance Dashboard](https://public.tableau.com/app/profile/emmanuel.casta.o/viz/Olist_17646411959020/Dashboard1)
<img width="1459" height="1279" alt="Dashboard 1 (6)" src="https://github.com/user-attachments/assets/0ee35a44-7548-4693-a773-0db74235fb3d" />


## Executive Summary

### Overview of Findings

Asprice Makeup showed steady growth earlier in the year, but recent sales dropped sharply by up to 83%. The analysis indicates that the absence of a loyalty program, weak marketing focus, limited promotions, and lack of wholesale channels contributed to this decline.

Key insights include:

- It is observed that there is consistent sales growth per year, while no seasonality patterns are demonstrated 
- Category and seller sales follow the Pareto rule
- More than 50% of sellers contribute only 5% revenue, it suggests that many sellers might be inactive
- Only 7 out of 75 categories comprise almost 50% of total sales
- Olist lacks of customer loyalty. Based on the RFM analysis, customers who contribute most  to the sales did not make additional purchases
- Outperforming states show lower freight values, while underperforming states tend to have higher freight values. This indicates that shipping cost strongly influence purchasing behavior.
- There are certain issues related to logistics. Even a few of the highest-performers products show complaints. Additionally, there is a significant quantity of low-quality review sellers who have sold a considerable amount of products.
- Customer financing preferences depend on the type of goods, particularly for expensive or long-term items.

### Based on these findings, Olist would benefit from:

- Leverage company growth through marketing ads across Brazil to sustain momentum and expand reach.
- Sellers-focused campaigns to encourage sales activity, providing training, incentives or
promotional tools to activate inactive sellers.
- Marketing campaigns focused on outperforming products and categories
- Balance freight values for underperforming states to encourage sales in these places
- Watch out for logistics and seller complaints by strengthening quality control, improving delivery reliablity, and monitoring seller performance.
- Take advantage of customer financing preferences through targeted marketing and financial strategies
- Implement customer engagement programs to increase repeat purchases.

---

## Insights Deep Dive

### Historical Sales Performance

- All months shows a consistent growth per year, indicating a general growth trend in sales per year.
This suggests that Olist has been strengthening its presence in the Brazilian market over time. 
- This group makes up only **15% of customers** but contributes **36% of total sales**.
  
- Based on the available data, we can infer that Olist may exhibit a seasonality pattern during the first 2 quarters of the year. However, due to the limited data across full yearly cycles, 
this conclusion cannot be confirmed with certainty. Since the dataset only extends to September 2018, we lack information on the final quarter of that year, preventing a complete comparison between first-quarter and last-quarter sales performance.

- The increase in sales observed during the first months of 2018 may be attributed to Olist�s overall growth rather than to a definitive seasonality pattern. 
With the current dataset, we cannot reliably distinguish between structural growth and seasonal effects.

![Customer Loyalty Snapshot](https://github.com/user-attachments/assets/5fb94855-efe2-4ff0-b9db-9a7a6ce6c7a5>)


### Products and Brand Distribution

- The data shows a strong **20–80 pattern**:
  - Only **18% of brands** generate **79% of total revenue**.
  - **20% of products** represent **60% of overall sales**.
  - The top-performing products contribute **35% of total revenue**.
  - One product alone accounts for about **10% of total revenue**, revealing significant dependence on a small product base.

![Brand and Product Distribution](https://github.com/user-attachments/assets/e28a604c-0ed3-4d77-a221-a20a4a1f3de2)

### Average Order Value (AOV) per Customer

- While most business metrics declined recently, **AOV increased**, indicating improved purchasing behavior.
- The rise in AOV correlates with the introduction of wholesale sales on September 7.
- Since then, AOV per customer has steadily risen despite overall sales dropping.

![AOV Trend](https://github.com/user-attachments/assets/c02efdc7-909e-4966-ae4d-94e52f3871f6)

---

## Recommendations

Based on the analysis, the following actions are recommended to the stakeholder team:

- **Customer Loyalty is a strong growth opportunity:**  
  Develop and launch a formal loyalty program rewarding repeat customers with gifts, special offers, or exclusive bundles to encourage retention.

- **Encourage purchases of top brands:**  
  Run targeted promotions or marketing campaigns promoting the top 5 brands to increase average order value (AOV) and sales volume.

- **Promote high-performing products at checkout:**  
  Recommend these products during the checkout process and offer exclusive discounts to increase sales and AOV.

- **Expand and improve wholesale sales:**  
  Maintain current wholesale channels, create different wholesale categories to reach a broader customer base, and increase wholesale options.

- **Launch retention-focused discounts:**  
