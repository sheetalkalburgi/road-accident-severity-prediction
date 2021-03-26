# Road Accident Severity Prediction

- There are a total of 75550 rows and 33 columns in the original dataset.
- Upon analysis we determined that there are 15 numerical features, out of them only 5 are continuous.
- Discrete numerical features are treated as categorical features and label encoded along with the categorical features, making total number of categorical features as 25.
- From the list of features, Accident_Index and Datetime columns are dropped as they were more of an identifier for the record, rather than an attribute.
- The entire dataset was divided using 60-15-25 (train/validation/test) split.
-  Total of 4 classifiers are created and stacking ensemble method is employed to build our classifiers.
- The classification accuracy on the test data for both the SVC and NN classifier were comparable, with SVC marginally performing better.
- Naïve Bayes classifiers, both mixed Naïve Bayes and Categorical Naïve Bayes accuracy was less than SVC and NN. However, Categorical Naïve Bayes performed slightly better than mixed Naïve Bayes which makes us think that the continuous features may not be useful predictors.
- Stacking the classifiers, did not improve the accuracy on the classification set, which is obvious since the performance of individual classifiers is comparable or almost similar.
- SVC model is the best model as it has the highest performance of 75.06% on the test data.
