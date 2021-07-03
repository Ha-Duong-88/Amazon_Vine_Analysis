# Amazon_Vine_Analysis

# Project Overview

Analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. 

## Scope
This project accessed approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. The scope involved using PySpark, perform  the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin, and PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset.

Technologies used for this project were:  Amazon Relational Database (RDS), PySpark, Pandas, SQL, Postgres, pgAdmin, Google Colab

# Analysis
Based on the analysis of the Amazon Watch Reviews data, the following results were observed:

  * There are a total 94 paid Vine reviews and 40471 unpaid Vine reviews.
  * There were a total of 48 paid and 15663 of unpaid 5-Stars reviews.
  * The percentage of 

The percent of five-star reviews of the total paid vine reviews is: 51.06382978723404 %


What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

Below is an image of the Spark code:

![vine_review_analytics](https://user-images.githubusercontent.com/80140082/124366474-ff87c580-dc04-11eb-8e6e-bda2b93af3a8.png)
