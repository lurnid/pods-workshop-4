# W4 Workshop activity 2: Building a decision tree

**In this workshop activity, you’ll practise building a decision tree and random forest.**

To create your decision tree, follow these steps:

1. Using the same approach as in Activity 1, build decision tree using:  
   `decision_tree(mode = "classification", min_n = 20)`
   with the following.
2. Fit the model using use: 
   `set_engine(“rpart”)`
   and fit.
3. Using this code below, plot the tree:  
   ```
   library(rpart.plot)`
   rpart.plot(decision_tree_fit$fit)
   ``` 

### Extension activity: Building a random forest

1. Using the same approach as above, build a random forest using:  
   `rand_forest(mode = "classification", trees = 30, min_n = 10)`
2. Fit the model using use:  
   `set_engine(“rpart”)` 
   and fit.

