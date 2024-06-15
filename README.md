# Credit_Card_Financial-Report

Credit Card Financial Weekly Dashboard Report


Project Objective:-

To develop a comprehensive credit card weekly dashboard that provides real-time insights into key performance metrics and trends, enabling stakeholders to monitor and analyze credit card operations effectively.

Import data to SQL database

1. Prepare csv file
2. Create tables in SQL
3. import csv file into SQL

Dax Queries :-

AgeGroup = IF('ccdb cust_details'[Customer_Age]>=60,"60 +", 
IF('ccdb cust_details'[Customer_Age]>=50,"50-60",
IF('ccdb cust_details'[Customer_Age]>=40,"40-50",
IF('ccdb cust_details'[Customer_Age]>=30,"30-40",
IF('ccdb cust_details'[Customer_Age]>=20,"20-30")))))


IncomeGroup = IF('ccdb cust_details'[Income]>=70000,"High",IF('ccdb cust_details'[Income]>=35000,"Medium","low"))

week_num2 = WEEKDAY('ccdb cc_details'[Week_Start_Date])

Revenue = 'ccdb cc_details'[Annual_Fees]+'ccdb cc_details'[Total_Trans_Amt]+'ccdb cc_details'[Interest_Earned]


Project Insights:-

Overall revenue is 57M

Total interest is 8M

Total transaction amount is 46M

Male customers are contributing more in revenue 31M, female 26M Blue & Silver credit card are contributing to 93% of overall transactions

TX, NY & CA is contributing to 68%


Credit card financial dashboard using Power Bi:-

Developed an interactive dashboard using

transaction and customer data from a SQL database, to provide real-time insights.

Streamlined data processing & analysis to monitor key performance metrics and trends.

Shared actionable insights with stakeholders based on dashboard findings to support decision-making processes.
