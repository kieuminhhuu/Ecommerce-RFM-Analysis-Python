# Ecommerce RFM Analysis[Python]
## I. Introduction
### 1. RFM Analysis
- **RFM (Recency – Frequency – Monetary)**: is a part of Marketing Analysis and is used to analyze customer value, thereby helping businesses analyze each group of customers they have to have special marketing or care campaigns
  - Recency: Distance from the last purchase to the specified date
  - Frequency: Frequency of purchases within a specified period of time
  - Monetary: Amount spent within a specified period of time
- **Quintiles method** is a statistical method of dividing data into five equal groups (or quantiles), each group accounting for 20% of the total observations
- **How to assign points to each indicator**: Assign scores from 1 to 5 to the R, F, M indices, which will be divided according to **the quintile method**:
  - Recency: Customers who purchase more recently will get a higher score
  - Frequency: Customers who purchase frequently will get a higher score
  - Monetary: Customers who spend more will get a higher score
- Combine the scores of each RFM index to create an overall score for each customer, from which they are classified into the corresponding customer group.
### 2. Dataset
- A dataset of a multinational online retail company containing all transactions that occurred between December 1, 2010 and December 9, 2011. The company primarily sells gifts for special occasions. Many of the company's customers are wholesalers.
### 3. Data Description
![ds](https://github.com/user-attachments/assets/2b786299-b2ea-4e15-adc3-22fe2f2a85d3)
### 4. Business Question
- The Marketing Department wants to run marketing campaigns to thank customers who have supported the company over the past time as well as exploit customers with the potential to become loyal customers, so the Marketing Department needs a customer group section. The Marketing Director proposed to the team a plan to use the RFM model implemented in Python to be able to process the large amount of data currently available from the company, perform analysis and make recommendations. 
## II. Data Visualization bằng Python
- Distribution of R values <br />
<img src="https://github.com/user-attachments/assets/aae364f6-d2a1-4951-9408-cc5e8d9cca96" alt="..." width="600" /><br />
- Distribution of F values <br />
<img src="https://github.com/user-attachments/assets/b51ab355-cecd-47b2-99d0-5cbc462a0bf1" alt="..." width="600" /><br />
- Distribution of M values <br />
<img src="https://github.com/user-attachments/assets/4b58366b-a2ce-4f33-a347-a52b05dd2b42" alt="..." width="600" /><br />
- Distribution of R and F values <br />
<img src="https://github.com/user-attachments/assets/7ca6f384-cbfd-4b26-b76b-5de9ac36fb04" alt="..." width="600" /><br />
- Distribution of R and M values <br />
<img src="https://github.com/user-attachments/assets/8bc5dc03-8bb9-4a28-80ab-32357b161a6c" alt="..." width="600" /><br />
- Distribution of F and M values <br />
<img src="https://github.com/user-attachments/assets/dd5aeb43-3312-4ab5-9c56-14bc05b63a3b" alt="..." width="600" /><br />
- Treemap <br />
<img src="https://github.com/user-attachments/assets/6f41e36f-4a89-4c2a-addb-c857fc5caffc" alt="..." width="600" /><br />
- Revenue from Segments <br />
<img src="https://github.com/user-attachments/assets/81c771d7-94aa-422e-9fcf-1677def11609" alt="..." width="600" /><br />
## Insight
- From the revenue chart by segment, we see that the champion group contributes significantly to the revenue of the business. A key characteristic of this group is that they often make purchases and the orders are of high value. Therefore, measures need to be taken to retain these customers
- Looking at the TreeMap chart, we see that the 4 groups Lost, New Customer, Hibernating Customer, Promissing account for the 1st, 3rd, 4th, and 5th percentiles in the customer group. The behavior of each of these groups is as follows:
  - Lost is a group of customers who have not returned for a long time, the order value of this group is not high
  - New Customers are those who have made recent purchases, but their purchase frequency and order value are not high
  - Hibernating Customers are those who have not returned for a long time, have weak purchasing power, and low basket value
  - Promising Customers are those who have recently made a purchase with a high order value but have not bought frequently yet
- These 4 groups account for a large proportion of the customer group but bring in very low revenue. Combined with the scatter charts, it can be seen that businesses do not have measures to attract customers to return to buy and do not have measures to increase the frequency and value of purchases, leading to a very low proportion of loyal customers and potential customers
## Recomendation
- For the Champions group, businesses should implement dedicated programs for loyal customers, such as a points system, exclusive VIP benefits, or enhanced customer care services, in order to retain this group
- There should be measures to attract back customers who have not returned for a long time, such as those in the Lost, Hibernating, and Needing Attention groups. Some possible measures include
  - Send emails introducing new product categories based on previously purchased products or those in which customers have shown interest
  - Offer coupons to customers when they return to shop
- To increase the purchase frequency or order value for New Customers and Promising groups, the following methods can be used:
  - Send information introducing products similar to those purchased by other customers, but of higher quality.
  - Send information introducing complementary products that pair with the ones customers have already purchased.
