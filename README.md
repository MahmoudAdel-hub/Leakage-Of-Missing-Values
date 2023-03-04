# Leakage Of Missing Values

Missing values leakage occurs when missing values in the dataset are imputed (i.e., filled in with a substitute value) before splitting the dataset into training and test sets. If this is done incorrectly, it can lead to data leakage, where information from the test set leaks into the training set, resulting in overly optimistic performance estimates.

The correct approach is to impute missing values separately for the training and test sets, using only information from the respective sets. This ensures that the imputed values in the test set are not influenced by information from the training set. One common method for doing this is to use the mean or median value from the training set to impute missing values in both the training and test sets. Another approach is to use more sophisticated imputation methods, such as k-nearest neighbors or multiple imputation, that take into account the relationships between the variables in the dataset.
