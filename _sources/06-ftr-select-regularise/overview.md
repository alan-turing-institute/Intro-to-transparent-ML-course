# Feature Selection and Regularisation

<!-- Capitalise initials. As compact as possible, prefer ONE line. -->
<!-- We use **UK** English spelling. -->
<!-- File names should be all lowercase, with words separated by hyphens (-), and no spaces.  Each chapter must include an "overview.md" and "quiz-sum-ref.md"-->

<!-- ```{admonition} Status
Ready for review and feedback
``` -->

```{admonition} Objectives
- Understand the ideas and processes behind several feature selection approaches
- Apply feature selection to reduce the number of features in model construction
- Understand the concepts of overfitting, bias-variance trade-off, and regularisation
- Apply regularisation via ridge/lasso regression to reduce overfitting in model training
```

**Expected time to complete**: 2.5 hours

In this chapter, we will learn about two popular approaches to improve the performance of a machine learning model by reducing its complexity and overfitting: **feature selection** and **regularisation**. [Feature selection](https://en.wikipedia.org/wiki/Feature_selection) is a process of selecting a subset of features from an original feature set. [Regularisation](https://en.wikipedia.org/wiki/Regularization_(mathematics)) aims to reduce the complexity of a model by penalising the (flexibility of) model parameters. Both feature selection and regularisation are useful in reducing the complexity of a model and thus reducing the risk of overfitting.

Feature selection is primarily a machine learning process so we consider its process transparency.

```{admonition} Process transparency: feature selection
- **Starting point**: a standardised dataset for a machine learning task with a performance metric defined and a machine learning model chosen to be trained
- Choose the feature selection method to use (e.g. best subset, forward/backward stepwise, lasso, etc.)
- Determine the model performance metric to use (e.g. mean square error, accuracy, etc.)
- Choose the model selection process (e.g. cross-validation, etc.)
- Compute the performance metric for candidate models with different feature sets
- **End point**: Select the subset of features that gives the best performance metric
```

Regularisation is a technique used in combination with machine learning models. Here, we consider the use of regularisation in {doc}`linear regression <../02-linear-reg/overview>` models and thus consider the system transparency of the regularised linear regression models, which we call ridge regression and lasso regression.

```{admonition} Ingredients: ridge/lasso regression
- Input: features of data samples
- Output: target values of data samples
- Model: fit a line (or plane/hyperplane) to the training data and assign the value on the fitted line (or plane/hyperplane) to the test data
  - Hyperparameter(s): $\lambda$, the weight of the regularisation term
  - Parameter(s): the intercept(s) and slope(s) of the fitted line (or plane/hyperplane), also known as the bias(es) and weight(s), respectively
- Loss function: minimise the sum of 1) the total distances of the training data points to the fitted line (or plane/hyperplane) and 2) the sum of the squares (for ridge) or absolute (for lasso) values of the weights, i.e. the regularisation term
- Learning algorithm:
  - Ridge regression:
    - closed-form analytical solution based on linear algebra, or
    - [Gradient descent](https://en.wikipedia.org/wiki/Gradient_descent): update the weights and intercepts iteratively by solving a _multivariate_ optimisation problem to minimise the loss function
  - Lasso:
    - [Coordinate descent](https://en.wikipedia.org/wiki/Coordinate_descent): update the weights and intercepts iteratively by solving one _univariate_ optimisation problem (for one variable/feature) at a time and successively (alternating between variables/features) to minimise the loss function
```

```{admonition} System transparency: ridge/lasso regression
The same as in {doc}`../02-linear-reg/overview`.
```

<!-- - What input to produce certain output:
- How to produce certain output: -->
