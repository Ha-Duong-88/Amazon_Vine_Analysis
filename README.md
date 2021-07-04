# Amazon_Vine_Analysis

# Project Overview

Analyze Amazon reviews are written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. This project accessed over 50 Amazon review datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. 

## Scope

The analysis was to determine if there is any bias toward favorable reviews from Vine members for Vine and non-Vine ratings and 5-Star Vine and non-Vine ratings.

This analysis specifically focused on video games reviews. The scope involved creating an Amazon Relational Database Service (Amazon RDS) and S3, using PySpark and Pandas DataFrame in Google Colaboratory Notebook to perform the ETL process to extract the dataset, transform the data, connect to the AWS RDS instance, and load the transformed data into pgAdmin. 

Technologies used for this project were:  Amazon RDS and S3, PySpark, Pandas, SQL, Postgres, pgAdmin, and Google Colaboratory

# Analysis

## Total Vine versus Non-Vine Reviews

    • Total number of revies is 40565

  total_number_reviews.png![total_number_reviews](https://user-images.githubusercontent.com/80140082/124389996-8472ed80-dc9e-11eb-9a98-d30e3ef194b2.png)

    • Total number of Vine reviews is 94
  
  total_count_paid_reviews.png![total_count_paid_reviews](https://user-images.githubusercontent.com/80140082/124390419-69a17880-dca0-11eb-9342-7d77c262bf4a.png)
  
    • Total number of non-Vine reviews is 40471

  total_count_unpaid_reviews.png![total_count_unpaid_reviews](https://user-images.githubusercontent.com/80140082/124390958-f77e6300-dca2-11eb-8ba7-3235a5ac8562.png)


## Total 5-Star Vine Reviews versus 5-Start Non-Vine Reviews 
  
    • Total number of 5-Star Vine (paid) reviews is 48
   
   total_5star_vine_reviews.png![total_5star_vine_reviews](https://user-images.githubusercontent.com/80140082/124390864-5f807980-dca2-11eb-8701-8e36e77e5eb2.png)

    • Total number of 5-Star non-Vine (unpaid) reviews is 15663
  
  total_5star_nonvine_reviews.png![total_5star_nonvine_reviews](https://user-images.githubusercontent.com/80140082/124390935-c56d0100-dca2-11eb-853d-a1b90d65cb7e.png)
  

## Total percent of 5-Star for Vine and 5-Star for non-Vine reviews

    • The percent of 5-Star Vine (paid) reviews is 51.06%
  
  percent_5star_vine_reviews.png![percent_5star_vine_reviews](https://user-images.githubusercontent.com/80140082/124391172-32cd6180-dca4-11eb-930e-be8832dfef02.png)

    • The percent of 5-Star non-Vine (unpaid) reviews is 38.7%
  
  percent_5star_nonvine_reviews.png![percent_5star_nonvine_reviews](https://user-images.githubusercontent.com/80140082/124391503-c0f61780-dca5-11eb-9c4a-42f401a057de.png)


## Summary

This analysis of the Amazon Vine and non-Vine reviews for watches, there is a potential for some positivity bias. The percentage of 5-Star Vine (paid) reviews is 51.05% compared to the 5-Star non-Vine (unpaid) reviews of 38.7%. Given this, there is a 50/50% probability that there could be some positivity bias in the 5-Star Vine reviews. However, additional data analysis would be needed to test and validate this hypothesis.

Paid Vine reviews could influence the positivity of reviews especially if the perentage is significantly high (i.e., significantly greater than 50%). While paid Vine reviews could generate positive reviews, it may not result in a high percentage of 5-Star reviews.

Additional analysis could be performed to determine to if there is any positivity bias for Vine reviews by comparing the 1-Star Vine reviews to the 5-Star Vine reviews. If the 1-Star rating for paid Vine reviews relative to the total non-Vine reviews is low, there may be a positivity bias for the 5-Star paid Vine reviews. Conversely, if the 1-Star rating is high, it is unlikely that there is positivity bias in the 5-Star ratings. We could also do some statistical testing to determine if there is any correlation between paid versus unpaid reviews to predict 5-Star ratings.

