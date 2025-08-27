# Strategic Insights for Credit Card Launch & Customer Segmentation

## Summary
This project analyzes customer demographics and spending behavior for a leading retail bank. The aim is to support the launch of a new line of credit cards. Using customer and transaction data, I identified distinct customer segments and usage patterns. The insights revealed high-potential groups and can be used for targeted strategies to boost adoption and engagement. The project emphasizes a data-driven, customer-centric approach to product design and marketing.

## Business Objectives
- Understand spending behaviour and credit card usage trends by demographic groups
- Segment customers based on income and spending behavior
- Identify high-potential users for marketing outreach
- Recommend strategic actions for launching new card products

## Exploratory Data Analysis (EDA) Summary

### Customer Demographics - dim_customers
-	Total Customers: 4,000 customers
-	Average Income: ₹51,657 ; Min: ₹24,816 ;	Max: ₹86,600
-	Age Groups: 21-24, 25-34, 35-45, 45+
-	Cities: Mumbai, Delhi NCR, Chennai, Hyderabad, Bengaluru
- Occupations: Salaried IT Employees, Salaried Other Employees,	Business Owners, Freelancers,	Government Employees
-	Genders: Male, Female
-	Marital Status: Married, Single

### Customer Spend Data - fact_spends
-	Total Records: 864,000 (6 months × 9 categories × 4,000 customers × 4 payment types)
-	Total Unique Customers: ✅ 4,000
-	Average Spend per transaction: ₹614.47 ;	Min: ₹6 ;	Max: ₹10,313
-	Months: May to October (6 months)
-	Categories (9 total):
Entertainment, Apparel, Electronics, Food, Groceries, Travel, Bills, Health & Wellness, Others
-	Payment Types:
Credit Card, Debit Card, UPI, Net Banking

## Key KPIs Tracked:
- Avg Income, Avg Monthly Spend
- Credit Card Usage % {(Credit card spend ÷ total spend) × 100}
- Income Utilization % {(Total spend ÷ Total income) × 100}
- Spend Categories
- Monthly Spend Trends

## Customer Demographics
## ![p-1](https://github.com/user-attachments/assets/7e8d072e-c510-407c-bf89-dd38086469a4)

Before going to the insights from this page, I would like to note that I have added a new column of **'Income group'** in the Customers table, which is as follows:
- **'Premium'**- Customers with income > 58000;  **'Regular'**- Income range 40000 to 58000;  **'Budget'**- Income < 40000.
- **"40000"** was around the **33rd percentile** of the income range for the entire population, and **"58000"** was around the **60th percentile**.

### Top Insights:
- **25-34 Age group** dominates the customer base with **1498 customers**.(Offers on products for such age group must be increased)
- **45+ Age group** despite having the **highest average income**(48% more than 21-24 age group), is the lowest in count i.e only **13.5% of the customer base**.(Massive untapped opportunity for premium customer aquisition)
- **78.4%** of the customers are **Married**.(More focus on offers/points on familiy friendly products like grocery, dinings, travel,etc)
- **Salaried IT Employees** dominate the customer base(**32%**),and also in the city with highest customers i.e **Mumbai**.
- Most of the **Business Owners and Salaried IT** people come in the **Premium** income group and earn more than 58000 per month.(Big market for premium cards) Whereas most of the **Govt Employees** come in the **Regular** income group, i.e, between 40k to 58k.
- **Hyderabad** has the lowest count of customers, i.e., **593 only**. (Emerging Market, so more marketing campaign is needed here)

## Spending Behaviour 
## ![p-2](https://github.com/user-attachments/assets/0b33cd1a-1640-479e-a6a2-69d4bee5f715) 
### Top Insights:

