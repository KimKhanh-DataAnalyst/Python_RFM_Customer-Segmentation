# Python_RFM_Customer-Segmentation
Please see the coding file attached or reach this link: https://colab.research.google.com/drive/1_WX6LpONUoPyFxfKNza9nOfvzUkt3UBi#scrollTo=ca6787be

# I. Introduction
## 1. Business question
- SuperStore is a global retail company. The Marketing Department wants to run marketing campaigns during the Christmas and New Year holidays to thank customers for their past support of the company. In addition, potential customers can be upgraded to become loyal customers.
- The Marketing Director also proposed a plan to use the RFM model in Python to segment customers and then launch appropriate marketing campaigns. Analyze the current situation of the company and give suggestions to the Marketing team
- With the retail model of Superstore company, which indicator should be most focused on in the 3 indicators R, F, and M?
## 2. Dataset
Dataset includes 4 different related tables including: transaction information, products information, returned orders of customers purchasing products from 2014 to 2017 and RFM classification

- Transaction information dataframe
  <img width="1230" alt="Image" src="https://github.com/user-attachments/assets/b58db1d4-5519-44f2-b4a9-a114a0be0e05" />[](url)

- Returned orders dataframe: We have to filter orders that were not returned before RFM anaalysis.

  <img width="498" alt="Image" src="https://github.com/user-attachments/assets/f9214240-9de9-44fd-9608-28f120b33289" />

- Segmentation dataframe: 'Product ID' is not unique because some products have same Product ID but have different Product Name => drop 'Product Name' then remove duplicate records so that 'Product ID' will be unique.

  <img width="670" alt="Image" src="https://github.com/user-attachments/assets/419d0b45-ac5e-4d55-a0c7-502fbf7e8065" />

- Products dataframe: We have to split each RFM score into single rows

  <img width="670" alt="Image" src="https://github.com/user-attachments/assets/4f39def6-3ba8-4e21-aa31-d5e7b948db67" />

## 3. RFM model
RFM is a method used for analyzing customer value. It is commonly used in database marketing and direct marketing and has received particular attention in retail and professional services industries
RFM stands for the three dimensions:
Recency – How recently did the customer purchase?
Frequency – How often do they purchase?
Monetary Value – How much do they spend?
RFM analysis numerically ranks a customer in each of these three categories, generally on a scale of 1 to 5 (the higher the number, the better the result). The “best” customer would receive a top score in every category.

# II. Data Visualization with Python

<img width="517" alt="Image" src="https://github.com/user-attachments/assets/b86a3c08-9f0b-4714-a59e-1a1c53710edd" />
<img width="515" alt="Image" src="https://github.com/user-attachments/assets/bf2530b6-4895-4b26-b966-8f2ccfc0ea2a" />
<img width="384" alt="Image" src="https://github.com/user-attachments/assets/13d2842f-5e89-494b-995f-8c221f25dd38" />
<img width="381" alt="Image" src="https://github.com/user-attachments/assets/64f28ec1-2977-4d7c-913e-282f3ace972d" />
<img width="645" alt="Image" src="https://github.com/user-attachments/assets/693f1b54-b631-45c1-8fd5-f903159d798f" />
<img width="656" alt="Image" src="https://github.com/user-attachments/assets/cc49ef59-a09b-4825-a2b2-c36575bd01af" />

# III. Insights

## 1. Recency, Frequency, and Monetary Value of Superstore

As a retailer, Superstore should prioritize Recency and Frequency over Monetary Value since their most loyal customers may make frequent purchases throughout the year at lower average transaction sizes. However, Superstore's Recency and Frequency metrics indicate areas for improvement:

The mean Frequency is 6 transactions per customer, which is relatively low for a retail company, indicating that customer loyalty is not strong.

The mean Recency is approximately 166 days, while the median Recency is 83 days. The significant difference between these two values suggests that a considerable portion of customers have high Recency values, indicating a high likelihood of customer churn.

## 2. Customer Segmentation Analysis (11 Segments of Superstore)

The two largest customer segments are Potential Loyalists (14.29%) and At Risk customers (12.14%).

