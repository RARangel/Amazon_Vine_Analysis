# Amazon_Vine_Analysis

## Overview

The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

This project analyzes the Amazon Music Reviews with the following method:
- Uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 
- Uses PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. 
- Summarizes the analysis to submit to the SellBy stakeholders.

### Deliverables

Deliverable 1: Perform ETL on Amazon Product Reviews    [file](Amazon_Reviews_ETL.ipynb)  
Deliverable 2: Determine Bias of Vine Reviews    [file](Vine_Review_Analysis.ipynb)   
Deliverable 3: A Written Report on the Analysis (README.md)

### Analysis

- There were a total of 7 Vine reviews and 105979 non-Vine reviews (105986 total).
- No Vine reviews gave 5 stars, whereas 67580 non-Vine reviews were 5 stars.
- Total percentages:  (0%) of Vine reviews were 5 stars.  (64%) of non-Vine reviews were 5 stars.

![image](https://user-images.githubusercontent.com/98564776/169737624-2e2687b3-3dda-4f1a-896e-5bef115d5900.png)


### Summary

In summary, there is a bias towards no 5 stars for reviews in the Vine program. The numbers also point towards the fact that non-Vine numbers are more likely to review music. For further analysis, the columns review_headline and review_body could shed light on the basis of ratings.
