# Hive-Case-Study
This repository contains code for a machine learning model that can classify images of flowers into different species using deep learning techniques. The model is built using Python and achieves high accuracy on a popular flower dataset.

This project is aimed at analyzing the clickstream data of an e-commerce website using Hive, a data warehousing tool that provides a SQL-like interface to query and analyze large datasets stored in Hadoop Distributed File System (HDFS). The dataset used in this project is a public clickstream dataset of a cosmetics store.

## Project Steps

The project involves the following steps:

1. Copy the dataset from the S3 bucket to the HDFS.
2. Launch an EMR cluster that utilizes the Hive services.
3. Create a database in Hive and create tables to store the data.
4. Load the data from HDFS into the Hive tables.
5. Run optimized queries to extract insights from the data.
6. Drop the database and terminate the EMR cluster.

## Dataset

The dataset consists of two files - "2019-Oct.csv" and "2019-Nov.csv", which contain the clickstream data of the e-commerce store for the months of October and November 2019, respectively. The attributes in the dataset are described below:

- event_time: time of the event (in UTC).
- event_type: type of the event (view, cart, purchase, remove_from_cart).
- product_id: ID of the product.
- category_id: ID of the product category.
- category_code: code of the product category (null for non-promoted products).
- brand: brand of the product.
- price: price of the product.
- user_id: ID of the user.
- user_session: session ID of the user.

## Questions to be Answered

The following questions need to be answered using Hive queries:

1. Find the total revenue generated due to purchases made in October.
2. Write a query to yield the total sum of purchases per month in a single output.
3. Write a query to find the change in revenue generated due to purchases from October to November.
4. Find distinct categories of products. Categories with null category code can be ignored.
5. Find the total number of products available under each category.
6. Which brand had the maximum sales in October and November combined?
7. Which brands increased their sales from October to November?
8. Your company wants to reward the top 10 users of its website with a Golden Customer plan. Write a query to generate a list of top 10 users who spend the most.

## Conclusion

This project aims to test the skills of the Big Data Analysts in Hive and Hadoop concepts. By analyzing the clickstream data of an e-commerce website, this project provides valuable insights into customer behavior and product trends, which can be used to improve sales and customer satisfaction.
