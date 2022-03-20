# Amazon_Vine_Analysis
- In this project, a complete ETL process has been performed in the AWS cloud platform and uploaded DataFrame to an AWS RDS instance. PySpark has been used to perform a statistical analysis of reviews of electronics items sold on Amazon.
- Analyzing Amazon reviews written by members of the paid Amazon Vine program.

## Overview
The purpose of the project is to analyze Amazon reviews written by members of the paid Amazon Vine program. In order to complete this analysis, I used a subset of data that pertained to the video game subcategory of Amazon. I then performed an ETL on this data by using AWS, Google Colaboratory, PostgreSQL, and PySpark. After taking closer look at one of the tables I made during the ETL phase regarding the vine reviews to determine if there was any positivity bias for reviews in the Vine Program.

### Results

Several quetions arose,  what percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- 51.06% of paid reviews are 5-stars and 38.7% of unpaid reveiws are 5-stars.
percentage_5_stars.

![percentage_paid](./Resources/percentage_paid_5.png)

![percentage_unpaid](./Resources/percentage_unpaid_5.png)

Below are the Results from SQL Queries:

![review_table](./Resources/review_id_table.png)

![products_table](./Resources/products_table.png)

![customers_table](./Resources/customers_table.png)

![vine_table](./Resources/vine_table.png)

## Summary
After looking that the results, I would conclude that there is a positivity bias for reviews in the Vine program:
- to note that while the non-vine sample size was very large, the vine sample size was less than 100 entries. 
- In addition to the current analysis, I could take it a step further and see the percentage of those who purchased the product by filtering through the verified_purchase column to either confirm or fail to confirm if there is bias for reviews in the Vine program.