#### Spend, Income Utilization % and Credit card usage %
 ![c1](https://github.com/user-attachments/assets/fa895e61-5fab-439c-90ee-ab74839b24d8)    ![c2](https://github.com/user-attachments/assets/ca78d470-4373-4182-9d37-a33cbb30e2b3)
- Total Spends in 6 months is: 530.9M, Average Monthly Spend is: 22.12K
- SO, the average **Income Utilization %** comes out to be: **42.82%**
- ![c3](https://github.com/user-attachments/assets/4e423df4-bae5-4f50-88d9-6751fb67d4d3)
- **Credit card usage %** is the amount spent through credit card vs the total amount spent, which on average comes out to be: **40.74%**, indicating a great acceptance of credit cards. (Marketing expenses will be less, and adoption will be easy)

#### By Age Group:
 ![c4](https://github.com/user-attachments/assets/05437f08-5901-4a24-96fb-a305fa0d19ae)
- Age group **35-45** is the highest spender, with the **income utilization % as 46.72%** and a decent credit card usage of 38.78%.
- Age group **25-34** has the highest **credit card usage of 46.62%** and the second-highest income utilization of 43.66%.
- Age group **45+** is the highest earners of all, but also a frugal & wise spender with **income utilization of 34.7%** and also low credit card usage of only 35.73%.

#### By Occupation:
 ![c6](https://github.com/user-attachments/assets/91521906-7b1f-49a3-8631-af057c9a98b6) 
- **Salaried IT employees** lead in spending, with **income utilization of 51.04%** and the 2nd highest avg income of about 61k.(High Income || Premium segment)
- **Business owners**, despite having the **highest avg income of 70k**, spend frugally with **income utilization of 33.22%**.(High Income || Premium segment)
- **Government Employees** are the lowest spenders with **income utilization of 29%**. (Stable Income || Maybe because they get many things free and subsidised from the govt itself.)
- **Freelancers**, despite having low income, have the 2nd highest **income utilization of 45.8%**. (Unstable Income || Because most of their income gets spent on necessities.)

#### By City:
 ![c5](https://github.com/user-attachments/assets/5589f699-4a21-45f8-b583-547e86e2086b)
- **Mumbai** has the highest income utilization of **51.43%**. (Business hub || High concentration of Business owners and IT Professionals)
- **Chennai** has the lowest income utilization of **31.1%**.

#### By Payment Type and Marital Status:
 ![c9](https://github.com/user-attachments/assets/7fe099bf-e058-4f80-98ae-957817648eca)  ![c10](https://github.com/user-attachments/assets/d76b187b-1f05-4808-b052-ef52e4b7e7c1)
- Credit cards already dominate spending, totalling 216M, followed by UPI (141M).
- Married people are the highest spenders, totalling 429M, with 80.8% of the total spend. (Focus on more family-friendly offers should be given)

#### By Categories:
  ![c7](https://github.com/user-attachments/assets/5b841ae0-5d2d-47b5-9b28-91710fef1b29)
- **'Bills'** has the highest spending of **105M**, followed by **'Groceries'(86M)** and **'Electronics'(80M)**.
- Payment for 'Groceries' is less from Credit card(27M) and highest from UPI(29M). (Because most of the vendors don't have card payment machines and deal in cash or UPI only)
- **Age group 21-24** has some different spending choices:
- ![c11](https://github.com/user-attachments/assets/ae944126-52b5-4e28-bf0e-8151f4f7e7c9)
- They spend the highest on 'Entertainment' (15.1M), followed by 'Electronics' (11.4M) and 'Apparel' (11.1M).

#### By Monthly Trend:
 ![c8](https://github.com/user-attachments/assets/c01d384e-3a79-4752-9039-1320845bfd71)
- **August and September** are the highest spending months, totalling 217M, constituting **40.8%** of the total spend, with September being the highest one at 116M.
- This is because of the festive season during those months. ( More focus on offers, discounts, and collaborative promotions must be there during these times)

#### Spending behaviour by Income:
 ![c12](https://github.com/user-attachments/assets/f5cb32ad-e932-48be-b0a4-c356bc6bce28)
- Here, as per the scatter plot for spend vs income, I took 30k on the spend line as a differentiating point because it was almost 50% of the high-income group's average monthly income. And for the income side, the three different income groups from earlier were taken into consideration.
- This revealed 5 very important customer segments based on high value, hidden value, emerging, and risky customers, for which the details are in the next slide.

## Customer Segmentation
##  ![p-3](https://github.com/user-attachments/assets/8f55a262-0274-463c-935d-657ce7554ab2) 
 Here, customers were divided into 5 major segments based on their spend vs income:
- "High Value" - income> 58000 ; spend > 30000
- "Prime Minimalists" - income> 58000 ; spend < 30000
- "Emerging" - income between 40000 and 58000 ; spend < 30000
- "Risky" - income < 40000 ; income utilization > 50%
- "Others"

### Top Insights:
#### Customer segments:
- The 'Emerging' segment is highest in numbers (28.2%), followed by 'Prime Minimalists' (21.5%).
- There are 9.8% 'Risky' customers also, who should be kept under watch.

#### By City and Age group:
 ![c2](https://github.com/user-attachments/assets/7d9c0dd2-ec43-467f-baaf-81abcdb9a3e6)  ![c1](https://github.com/user-attachments/assets/253e3de1-2d88-45f5-abaa-662af15d2be6)
- **Mumbai** has the highest count of **'High value' customers (327)** as well as **'Emerging' customers (310)**, followed by Delhi-NCR with 216 'High value' customers and 3rd highest count of 'Emerging' customers (199).
- Chennai and Hyderabad don't have any 'Risky' customers. (Nice)
- **Chennai** has the highest count of **'Prime Minimalists'** customers (332), followed by Hyderabad at 189.
- Mumbai and Delhi-NCR are the highest spenders, whereas Chennai and Hyderabad are the least spenders.
- Age group **25-34** has the highest no. of **'Prime Minimalists' (376)** and **35-45** age group has highest count of **'High Value' customers(352)**.
- Age group **21-24** has the highest count of **'Emerging' customers(385)**, but doesn't has any high income customers.
- Age group **45+** mostly consists of **'Prime Minimalists'(245)**, followed by **'Emerging'(156)**.

#### By Gender, Marital Status, Occupation, and Payment Type:
 ![c4](https://github.com/user-attachments/assets/34d8f202-13f0-4df8-88b5-5da537f93c2f)  ![c7](https://github.com/user-attachments/assets/91f5fab0-6a5b-4328-9f72-5ab9fc06fa79)
  ![c3](https://github.com/user-attachments/assets/08e4cb05-e086-4ca0-a1be-e2d26f36662d)   ![c5](https://github.com/user-attachments/assets/e7004995-fa28-45ad-ad1a-94a38adaa1c6)
- In both Male and Female genders, the **'Emerging'** customers are highest, followed by 'Prime Minimalists'.
- Married people are mostly 'Emerging' customers(790), followed by 'Prime Minimalists'(777) and 'High Value'(661), while Singles are mostly 'Emerging'(338).
- IT Employees contain the highest count of 'High value' customers(670), followed by only 85 Business Owners.
- Business owners contain the highest count of 'Prime Minimalists' customers(456), followed by 358 in IT Employees, and only 46 Govt Employees.
- Other salaried employees and freelancers don't have any high-income customers, and Freelancers are the most 'Risky' customers(285).
- All of the segments use credit cards the most, followed by UPI.

#### By Categories:
  ![c6](https://github.com/user-attachments/assets/d91537c8-98e6-44aa-b0c5-4a48445c5d5b)
- 'High Value' customers are the highest spenders across all categories except Entertainment and Apparel, where 'Emerging' customers dominate.
- In both Electronics and Food, the high-income 'Prime Minimalists' customers are spending less than the 'Emerging' customers who are in the middle-income range.

## Strategic Recommendations
### Target High-potential Customer Segments
As per the findings from above, the top 3 target segments were identified for the new card launch:
#### "High Value"
- Ideal for **Ultra Premium cards** with exciting offers and cashback points across all categories and premium banking services.
- 25-34 and 35-45, i.e, **25-45 age group**, are the primary target audience. Therefore, focus more on offers related to that age group.
- Mainly concentrated in **Mumbai and Delhi-NCR**. (More marketing focus in these cities) And only 2 occupations, **IT Employees** and **Business Owners**, come under this category.
- For business owners, they must be given interest-free extra time for repayment, and Airport lounge access.
- IT Professionals should be given exclusive offers on tech purchases, software subscriptions, online services, up-skilling courses, and travel-related offers.
- Cashbacks on Utility Bills, Groceries, Electronics, Health & Wellness, and Travel bookings.

#### "Prime Minimalists"
- Ideal for **Premium cards** with zero annual fee, including offers like investment services and retirement planning, etc.
- 25-34 and 45+ age groups are the primary target, followed by the 35-45 age group. As in the 45+ age group, this segment is the majority, so we should focus more on acquiring more 45+ customers.
- More marketing focus in Chennai(the highest count of this segment), followed by Hyderabad. The majority of those are Business owners and IT Employees, and a little bit of Government employees.
- Cashbacks on investments like Mutual funds or SIPs, Groceries, Health & wellness centres and devices.
- Special Credit card digital coaching to lessen fear and promote proper use of cards and shift their debit card usage to credit cards. 

#### 'Emerging'
- Ideal for **Cashback cards** with special offers and cashbacks on Entertainment, Apparel, and others.
- 21-24 and 35-45 age groups are the primary target customers.
- Equal marketing focus across all locations as they are spread everywhere, with the highest in Mumbai.
- Other salaried employees and Government Employees are our main target, so focus offers tailored to them.
- Special retirement planning services for salaried employees, and cashbacks on investments.

- ##### For **Risky** customers, we should keep them on watch for overspending or utilizing the full limit of the card, restrict the limit of the card, send regular nudges about the usage, and create free credit coach programs for them on the app itself. For **"Other"** categories, they are not currently in focus for new cards, but they should be monitored for future actions.
#### Other General Recommendations
- 
