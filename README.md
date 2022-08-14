# Amazon_Vine_Analysis

## Overview of the analysis:
The purspose is to determine if there´s any type of bias among reviews such that Vine members favor the scores of reviews over other type of reviews.

I used the video games list of reviews from Amazon in the US,but any list could have been used from this [site](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt).

I used PySpark to connect to AWS RDS and send finished data to PgAdmin.

## Results: 
* How many Vine reviews and non-Vine reviews were there?
We had 94 non-paid reviews and 40471 paid reviews as shown in the image:
![Picture1](https://github.com/karen-trena/Amazon_Vine_Analysis/blob/main/Picture1.png)

* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
We had 48 paid 5-star reviews and 15663 non-paid 5-star reviews:
![Picture2](https://github.com/karen-trena/Amazon_Vine_Analysis/blob/main/Picture3.png)

* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
We had 51% paid 5-star reviews and 39% unpaid 5-star reviews
![Picture3](https://github.com/karen-trena/Amazon_Vine_Analysis/blob/main/Picture4.png)


## Summary:
Data is skewed positively towards Vine reviews as seen above. I´m sure that if we make a hypotesis test over this percentages we would get there´s a statisical difference over these proportions.
Additionally, we could also check the median and make a hypothesis test over means instead of proportions.