Negative segments, such as Hibernating (11.38%) and Lost (10.49%), account for a significant portion of customers. However, these segments contribute to less than 8% of total revenue.

The two most valuable segments, Champions (8.98%) and Loyal Customers (7.84%), together make up less than 17% of the total customer base.

Potential Loyalists, considered an ideal target group, represent the highest proportion of customers (14.29%) but contribute only 9.02% of total revenue. Conversely, the At Risk segment accounts for 18.24% of revenue, indicating that these customers had significant past spending but are now disengaged.

Strategic Focus:

For the upcoming Christmas - New Year marketing campaign, Superstore should focus on:

Converting Potential Loyalists into Loyal Customers and Champions through engagement strategies.

Re-engaging At Risk customers to prevent further attrition.

## 3. Detailed Analysis of Key Segments

3a. Potential Loyalist Segment

The cart value in the Furniture and Technology categories declined in 2017, despite an increase in both the number of orders and total revenue. This shift suggests a change in customer purchasing behavior:

Furniture Category:

Number of orders increased by 53% (from 62 to 95 orders).

However, cart value decreased by 18% (from $326 to $226 per transaction).

Technology Category:

Number of orders increased by 38% (from 40 to 74 orders).

However, cart value decreased by 31% (from $383 to $266 per transaction).

Additionally, customer behavior across different sales channels shifted:

Consumer Segment:

Number of orders increased by 40% (from 112 to 186 orders).

However, cart value decreased by 26% (from $292 to $214 per transaction).

Home Office Segment:

Number of orders increased by 76% (from 30 to 53 orders).

However, cart value decreased by 22% (from $276 to $225 per transaction).

3b. At Risk Segment

In 2017, the At Risk segment showed a decline across all key performance indicators:

All three product categories (Furniture, Office Supplies, and Technology) saw declines in orders and revenue.

Office Supplies & Technology categories experienced declines in cart value:

Office Supplies: Cart value decreased by 23% (from $263 to $203 per transaction).

Technology: Cart value decreased by 22% (from $836 to $651 per transaction).

Furniture category, however, showed a positive trend:

Cart value increased from $350 to $476 per transaction, despite an overall decline in the number of orders.

Channel-Specific Trends:

Consumer and Corporate channels saw declines in orders, revenue, and cart value:

Consumer: Orders decreased by 17%, and cart value dropped by 38%.

Corporate: Orders decreased by 26%, and cart value dropped by 5%.

Home Office channel, however, exhibited a different trend:

Despite a 25% decline in order volume, cart value increased by 73%.

# IV. Recommendations

## 1. Improve Recency and Frequency Performance

Implement strategies to increase customer engagement and repeat purchases.

In the upcoming Christmas - New Year campaign, prioritize efforts to:

Convert Potential Loyalists into Loyal Customers and Champions.

Reconnect with At Risk customers to regain their engagement.

## 2. Recommendations for the Potential Loyalist Segment

Encourage higher cart values:

Offer special promotions for customers purchasing in the same category with cart values above $238.68 (the current segment average).

Create bundle deals or discounts for complementary products.

Introduce a Membership/Loyalty Program:

Focus on Consumer and Home Office channels.

Prioritize the Furniture and Technology categories.

Personalized product recommendations:

Promote best-selling sub-categories such as Paper, Binders, Furnishings, Storage, and Art.

## 3. Recommendations for the At Risk Segment

Investigate key factors behind customer attrition:

Analyze the correlation between return orders, product categories, and customer drop-off rates.

Conduct surveys using incentives (exchange points, gifts, or vouchers) to identify the main reasons customers have not returned.

Enhance customer retention strategies:

Introduce a free shipping upgrade policy: Since nearly 60% of orders use Standard Class shipping, offer a free upgrade to Second Class shipping as an incentive.

Send personalized email campaigns to At Risk customers with tailored recommendations based on their past purchases.

Promote best-selling sub-categories such as Binders, Paper, Furnishings, Phones, and Storage to re-engage previous buyers.


By implementing these strategies, Superstore can increase customer retention, improve purchase frequency, and drive higher revenues across key customer segments.
