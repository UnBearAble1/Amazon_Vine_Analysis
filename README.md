# Amazon Vine Analysis

## Overview of the analysis

This analysis took publically available reviews for amazon products and used RDS and S3 of amazon web service to extract transform and load the data to narrow in specifically on reviews that were paid through amazon's vine service against reviews that were not paid to determine if there is a bias in the reviews posted for the products. This particular review looked at health and beauty products written in the US region

## Results

To have sufficient data to make the determination of whether there is a bias in the results, the reviews were broken down into two dataframes, one where the results were part of the vine service and one where they were not. The tables were used to determine the total number of reviews, the total number of five star reviews, and then the percentage of reviews that were five star reviews.

The results for those reviews that are part of the vine program are as follows:
![vine_reviews](https://github.com/UnBearAble1/Amazon_Vine_Analysis/blob/main/Vine%20Reviews.png)

The results for those reviews that are not part of the vine program are as follows:
![non-vine_reviews](https://github.com/UnBearAble1/Amazon_Vine_Analysis/blob/main/Non-Vine%20Reviews.png)

## Summary

Based on the above results, it appears that there is a skew towards not rating products at five start for vine reviews. An additional analysis using the available data could further break down the reviews into those that are vine reviews and non-vine reviews that are a verified purchase to see if they more closely align and potentially filter out reviews that are skewed one way or another
