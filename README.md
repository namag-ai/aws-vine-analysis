# Amazon Vine Analysis
Performing ETL with AWS and Google COllab



## Overview of the analysis: 
The purpose of this projects is to discover whether there is any bias toward favorable reviews from Vine members regarding Outdoors products in Amazon Vine program.
I am utilizing PySpark and Pandas for ETL process then using RDS as well as S3 via Amazon web Service to load the cleaned data into pgAdmin and create variety of metrics. 

## Resources 

* [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
* [Colab Notebooks](https://colab.research.google.com/drive/1a_gBZ-A1EywymsrAJ79mAU9WeOl5Tdr-?usp=sharing)

## Results

#### Total number of reviews

* Vine Review: Upon eliminating numbers of Non Vine review, there are 107 was member of paid Vine program .

<img  alt="Screen Shot 2022-05-07 at 5 09 02 PM" src="https://user-images.githubusercontent.com/98676400/169712778-b7f5232c-e17d-4643-9189-4e04f1456502.png"> 

* Non Vine reviews: Once 107 paid member removed from total review , 39,869 review was from Non Vine program .


<img  alt="Screen Shot 2022-05-07 at 5 09 02 PM" src="https://user-images.githubusercontent.com/98676400/169712836-eb10422e-05a1-4818-81dd-e170995b2f79.png"> 

#### Total number of 5 stars reviews

* 5 stars Vine Review: 5 star reviews that comes from member of Vine program is 56 . 

<img  alt="Screen Shot 2022-05-07 at 5 09 02 PM" src="https://user-images.githubusercontent.com/98676400/169712951-6a19f2ac-1590-45df-b508-6f3242886c99.png"> 

* 5 stars Non Vine Review: 5 star reviews that comes from  Non Vine program is 21,005 . 

<img  alt="Screen Shot 2022-05-07 at 5 09 02 PM" src="https://user-images.githubusercontent.com/98676400/169713005-bdcb3773-bfc7-4474-a251-98d5b7fa96ba.png"> 


#### Percentage of 5-star reviews

* Percent of 5 star Vine reviews: 52.34 %
* Percent of 5 star Non Vine reviews: 52.69 %


# Summary

As we can see from the percentage of <strong>5-star reviews</strong>, there is an insignificant difference between Vine and Non Vine 5 star reviews as <strong>.35%</strong>. Therefore, I would conclude that there is no obvious positive bias for revies in the Vine program. 
In order to have better idea on biasness, one can create a Hypothesis Testing and see there is any difference between mean of sampling and the population to provide more evidence and reject or fail to reject the Hypothesis. In addition to this, analyzing the other datasets available on Amazon Review Datasets and compare <strong>1-star</strong> reviews as well as <strong>5-star</strong> reviews  would be helpful to discover any biasness.










