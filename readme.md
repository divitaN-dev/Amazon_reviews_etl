## Overview of Project

### Purpose

* Amazon product sales are often determined by positive reviews of a given product. Using a reviews dataset of Kitchen products, an ETL (Extract, Tranform, Load) process is perfomed using the Relational Database (RDS) service of Amazon Web Services. 
The data extraction and tranformation is done using PySpark in Google co-lab environment. The tranformed dataset with insights drawn is then loaded into a Postgres data via an AWS connection.
A promotional program Vine is often used to incentivise customers to write product reviews, therefore a comparison between vine program reviews and regular reviews is also performed to check for any possible bias.


## Results

* The total number of Vine and non-Vine reviews are summarised as follows -
    * Vine reviews - 1207
    * Regular reviews - 97,839

![total-reviews](https://github.com/divitaN-dev/Amazon_reviews_etl/blob/main/img/total_reviews.png)


* The total number of Vine and non-Vine reviews that were at 5-stars are summarised as follows- 
    * 5-star Vine reveiws - 509
    * 5-star regular reviews - 45,858

![5-star-reviews](https://github.com/divitaN-dev/Amazon_reviews_etl/blob/main/img/total-5-stars.png)

* The total number of Vine and non-Vine reviews as a percentage of total vine and regular reviews are summarised as follows- 
    * 5-star Vine reviews as a percentage of total Vine reviews- 42.17%
    * 5-star regular reviews as a percentage of total regular reviews - 46.87%
    
![vine-reviews-percent](https://github.com/divitaN-dev/Amazon_reviews_etl/blob/main/img/reviews-percent.png)


###Summary

* There doesn't seem to be a significant poistive bias when customers are incentivised to write reviews as a part of the vine program; since the comparison of 5-star reviews differs by just 4.7% for vine and non-vine reviews.
However, further analysis for significance may be needed when the number of reviews go beyond an established threshold, since many amazon products tend to sell hundreds of thousands in quantitites.

* Since the current dataset also contains significantly larger numbers of regular reviews - 97,839 and a meager 1,207 reviews of vine reviews, a further analysis of products with a better balance between vine and non-vine reviews will provide more conclusive insights.

