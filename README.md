# Data aggregation and analysis for supermarket transactions_project for commonwealth bank data science Job simulation
## Overview
The data set is a csv file named “supermarket_transactions.csv.” it contains three years of transactional data that was collected from supermarkets across Australia. 
Analysis was needed to ask the following questions:
* Across locations, how many apples were purchased in cash?
* How much total cash was spent on these apples?
* Across all payment methods, how much money was spent at the Bakershire store location by non-member customers?
## Aggregation and Analysis
In other to answer the questions above, the datasheet was filterered to aggregate the dataset based on categories required and formulas were used to get the summation

Question 1: Across locations, how many apples were purchased in cash?

To answer this question, the data sheet was filtered to include only rows where the
`product_name` is “apple” and where the `payment_method` is “cash.” Then, the
`quantity` column was summed to get an answer of 117 apples,  with the formula (=SUBTOTAL(9,D23744:D23814))

Question 2: How much total cash was spent on these apples?

Here, the data sheet was filtered to include only rows where the `product_name` is “apple” and where the `payment_method` is “cash.” Then, the `total_amount` column wwas summed to get an answer of $537.03, with the formula (=SUBTOTAL(9,H23744:H23814))

Question 3: Across all payment methods, how much money was spent at the Bakershire store location by non-member customers?

For this question, the previous filter criteria was all cleared. Then,  the data sheet was filtered to include only rows where the `customer_type` was non-member, and the `store` was Bakershire. Then,  the `total_amount` column was summed to get an answer of $2,857.51, with the formula  (=SUBTOTAL(9,H113:H50495))
