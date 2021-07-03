# Amazon_Vine_Analysis

# Project Overview

Analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. 

## Scope
This project accessed approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. The scope involved using PySpark, perform  the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin, and PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset.

Technologies used for this project were:  Amazon Relational Database (RDS), PySpark, Pandas, SQL, Postgres, pgAdmin, Google Colab

# Analysis
Based on the analysis of the Amazon Watch Reviews data, the following results were observed:

  * There are a total 94 paid Vine reviews and 40471 unpaid Vine reviews.
  * There were a total of 48 5-Star paid and 15663 of unpaid 5-Star reviews.
  * The percent of five-Star reviews of the total paid Vine reviews is 51% and unpaid vine reviews is 38%

There may be positivity bias for the 5-star reviews given that five-star paid Vine reviews percent is 51% compared to the unpaid Vine reviews. However, more data and analysis would be needed to test and validate this.

An additional analysis that could be performed is to compare the 1-star reviews for any negativity bias and compare them to the 5-star paid reviews. Instead of filtering by 1 instead of 5 in this case. If the 1-Star rating for paid Vine reviews relative to the total Vine (paid and unpaid) reviews is low, there may be a positivity bias.

Below is an image of the Spark code:

![vine_review_analytics](https://user-images.githubusercontent.com/80140082/124366474-ff87c580-dc04-11eb-8e6e-bda2b93af3a8.png)
