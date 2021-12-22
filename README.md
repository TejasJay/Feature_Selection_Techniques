# Feature_Selection_Techniques

![60ecb081507f4559c84381f5_feature-selection-graphic](https://user-images.githubusercontent.com/79327536/147025433-62ccc991-639b-4f68-bd14-500cc8f298ea.png)


When building a machine learning model in real-life, it’s almost rare that all the variables in the dataset are useful to build a model. Adding redundant variables reduces the generalization capability of the model and may also reduce the overall accuracy of a classifier. Furthermore adding more and more variables to a model increases the overall complexity of the model.

## Types of feature selection techniques

### A. Filter methods
Filter methods pick up the intrinsic properties of the features measured via univariate statistics instead of cross-validation performance. These methods are faster and less computationally expensive than wrapper methods. When dealing with high-dimensional data, it is computationally cheaper to use filter methods.
- Variance Threshold
- Correlation Coefficient
- Information Gain
- Chi-square Test
- Fisher’s Score
- Mean Absolute Difference (MAD)

### B. Wrapper methods
Wrappers require some method to search the space of all possible subsets of features, assessing their quality by learning and evaluating a classifier with that feature subset. The feature selection process is based on a specific machine learning algorithm that we are trying to fit on a given dataset. It follows a greedy search approach by evaluating all the possible combinations of features against the evaluation criterion. The wrapper methods usually result in better predictive accuracy than filter methods.
- Forward Feature Selection
- Backward Feature Elimination
- Exhaustive Feature Selection
- Recursive Feature Elimination

### C. Embedded methods
These methods encompass the benefits of both the wrapper and filter methods, by including interactions of features but also maintaining reasonable computational cost. Embedded methods are iterative in the sense that takes care of each iteration of the model training process and carefully extracts those features which contribute the most to the training for a particular iteration.
- LASSO Regularization (L1)
- Random Forest Importance

