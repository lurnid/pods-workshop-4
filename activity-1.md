
# W4 Workshop activity 1: Building a logistic regression model

**In this workshop activity, you'll practise creating a logistic regression model using loans data from a banking scenario.**

Here's the scenario:

- You work for a bank as a data scientist. One of the products that they have on offer is personal loans.​
- The bank has data on previous loans sold. While most people repaid the loan, some defaulted.​
- The bank obviously wants to minimise the amount of loans they agree to that are defaulted.
- You have been tasked with creating a model to help in this process.​

The problem

- Loan data for every customer who borrowed £1000 for 12 months.
- Examples/cases = row = single customer/loan.
- Features = columns = fields = characteristics of customer/loan.
- Target: The characteristic/column you're trying to predict/understand.
- Problem: What model best describes the relationship of the features to the target?

**Step 1:** Learn pattern (model) from data which describes a features relationship to target.

**Step 2:** Use pattern to guess unknown target from known features.

### Load the data

Load the following libraries:

- numpy
- pandas
- seaborn
- matplotlib
- scikit-learn

Load the following data file into a DataFrame:

- **csv** (available in the next step on Canvas)

### Familiarise yourself

Familiarise yourself with the dataset. Seek to understand:

- types of data.
- distributions of features.
- obvious patterns.
- errors, nulls, outliers.

### Prepare the data

Prepare the dataset for modelling by performing the following steps:

1. Remove or impute null values (with justification).
2. Encode the target variable using `LabelEncoder`.
3. Encode categorical features using either `OrdinalEncoder` or `pd.get_dummies()` (with justification).
4. Decide whether to scale (normalise/standardise) numeric features.
5. Split the data into training and testing sets.

Building your first model

1. Create a logistic regression model using
   `LogisticRegression()` from `sklearn.linear_model`

2. Fit the model on
    ```
    X_train
    ```
    and
    ```
    y_train
    ```

3. Generate predictions from the model for
    ```
    X_test
    ```
    using the **predict** method, storing them in the variable
    ```
    y_pred
    ```
