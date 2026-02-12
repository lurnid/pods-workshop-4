# W4 Workshop activity 2: Building a decision tree

**In this workshop activity, you'll practise building a decision tree and random forest.**

To create your decision tree, follow these steps:

1. Using the same approach as in Activity 1, build a decision tree using:
   `DecisionTreeClassifier(max_depth=2, min_samples_leaf=20)` from `sklearn.tree`
2. Fit the model on your training data.
3. Plot the tree using the code below:
   ```python
   from sklearn import tree
   from matplotlib import pyplot as plt

   fig = plt.figure(figsize=(25, 15))
   tree.plot_tree(dt, feature_names=X_train.columns, class_names=['Settles', 'Defaults'], filled=True)
   ```

### Extension activity: Building a random forest

1. Using the same approach as above, build a random forest using:
   `RandomForestClassifier(n_estimators=30, min_samples_leaf=10)` from `sklearn.ensemble`
2. Fit the model on your training data.
