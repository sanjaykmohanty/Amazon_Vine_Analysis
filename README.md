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
The results suggest that Vine members did only 16 reviews out of which 20 are 5-star reviews, which translates to about 33% of 5-star reviews. Whereas Non-Vine members did 28,287 revies out of which 15,689 are 5-star reviews, which translates to 55% of 5-star reviews. 

Based on the results, one could conclude that Vine members did not show bias when rating their products. The number of 5-star ratings by the Vine members was about 22% less than non-Vine members (33% vs. 55%). 

Although it seems like Vine customers are more critical when submitting their review, to reach a conclusion, all data should be included rather than filtering the data to a percentage of helpful vs. total votes. Reviewing all the data available in the dataset would give more insight to the reviews. As shown below, the Vine members' 5-star rating is at 34% but the non-Vine members' 5-star ratings is at 69%. The analysis supports the claim that there is no bias in Vine members' review ratings. 

![image](https://user-images.githubusercontent.com/31812730/209476761-101d8ffe-f813-4d01-b8d6-ab4eb3eaaa2a.png)

This analysis is done solely on the US Grocery data. Similar analysis can be done on all other available datasets to understand if there is bias for any specific products, or the no bias claim is true across the board.


