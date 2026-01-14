# Olist Data Analysis Project

## Project Background

Olist founded in 2015 is the largest department store in Brazilian marketplaces, it connects small business and allows sellers offer their products while Olist is in charge of logistics.
This project analyzes sales from 2016 - 2018. The company has significant amount of records (100k) in orders, customers, sellers, products, locations and payments details. This project throughly analyzes and sythezises the data in order to obtain meaningful insights that will lead to improve performance in sales and different areas of the company.

**Insights and recommendations focus on the following key analytical areas:**

- **Category 1 Historical Sales Performance:**
Comprehensive evaluation of historical sales behavior across orders, sellers, states, and product categories to identify trends and seasonal patterns.

- **Category 2 Sellers and Category Performance:** 
In-depth analysis of sellers and category performance to determine which categories drive the highest sales for both individual sellers and the company overall.

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

Olist showed steady growth month by month. The analysis indicates a strong market presence, particularly in Sao Paulo (SP), Minas Gerais (MG), and Rio de Janeiro (RJ). Additionally, a lack of customer loyalty and logistic problems are key issues that prevent Olist from developing better sales numbers. 
Furthermore, there is observed the pareto rule in sales performance for categories and sellers, which means that Olist relies heavily on a few categories and sellers.

Key insights include:

- It is observed that there is consistent sales growth per year, while no seasonality patterns are demonstrated 
- Category and seller sales follow the Pareto rule
- More than 50% of sellers contribute only 5% revenue, which suggests that many sellers might be inactive
- Only 7 out of 75 categories comprise almost 50% of total sales
- Olist lacks customer loyalty. Based on the RFM analysis, customers who contribute most  to the sales did not make additional purchases
- Outperforming states show lower freight values, while underperforming states tend to have higher freight values. This indicates that shipping cost strongly influences purchasing behavior.
- There are certain issues related to logistics. Even a few of the highest-performing products show complaints. Additionally, there is a significant quantity of low-quality review sellers who have sold a considerable amount of products.
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

- All months show a consistent growth per year, indicating a general growth trend in sales per year.
This suggests that Olist has been strengthening its presence in the Brazilian market over time. 
  
- Based on the available data, we can infer that Olist may exhibit a seasonality pattern during the first 2 quarters of the year. However, due to the limited data across full yearly cycles, 
this conclusion cannot be confirmed with certainty. Since the dataset only extends to September 2018, we lack information on the final quarter of that year, preventing a complete comparison between first-quarter and last-quarter sales performance.

- The increase in sales observed during the first months of 2018 may be attributed to Olist�s overall growth rather than to a definitive seasonality pattern. 
With the current dataset, we cannot reliably distinguish between structural growth and seasonal effects.

![Customer Loyalty Snapshot](https://github.com/user-attachments/assets/a202a70e-f7f4-4bed-b4e2-0de7d446c750)



### Products and Category Performance

-  The data shows a strong **20–80 pattern**:
  - Only **7 out of 75** categories account for almost **50% of total sales**.
  - **21% of categories** represent **80% of total revenue**.
  - **17% of sellers** generate **80% of total sales**.
  - More than a half of sellers contribute **less than 5% of total revenue**.
  - **The top 10** sellers have different top 5 best-selling categories overall.
  - **The top 10** sellers generally rely heavily on one main category that generates the majority of their revenue


### Customer Behavior and Segmentation

- The "Best Customers" segment represents only 2% of the company's total revenue.
- "Potential Loyal Customers" contribute approximately one-fourth of total revenue, highlighting the importance of implementing loyalty-building initiatives.
- The "At Risk" segment accounts for nearly one-third of all customers, indicating that many previously frequent buyers are no longer generating sales.
- These findings underscore the importance of maintaining customer relationships over time to secure consistent and recurring revenue.
- Based on the RFM analysis, customers who contribute most  to the sales did not make additional purchases

Nr. Orders per Customer Viz
- This chart shows the dominance of single-purchase customers, which suggests low repeat purchase rates


![Nr. Orders per Customer](https://github.com/user-attachments/assets/8a2627b8-65f8-49cd-aa54-08d71a6871b2)

### Geographic Sales Distribution

- Beleza_saude appears in the top 5 categories in every state, indicating consistently strong performance
  and broad customer demand across the country.
- Cama_mesa_banho appears in the top 5 in only 8 out of 27 states, which suggests a more region-specific demand.
Addtionally, it is purchased mainly in the highest-revenue states, showing stronger demand in larger and more developed markets.
- Sao Paulo (SP) is the state with the highest overall revenue. It also shows high category diversification,
meaning its sales are distributed across many different product categories rather than concentrated in a few.
- Consumer preferences are relatively consistent across states, but purchasing power and market size vary significantly.
- States with the highest revenue also tend to have the largest number of sellers. In contrast, low-revenue states usually have very few sellers or in some cases, none, indicating that seller scarcity directly limits sales potential.

Sales Performance by State (to consult state details and accurate specific information please enter into the dashboard)


![State Performance](https://github.com/user-attachments/assets/fcf24d00-c86a-41f8-8dd3-95a2bdaf5edc)

### Review score and Service Quality

- Several sellers show low average ratings (<3.0), suggesting operational deficiencies such as late shipments, poor handling, or inconsistent service. 
These sellers should be monitored closely and may require training or performance improvement plans.

- Delivery delays significantly reduce customer satisfaction, as evidenced by the lower average review scores for delayed orders.
This reinforces the importance of logistics efficiency and accurate delivery-time estimates.

- Categories with both high sales volume and high review scores represent strong performance areas. 
In contrast, categories with low review scores signal opportunities for targeted service or product improvements.

- Moveis_escritorio is a high-priority category for intervention because it combines low review scores with high order volume, 
meaning a large number of customers are being negatively affected.

- Cama_mesa_banho is another key category: despite being among the highest in revenue and total orders, it also shows one of the lowest average review scores. 
This mismatch indicates a risk of long-term customer dissatisfaction in a high-impact category.

- Seller 7c67e1448b00f6e969d365cea6b010ab stands out as a critical case: despite selling over 1,300 products, 
the seller maintains the lowest average review scores, suggesting severe operational or quality-related issues.

- Improving logistics reliability and monitoring low-performing sellers could significantly raise customer satisfaction across the platform.

### Order payments type

- High-installment sellers vary significantly across product categories. 

- Categories like 'eletrodomesticos_2', 'moveis_decoracao', and 'automotivo' have the highest average installments, suggesting reliance on financing for higher-priced or durable goods.

- Customer financing preferences align with product type, particularly for expensive or long-term purchase items. 


## Recommendations

Based on the analysis, the following actions are recommended to the stakeholder team:

- **Company growth:** Leverage company growth through marketing ads across Brazil to sustain momentum and expand reach.
- **Seller campaigns:** Sellers-focused campaigns to encourage sales activity, providing training, incentives or
promotional tools to activate inactive sellers.
- **Marketing campaigns:** Marketing campaigns focused on outperforming products and categories
- **Underperforming teams:** Balance freight values for underperforming states to encourage sales in these places
- **Logistic and seller:** complaints campaigns:*Watch out for logistics and seller complaints by strengthening quality control, improving delivery reliablity, and monitoring seller performance.
- **Customer preferences:**(Take advantage of customer financing preferences through targeted marketing and financial strategies
- **Customer engagement:** Implement customer engagement programs to increase repeat purchases.
