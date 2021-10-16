# Amazon Reviews

## Purpose of Analysis
###
The purpose of this analysis is to determine if there is a bias in paid Amazon reviews as compared to unpaid Amazon reviews.  Using PySpark, ETL process was completed on the database https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Electronics_v1_00.tsv.gz.  The analysis looks at number of 5 star reviews for paid vs. unpaid reviews and the percentage of the the reviews that are deemed helpful to determine if there is an underlying bias.

## Results
###
For the paid Vine reviews there were a total of 261 product reviews, of which 106 products received a 5 star review.  This means 40.6% of the paid product reviews were give a 5 star review.  

![image](https://user-images.githubusercontent.com/86161212/137602121-b98ecb6b-d46d-464e-9139-577f5de03fa7.png)


For the unpaid reviews there were a total of 24,040 product reviews.  Of the unpaid reviews, 10,899 product reviews received a 5 star rating.  This is a total of 45.3% of product reviews.

![image](https://user-images.githubusercontent.com/86161212/137602139-6f929d8e-5668-40b6-b63e-13ab833e7bee.png)

- Total reviews: 24,301. 261 Vine reviews, 24,040 non-Vine reviews
- Total 5 star ratings: 11,005. 106 Vine reviews, 10,899 non-Vine reviews
- Percentage of Vine 5 star reviews: 40.6%.  Percentage of non-Vine 5 star reviews: 45.3%

Unpaid product reviews received 4.7% more 5 star reviews as compared to paid product reviews.

## Conclusion
###
The analysis of 5 star Amazon review ratings examined product reviews in which a minimum of 50% of the reviews were voted as "helpful".  Of the the 24,301 reviews that received a minimum 50% helpful rating, only 261 were written by Vine reviews.  99% of the 24,301 helpful product reviews were written by non-paid reviewers.  Although the unpaid reviews granted a slightly higher 5 star review to products, it is difficult to assess any bias as the pool of helpful paid reviews is so small. In total, the Electronics database has 705,889 reviews, only 106 were rating as helpful Vine reviews, while 10,899 were rate as helpful non-Vine reviews.  Overall non-Vine reviews are rated as more helpful than Vine reviews in this category, and while there were 4.7% more 5 star reviews of products, as the sample size is much greater

![image](https://user-images.githubusercontent.com/86161212/137603139-fc9e58bd-4f46-4e2b-9a40-7fc78be0a4a7.png)

