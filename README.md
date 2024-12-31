# Marketing-Insights-For-E-Commerce-Company-


Business Context:  
One of the leading E-Commerce Company would like to get marketing insights from the data to 
define marketing strategies going forward.  Also, expecting to build an analytical dashboard to 
monitor various KPI’s & business metrics. 
Available Data: 
Transaction data has been provided for the period of 1st Jan 2019 to 31st Dec 2019. The below data 
sets have been provided.  
Online_Sales.csv: This file contains actual orders data (point of Sales data) at transaction level with 
below variables. 
CustomerID: Customer unique ID 
Transaction_ID: Transaction Unique ID 
Transaction_Date: Date of Transaction 
Product_SKU: SKU ID – Unique Id for product 
Product_Description: Product Description 
Product_Cateogry: Product Category 
Quantity: Number of items ordered 
Avg_Price: Price per one quantity 
Delivery_Charges: Charges for delivery 
Coupon_Status: Any discount coupon applied 
 
Customers_Data.csv: This file contains customer’s demographics. 
CustomerID: Customer Unique ID 
Gender: Gender of customer 
Location: Location of Customer 
Tenure_Months: Tenure in Months 
 
Discount_Coupon.csv: Discount coupons have been given for different categories in different 
months 
Month:  Discount coupon applied in that month 
Product_Category: Product category 
Coupon_Code: Coupon Code for given Category and given month 
Discount_pct: Discount Percentage for given coupon 
 
Marketing_Spend.csv: Marketing spend on both offline & online channels on day wise. 
Date: Date 
Offline_Spend: Marketing spend on offline channels like TV, Radio, NewsPapers, Hordings etc… 
Online_Spend: Marketing spend on online channels like Google keywords, facebook etc.. 
 
Tax_Amount.csv: GST Details for given category 
Product_Category: Product Category 
GST: Percentage of GST


Key Definitions: 
Invoice Value:  Invoice Value =(( Quantity*Avg_price)*(1-Dicount_pct)*(1+GST))+Delivery_Charges 
Average order value = Revenue / Transaction per customer 
 
Profit Margin Profit margin is the commonly used profitability ratio. It represents how much 
percentage of total sales has earned as the gain. 
 
Purchase Frequency is the average number of purchases made by a customer over a defined period 
of time (typically one month or one year). It is the sum of total number transactions divided by total 
number customers. 
 
Repeat rate shows you the percentage of your current customer base that has come back to shop 
again. 
 
Churn Rate is the annual percentage rate at which customers stop subscribing. 
 
Customer lifetime value, lifetime customer value, or life-time value is a prediction of the net 
profit/revenue attributed to the entire future relationship with a customer. 
Business Objective: 
The e-commerce company is expecting below analysis using the data 
1. Calculate Invoice amount  or sale_amount  or revenue for each transaction and item level 
 Invoice Value =(( Quantity*Avg_price)*(1-Dicount_pct)*(1+GST))+Delivery_Charges 
2. Perform Detailed exploratory analysis 
 Understanding how many customers acquired every month 
 Understand the retention of customers on month on month basis 
 How the revenues from existing/new customers on month on month basis 
 How the discounts playing role in the revenues? 
 Analyse KPI’s like Revenue, number of orders, average order value, number of 
customers (existing/new), quantity, by category, by month, by week, by day etc… 
 Understand the trends/seasonality of sales by category, location, month etc… 
 How number order varies and sales with different days? 
 Calculate the Revenue, Marketing spend, percentage of marketing spend out of 
revenue, Tax, percentage of delivery charges by month. 
 How marketing spend is impacting on revenue? 
 Which product was appeared in the transactions? 
 Which product was purchased mostly based on the quantity? 
3. Performing Customer Segmentation 
 Heuristic (Value based, RFM) – Divide the customers into Premium, Gold, Silver, 
Standard customers and define strategy on the same.  
 Scientific (Using K-Means) & Understand the profiles. Define strategy for each 
