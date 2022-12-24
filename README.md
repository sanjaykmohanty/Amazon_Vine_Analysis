# Amazon Vine Analysis

## Overview
The purpose of this project is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program allows manufacturers and publishers to receive reviews for their products. 

In this project, we picked reviews on US groceries and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 

We used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. A summary of the analysis is included in this report which can be submitted to the stakeholders.

## Resources
- **Data Source:** [Amazon Review dataset, US Grocery Review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Grocery_v1_00.tsv.gz)
- **Software:** Google Colab Notebook, PostgreSQL 13, pgAdmin 6, AWS

## Results

![image](https://user-images.githubusercontent.com/31812730/209446525-8b6ef1e4-4ff0-4035-9290-3f0ecf90b40c.png)


![image](https://user-images.githubusercontent.com/31812730/209446505-b715123d-4f7b-4f40-9543-bf89afc5152b.png)

## Summary
51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%. This describes a positivity bias for reviews in the Vine program.
Additionally we could analyse the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.
