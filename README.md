# bootcamp_Machine-Learning

# Introduction
The goal in this assignment was to build and evaluate several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so I have employed different techniques for training and evaluating models with imbalanced classes. I used the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

# A. Resampling

The libraries that used for this model are imbalanced learn library to resample the LendingClub data and build and evaluate logistic regression classifiers using the resampled data.

## Model Analysis

1. Loaded the Lending Club data, splited the data into training and testing sets, and scaled the features data.

2. **Oversample** the data using the Naive Random Oversampler and SMOTE algorithms below is the printed reports.



3. **Undersample** the data using the Cluster Centroids algorithm.
Over- and under-sample using a combination SMOTEENN algorithm.

## Resampling Conclusion

- SMOTEENN (Combination of Over/Under Sampling) and SMOTE Oversampling has almost the same accuracy score which is slightly better than the other two models.

- Based on these models reports it looks like SMOTEENN has best recal score.

- SMOTE and SMOTEENN has the same geo mean an looks slighly better than other two models.

# B. Ensemble Learning

In this section, I have trained  and compared two different ensemble classifiers to predict loan risk and evaluate each model. Balanced Random Forest Classifier and the Easy Ensemble Classifier.

## Model Analysis

1.  Loaded the Lending Club data, splited the data into training and testing sets, and scaled the features data.

2. **Balanced Random Forest Classifier** printed report.

3. **Easy Ensemble Classifier** Printed report.

## Ensemble Learning Conclusion

- Easy Ensemble Classifier has best balanced accuracy since it is over 90%.
- Easy Ensemble Classifier has higher recal score.
- Easy Ensemble Classifier has higher geo mean score.
- The top three features are ('total_rec_prncp'), ('total_pymnt'), ('total_pymnt_inv').