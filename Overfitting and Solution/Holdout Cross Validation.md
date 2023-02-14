# Holdout Cross Validation

Spitting data into `training set` and a `test set`, such that learing happens on the training set and is evaluated on the test set<br>
This is another approach to solve overfitting in out model, where we actually check whether our model can generalize the future data points.<br>
in case of overfitting, we are likely to observe that our test set are not getting generalized very well based on our hypothesis

## k - fold Cross Validation 
* Rather than dividing the data points into 2 sets
* We try k different training and test sets and this experimenting k times.
* k different results
* often times, we then take the average of all the results
* scikit-learn
