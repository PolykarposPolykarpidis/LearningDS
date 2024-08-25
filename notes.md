# Cross-validation and/vs Stratified Sampling

Cross-validation and stratified sampling are two important concepts in machine learning, and they're often used together to evaluate the performance of models. Let's break them down:

**Cross-validation:**

Cross-validation is a resampling technique used to evaluate the performance of a machine learning model on unseen data. The goal is to estimate the model's performance on a new, independent dataset.

Here's how it works:

1. Divide your dataset into k folds (e.g., 5 folds).
2. For each fold, use the other k-1 folds as the training set and the remaining fold as the validation set.
3. Train the model on the training set and evaluate its performance on the validation set.
4. Repeat this process for each fold, so you have k iterations.
5. Calculate the average performance across all folds.

Cross-validation helps you avoid overfitting by providing a more realistic estimate of your model's performance on unseen data. It's particularly useful when you have a small dataset or want to estimate the model's performance on new data.

**Stratified sampling:**

Stratified sampling is a technique used to ensure that the samples in your dataset are representative of the underlying population. It's particularly useful when you're working with imbalanced datasets (e.g., class imbalance).

Here's how it works:

1. Identify the class or categorical variable you're interested in (e.g., response variable).
2. Divide your dataset into subsets based on this class or categorical variable.
3. For each subset, calculate the proportion of instances in each class.
4. Sample instances from each subset according to these proportions, so that the sampled dataset is representative of the original dataset.

Stratified sampling helps you avoid biased results when working with imbalanced datasets. By ensuring that your samples are representative of the underlying population, you can get more accurate estimates of your model's performance.

**Combining cross-validation and stratified sampling:**

When you're working with imbalanced datasets, it's common to use stratified sampling to create a balanced dataset. Then, you can use cross-validation to evaluate the performance of your model on this balanced dataset.

For example, let's say you're working with a classification problem where one class has 10% of the instances, and the other class has 90% of the instances. You can use stratified sampling to create a balanced dataset with 50% of each class. Then, you can use cross-validation to evaluate the performance of your model on this balanced dataset.

By combining cross-validation and stratified sampling, you can get a more accurate estimate of your model's performance on unseen data, while also ensuring that your samples are representative of the underlying population.

# Define the regression problem
- Singular regression problem vs Multiple regression problem (see the num of predictors)
- Univariate regression problem vs Multivariate regression problem (see the num of predicted values)
- Batch learning vs Online learning.

# Performance measure
