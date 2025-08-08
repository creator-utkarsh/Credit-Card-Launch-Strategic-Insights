# Credit Card Strategy & Customer Segmentation
## Summary
This project analyzes customer demographics and spending behavior for a leading retail bank. The aim is to support the launch of a new line of credit cards. Using customer and transaction data, I identified distinct customer segments and usage patterns. The insights revealed high-potential groups and suggested targeted strategies to boost adoption and engagement. The project emphasizes a data-driven, customer-centric approach to product design and marketing.

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
- Credit Card Usage %(Credit card spend ÷ total spend) × 100
- Income Utilization % {(Total spend ÷ Total income) × 100}
- Spend Categories
- Monthly Spend Trends

## Customer Demographics
![p-1](https://github.com/user-attachments/assets/7e8d072e-c510-407c-bf89-dd38086469a4)

Before going to the insights from this page, I would like to note that I have added a new column of **'Income group'** in the Customers table, which is as follows:
- **'Premium'**- Customers with income > 58000;  **'Regular'**- Income range 40000 to 58000;  **'Budget'**- Income < 40000.
- **"40000"** was around the **33rd percentile** of the income range for the entire population, and **"58000"** was around the **60th percentile**.
### Top Insights:
- **25-34 Age group** dominates the customer base with **1498 customers**.(Offers on products for such age group must be increased)
- **45+ Age group** despite having the **highest average income**(48% more than 21-24 age group), is the lowest in count i.e only **13.5% of the customer base**.(Massive untapped opportunity for premium customer aquisition)
- **78.4%** of the customers are **Married**.(More focus on offers/points on familiy friendly products like grocery, dinings, travel,etc)
- **Salaried IT Employees** dominate the customer base(**32%**),and also in the city with highest customers i.e **Mumbai**.
- Most of the **Business Owners and Salaried IT** people come in the **Premium** income group and earn more than 58000 per month.(Big market for premium cards) Whereas most of the **Govt Employees** come in the **Regular** income group i.e between 40k to 58k.