segment.  
4. Predicting Customer Lifetime Value (Low Value/Medium Value/High Value) 
 First define dependent variable with categories low value, medium value, high value 
using customer revenue.

 Then perform Classification model 
5. Cross-Selling (Which products are selling together) 
 You can perform exploratory analysis & market basket analysis to understand which 
of items can be bundled together. 
6. Predicting Next Purchase Day(How soon each customer can visit the store (0-30 days, 30-60 
days, 60-90 days, 90+ days) 
 For this, we need create dependent variable at customer level (average days per one 
transaction for only repeat customers and divide into groups 0-30 days, 30-60 days,  
60-90 days and 90+ days) then build classification model to predict next purchase of 
given customer. 
7. Perform cohort analysis by defining below cohorts 
 Customers who started in each month and understand their behaviour  
 Which Month cohort has maximum retention?


Other inputs related to Analysis for additional reference: 
1. Why do we need customer Segmentation? 
As every customer is unique and can be targeted in different ways. The Customer segmentation 
plays an important role in this case. The segmentation helps to understand profiles of customers and 
can be helpful in defining cross sell/upsell/activation/acquisition strategies. 
2. What is RFM Segmentation? 
RFM Segmentation is an acronym of recency, frequency and monetary based segmentation.  
Recency is about when the last order of a customer. It means the number of days since a customer 
made the last purchase. If it’s a case for a website or an app, this could be interpreted as the last 
visit day or the last login time. 
Frequency is about the number of purchases in a given period. It could be 3 months, 6 months or 1 
year. So we can understand this value as for how often or how many customers used the product of 
a company. The bigger the value is, the more engaged the customers are.  
Alternatively 
We can define, average duration between two transactions 
Monetary is the total amount of money a customer spent in that given period. Therefore big 
spenders will be differentiated with other customers such as MVP or VIP. 
3. What is LTV and How to define it? 
In the current world, almost every retailer promotes its subscription and this is further used to 
understand the customer lifetime.  Retailer can manage these customers in better manner if they 
know which customer is high life time value. 
Customer lifetime value (LTV) can also be defined as the monetary value of a customer relationship, 
based on the present value of the projected future cash flows from the customer relationship. 
Customer lifetime value is an important concept in that it encourages firms to shift their focus from 
quarterly profits to the long-term health of their customer relationships. Customer lifetime value is 
an important metric because it represents an upper limit on spending to acquire new customers. For 
this reason it is an important element in calculating payback of advertising spent in marketing mix 
modelling. 
4. Why do need to predict Customer Lifetime Value? 
The LTV is an important building block in campaign design and marketing mix management.   
Although targeting models can help to identify the right customers to be targeted, LTV analysis can 
help to quantify the expected outcome of targeting in terms of revenues and profits. The LTV is also 
important because other major metrics and decision thresholds can be derived from it.  
For example, the LTV is naturally an upper limit on the spending to acquire a customer, and the sum 
of the LTVs for all of the customers of a brand, known as the customer equity, is a major metric for 

business valuations. Similarly to many other problems of marketing analytics and algorithmic 
marketing, LTV modelling can be approached from descriptive, predictive, and prescriptive 
perspectives. 
5. How Next Purchase Day helps to Retailers? 
Our objective is to analyse when our customer will purchase products in the future so for such 
customers we can build strategy and can come up with strategies and marketing campaigns 
accordingly. 
     a. Group-1: Customers who will purchase in more than 60 days 
     b. Group-2:  Customers who will purchase in 30-60 days 
     c. Group-3: Customers who will purchase in 0-30 days       
 
6. What is Cohort Analysis? How it will be helpful? 
A cohort is a group of users who share a common characteristic that is identified in this report by an 
Analytics dimension. 
For example, all users with the same Acquisition Date belong to the same cohort.  
The Cohort Analysis report lets you isolate and analyze cohort behaviour. 
Cohort analysis in e-commerce means to monitor your customers’ behaviour based on common 
traits they share – the first product they bought, when they became customers, etc. - - to find 
patterns and tailor marketing activities for the group.
