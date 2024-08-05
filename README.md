# Amazon Sales 

## Overview

In this project, I analyzed data from over 1,000 Amazon products and their ratings to provide insights into sales.

## Dataset

The Amazon product data is sourced from Kaggle (link). It contains various details about the products, including:

product_id: Product ID
product_name: Name of the product
category: Category of the product
discounted_price: Discounted price of the product
actual_price: Actual price of the product
discount_percentage: Percentage of discount for the product
rating: Rating of the product
rating_count: Number of people who rated the product
about_product: Description of the product
user_id: ID of the user who wrote the review for the product
user_name: Name of the user who wrote the review for the product
review_id: ID of the user review
review_title: Short review
review_content: Long review
img_link: Image link of the product
product_link: Official website link of the product

## Project Goals

1) **Categorical Distribution:** Determine the percentage of each product category within the dataset.
2) **Sales Analysis:** Analyze which categories of products have been sold.
3) **Price Comparison:** Compare the prices of products across different categories.
4) **Discount Analysis:** Compare the discount percentages across categories to identify which category has the highest discount rate.
5) **Sales Insights:** Analyze the relationship between ratings and rating counts to gain insights into sales performance.

## Process

Python played a pivotal role in my analysis, allowing for a comprehensive examination of the data and the discovery of key insights. I leveraged several Python libraries to facilitate this process: Pandas for data analysis, Matplotlib for data visualization, and Seaborn for creating advanced visualizations.

## Outcomes

- The values of `discounted_price`, `actual_price`, `discount_percentage`, `rating`, and `rating_count` are of type `str`. Therefore, the first step is to change the data type of these columns.

- I created five rating categories: Very Good, Good, Okay, Bad, and Very Bad. Additionally, I added a new column called evaluation to categorize the ratings.

- The values in the category column have been consolidated from general to specific. I separate the items in this column using the & symbol. The first two columns have no null values; therefore, we focus on these two columns as `cat_1` and `cat_2`.

- Firstly, I analyzed the percentage of products in each category by creating a pie chart. As shown, the largest portion, with 36%, belongs to the Electronics category. The Computers & Accessories and Home & Kitchen categories follow, each accounting for 30%. The remaining six categories each contribute 3% of the total products.

![1](https://github.com/user-attachments/assets/e05bbc02-999e-4e25-8f77-b75160672684)


- 


