# Amazon_Vine_Analysis
Performing analysis on Amazon review data using *PySpark*, *ETL*, AWS RDS, and pgAdmin 

## Overview of Project
Data is considered "Big Data" when it exceeds the capacity of operational databases. *Apache Hadoop* (Hadoop) is one of the most popular open source frameworks, with numerous technologies for big data. Cloud services let us store large amounts of data at remote locations rather than locally on top of many other services. Partnering with an account manager at BigMarket, we used the most popular cloud services available: Amazon Web Services (AWS). For this SellBy project, we analyzed Amazon reviews written by members of the paid Amazon Vine program. We had access to approximately 50 datasets, but picked reviews specifically for the product-- watches. We used *PySpark* to perform the *ETL* process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Afterwards, we used *PySpark* to determine if there is any bias toward favorable reviews from Vine members in the dataset. Last, we wrote an analysis to submit to the SellBy stakeholders. 


## Results

* There were a total of **47** Vine reviews and **8362** non-Vine reviews 
<img width="500" alt="Screenshot (108)" src="https://user-images.githubusercontent.com/107021231/193376477-8af0ba4e-452d-44ae-ab84-b38bb4277d45.png">



* There were **15** Vine reviews (5 stars) and **4332** non-Vine reviews (5 stars) 
<img width="800" alt="Screenshot (110)" src="https://user-images.githubusercontent.com/107021231/193376814-7d95bc7f-c2e2-46a2-821e-bf7723213cbb.png">



* Percentage of Vine reviews (5 stars): **~31.91%** and Percentage of non-Vine reviews (5 stars): **~51.81%** 
<img width="800" alt="Screenshot (111)" src="https://user-images.githubusercontent.com/107021231/193376817-1688fd0f-a9bf-4c37-9423-11aa221a953e.png">



## Summary

Based on the Amazon review data, there are more non-Vine reviewers than Vine reviewers. As a result, although there is also more 5-star non-Vine reviews than 5-star Vine reviews, this could be due to their larger number of total reviews in general. However, based on the percentage, there is about 51% 5-star non-Vine reviews and about 31% 5-star Vine reviews. As a result, we can conlcude that the vine members do not show a bias (positivity bias) towards giving higher ratings depsite being paid to provide those ratings for the products in the watches category. One additional analysis that could be performed with dataset to support this current analysis findings may include extracting the same Vine/non-Vine review data from several other products (eg. grocery, sports, shoes, electronics, etc.) in Amazon to reveal the non-bias in other product categories as well. 
