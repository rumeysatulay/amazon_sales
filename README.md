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

![1](https://github.com/user-attachments/assets/e5376671-a6ca-4b27-b5f7-eeaef98887a4)

- I examined the review count. Although the data does not include the number of products sold, we can infer that it is proportional to the number of reviews. In the general categories, the most reviewed products are in Electronics. In the subcategory chart, it is evident that the most reviewed category is Accessories & Peripherals.

![2](https://github.com/user-attachments/assets/70509b3f-5a0b-4ee3-a08d-24199f65c21d)

- I plotted the prices according to both general and subcategories. As shown, Electronics has the highest prices, with a mean price around $120. Home & Kitchen and Car & Motorbike categories follow, with mean prices approximately half of that of Electronics, around $50. The cheapest category is Toys & Games, with a mean price of $1.80. In the subcategories, Laptops have the highest mean price, as expected, at $714.

![3](https://github.com/user-attachments/assets/95fdaa0b-1321-4be9-b2b0-30ca2791e3dc)

- I examined the discount rates of products according to their categories. The highest discount rate is in the Home Improvement category, at 57%. Computers & Accessories follows with a 53% discount rate. Given that Computers & Accessories has the highest prices, a high discount rate is expected in this category. The Toys & Games category shows no discount, which is understandable given the already low prices. In the subcategories, Wearable Technology has the highest discount rate.

![4](https://github.com/user-attachments/assets/15fcf251-0ae0-45af-ac53-0b99b8785bb3)

- I examined the ratings, which are out of five. I created five groups: Very Good, Good, Okay, Bad, and Very Bad. I then created a bar chart to visualize the distribution of product ratings. As shown, there are only six products in the Bad category, with ratings lower than 2 out of 5. The general rating falls into the Good category, meaning ratings are between 4.5 and 4.0. Out of 1,462 products, 1,006 are reviewed in this category.

![5](https://github.com/user-attachments/assets/f6b4a949-83b8-4331-b258-56411f151daa)

- The ratings of the products are also visualized in a histogram plot. We can see that the distribution of product ratings follows a normal distribution.

![6](https://github.com/user-attachments/assets/ee44a375-09e4-4a88-a75e-df4081e8e71d)

- I plotted the relationship between Rating and Review Count, where Review Count is used as a proxy for the number of sold products. The graph illustrates that as the rating increases, both the number of reviews and the number of sold products generally rise. However, there is a noticeable decrease in the number of reviews for ratings above 4.25. This decline could be attributed to several factors, one of which may be the higher price associated with products that receive the highest ratings.

![8](https://github.com/user-attachments/assets/a6d77242-926e-41a9-a7d3-0a7e89d57fa7)


- In these graphs, the distribution of ratings across categories and sub-categories is shown. Although there are no significant differences across the categories, the highest-rated category is Office Products, with a mean rating of 4.31 out of 5. In the sub-categories, Tablets have the highest rating, with a score of 4.6 out of 5.

![7](https://github.com/user-attachments/assets/50a4ca22-04be-4b22-90b6-4df4075d9e31)
