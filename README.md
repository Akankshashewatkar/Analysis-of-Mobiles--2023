# Analysis-of-Mobiles--2023
Analysis of Mobile dataset using MySQL and interactive dashboard creation with Power BI.
effectively used MySQL for comprehensive mobile dataset analysis, covering various aspects such as pricing, specific brands, operating systems, and feature support. Your queries provide valuable insights, including identifying the most expensive and cheapest phones, listing top Samsung phones, and categorizing Android and iOS devices based on their prices. The inclusion of 5G support and the total price calculation by brand further enriches the dataset exploration. The incorporation of Power BI for creating an interactive dashboard enhances the visualization and presentation of this insightful mobile dataset analysis.

Analysis of Mobile dataset using MySQL and interactive dashboard creation with Power BI.

Tasks are done using MySQL:

create schema mobile; use mobile; select * from mobile;

-- check mobile features and price list -- select phone_name, price from mobile;

-- Find out the price of five most expensive phones -- select * from mobile order by price desc limit 5;

-- Find out the price of five most chepest phones -- select * from mobile order by price asc limit 5;

-- List of top 5 Samsung phones with price and all features -- select * from mobile where brands = "Samsung" order by price desc limit 5;

-- Must have android phone list then Top 5 high price android phones -- select * from mobile where Operating_System_Type = "Android" order by price desc limit 5;

-- Must have android phone list then Top 5 lower price android phones -- select * from mobile where Operating_System_Type = "Android" order by price asc limit 5;

-- Must have IOS phone list then Top 5 High price IOS phones -- Select * from mobile where Operating_System_Type = "IOS" order by price desc limit 5;

-- Must have IOS phone list then Top 5 Lower price IOS phones -- Select * from mobile where Operating_System_Type = "IOS" order by price asc limit 5;

-- Write a query which phone support 5G and also Top 5 phones with 5G support -- select * from mobile where 5G_Availability = "Yes" order by price desc limit 5;

-- Total price of all mobile is to be found with brand name -- select brands, sum(price) from mobile group by brands;
![Uploading Screenshot (67).png…]()
