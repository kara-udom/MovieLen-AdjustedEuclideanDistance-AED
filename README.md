# MovieLen-AdjustedEuclideanDistance-AED
## Project Overview
This project evaluates the performance of a new similarity measure — Adjusted Euclidean Distance (AED) — within a User-Based Collaborative Filtering (K-Nearest Neighbour) recommendation system.
The objective is to compare AED against traditional similarity measures (e.g., Pearson Correlation) and assess performance using evaluation metrics such as MAE and RMSE.

## Dataset
In this report uses MovieLens data sets which were collected by the GroupLens Research Project at the University of Minnesota from September 19th, 1997 through April 22nd, 1998. This data set consists of: 100,000 ratings (1-5) from 943 users on 1682 movies.
### Part 1 : Set up and Install
Install necessary packages such as pandas and numpy. Then load Movies Lens by read_csv 'ml-100k/u.data' sperated list by tabs user id | item id | rating | timestamp.
### Part 2.1 : Training dataset
Use train_test_split to split training set into 80% and test set 20%. Training Dataset will be considered as
two dimension matrix and compare each user with other users by using itertuples(), train_ds will be divided portion to 80% of total dataset
### Part 2.2 : Testing dataset
Testing dataset considered as two dimensional and use itertuples for each data rows. test_ds will be divided portion to 20% of total dataset.
### Part 3: Implement AED Similarity Measure
Implemented a custom similarity measure: Adjusts traditional Euclidean distance, Accounts for user rating behavior, Designed to improve similarity accuracy in sparse datasets
### Part 4: Implement user based
For comparison, the traditional approach was implemented: Compute Pearson Correlation Coefficient, Identify K-nearest neighbours, Generate rating predictions, Evaluate model performance
## Comparison and Conclusion
The User-based method, in this case, appears to perform better than the AED method in terms of both MAE and RMSE.
As a result, the AED method in this report need to be improvement in the future to ensure all of formula applied correctly.

### Reference
Data set - F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4, Article 19 (December 2015), 19 pages.
DOI=http://dx.doi.org/10.1145/2827872