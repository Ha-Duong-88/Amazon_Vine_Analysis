# Amazon_Vine_Analysis

# Project Overview

Analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. 

## Scope
This project accessed approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. The scope involved using PySpark, perform  the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin, and PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset.

Technologies used for this project were:  Amazon Relational Database (RDS), PySpark, Pandas, SQL, Postgres, pgAdmin, Google Colab

# Analysis


How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
Based on the analysis of the Amazon Watch Reviews data, the following results were observed:

## Total Vine versus Non-Vine Reviews
  
  •	Total number of revies is 40565

  total_number_reviews.png![total_number_reviews](https://user-images.githubusercontent.com/80140082/124389996-8472ed80-dc9e-11eb-9a98-d30e3ef194b2.png)

  •	Total number of Vine reviews is 94
  
  total_count_paid_reviews.png![total_count_paid_reviews](https://user-images.githubusercontent.com/80140082/124390419-69a17880-dca0-11eb-9342-7d77c262bf4a.png)

  •	Total number of non-Vine reviews is 40471

  total_count_unpaid_reviews.png![total_count_unpaid_reviews](https://user-images.githubusercontent.com/80140082/124390958-f77e6300-dca2-11eb-8ba7-3235a5ac8562.png)


## Total 5-Star Vine Reviews versus 5-Start Non-Vine Reviews 
  
   •	Total number of 5-Star Vine (paid) reviews is 48
   
   total_5star_vine_reviews.png![total_5star_vine_reviews](https://user-images.githubusercontent.com/80140082/124390864-5f807980-dca2-11eb-8701-8e36e77e5eb2.png)


  •	Total number of 5-Star non-Vine (unpaid) reviews is 15663
  
  total_5star_nonvine_reviews.png![total_5star_nonvine_reviews](https://user-images.githubusercontent.com/80140082/124390935-c56d0100-dca2-11eb-853d-a1b90d65cb7e.png)

  
  * The percent of five-Star reviews of the total paid Vine reviews is 51% and unpaid vine reviews is 38%

There may be positivity bias for the 5-star reviews given that five-star paid Vine reviews percent is 51% compared to the unpaid Vine reviews. However, more data and analysis would be needed to test and validate this.

An additional analysis that could be performed is to compare the 1-star reviews for any negativity bias and compare them to the 5-star paid reviews. Instead of filtering by 1 instead of 5 in this case. If the 1-Star rating for paid Vine reviews relative to the total Vine (paid and unpaid) reviews is low, there may be a positivity bias.

Below is an image of the Spark code:

![vine_review_analytics](https://user-images.githubusercontent.com/80140082/124366474-ff87c580-dc04-11eb-8e6e-bda2b93af3a8.png)
