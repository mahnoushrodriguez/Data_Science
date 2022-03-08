# Data Science Mini Projects

This repo contains a few samples codes mostly related to ecommrce and online marketing.

<strong>Customer Cohort Analysis</strong>

Project description:</br>
We would like to create customer cohorts based on purchase history. This [cohort analysis](https://en.wikipedia.org/wiki/Cohort_analysis) allow us to track their purchasing behavior, analyze the results and customize our strategies and offerings accordingly.

Notebook: Cohort_Analysis_mini_project.ipynb

[Customer Cohort Analysis](Desktop/cohort_analysis.jpg)

Content:

1. Importing required libraries
2. Loading the data
3. Data Cleaning & Preperation
   1. Handling duplicates
   2. Handling missing values
   3. Handling returned orders
   4. Combining order line items
4. Cohort Analysis
   1. Creating customer & order cohorts
   2. Creating cohort dataframe
   3. Creating cohort matrix
   4. Building cohort generator function
   5. Exploring cohorts

RFM Modeling with K-Means

1. Importing required libraries
2. Loading the data
3. RFM Modeling
   1. Recency
   2. Frequency
   3. Monetary Value
   4. Exploring RFM distribution
4. RFM Modeling with quartile binning
   1. Building quartile based RFM generator function
   2. Exploring the quartile based RFM model
5. RFM Modeling with K-Means
   1. Log transformation of the data
   2. Scaling the data
   3. Transformed data visualization
   4. Calculating optimal number of clusters
   5. Buliding K-Means based RFM generator function
   6. Using the functions
   7. Labeling clusters

A/B Testing Ad Performance

1. Importing required libraries
2. Loading & cleaning the data
3. Two-sided A/B Testing
   1. Formulating the hypothesis
   2. Solution1: Normal Approximation Method
      1. Building z test function
      2. Alternative solution: using statsmodels
   3. Solution 2: Chi-Squared Test
      1. Creating a two-way contingency table
      2. Building chi-squared test function
      3. Alternative solution: using scipy
   4. Solution3: Randomization Test (Resampling)
   5. Two-sided Hypothesis Testing Conclusion
4. One-sided Hypothesis Testing
   1. Hypothesis test using approximation method
   2. Hypothesis test using chi-squared test
   3. Hypothesis test using resampling
   4. One-sided Hypothesis Testing Conclusion
5. Practical significance

Customer Lifetime Value & Segmentation for ecommerce

1. Importing required libraries
2. Data loading & preperation
3. Using BG/NBD Model to predict the number of orders
   1. Calculating RFM metrics
   2. Fitting the BG/NBD model without Train_Test Split
      1. Recency Frequecy Matrix
      2. Probability Alive Matrix
      3. Customer Ranking
   3. Fitting the BG/NBD model with Train_Test Split
      1. Customer Purchase Predictions
      2. Model tuning
   4. Customer Probability History
4. Estimating Customer Lifetime Value (CLV)
   1. Gamma-Gamma model to predict customers monetary values
      1. Preparing data
      2. Fitting Gamma-Gamma model
      3. Predicting Average Order Value per customer (AOV)
   2. Predicting expected number of orders per customer using BG/NBD
   3. Predicting CLV per customer using gamma-gamma model
5. Segmenting repeat customers based on CLV
   1. Bucket Segmentation
      1. Segmentation using quantiles
      2. Segmentation using custom bins
   2. K-means customer segmentation
