## Amazon_Vine_Analysis

### Overview of the analysis of the Vine program
For this analysis, we are looking at analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

We were given access to 50 datasets and each of them contain reviews of a specific product. The apparel dataset was picked and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 
We also determined if there was any bias towards reviews from the Vine members.

## Results
![results](/image1.png)
* How many Vine reviews and non-Vine reviews were there? </br>
There were 33 Vine reviews and 45388 non-vine reviews 
* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?</br>
15 Vine reviews were 5 stars and 23733 non-vine reviews were 5 stars
* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?</br>
45% of the Vine (paid) reviews were 5 stars and 52% of the non-Viine reviews were 5 stars. 


## Summary
I believe that there is no bias for reviews from the Vine program since the percentage of 5-star reviews is higher for non-Vine reviews. 45% for Vine reviews and 52% for non-vine reviews. 
We can further look for potential bias by looking at the verified_purchase column to see how many of the non-Vine reviews were from customers that purchased the items from Amazon instead of gifted. 
