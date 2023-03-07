# Trees and Ensembles

<!-- Capitalise initials. As compact as possible, prefer ONE line. -->
<!-- We use **UK** English spelling. -->
<!-- File names should be all lowercase, with words separated by hyphens (-), and no spaces.  Each chapter must include an "overview.md" and "quiz-sum-ref.md"-->

<!-- ```{admonition} Status
Ready for review and feedback
``` -->

```{admonition} Objectives
- Understand decision trees for regression and classification.
- Apply decision trees to real-world problems and interpret the results.
- Understand bagging, random forests, and boosting for ensemble-based learning.
- Apply ensemble learning to real-world problems and interpret the results.
```

**Expected time to complete**: 3 hours

In this chapter, we will study classification and regression models that are based on trees and ensembles. These models are very popular in practice, and are used in a wide range of applications. We will start with [decision trees](https://en.wikipedia.org/wiki/Decision_tree), which are the simplest form of tree-based models. We will then study bagging, random forests, and boosting, which are ensemble learning methods that combine multiple decision trees or other models to improve their performance.

Tree-based models involve dividing (stratifying, segmenting) the feature space into a number of simple regions, and then making a prediction for each region. This is in contrast to linear models, which involve fitting a single linear function to the data. The main advantage of tree-based models is that they are very easy to **interpret**. The main disadvantage is that they are prone to overfitting, and have limited predictive power.

To overcome these disadvantages, we can use ensemble learning, which combine multiple trees to produce a single model for a single consensus prediction. Therefore, ensemble learning is more a machine learning process than a specific model. The main advantage of ensemble learning methods is that they are less prone to overfitting, and have better predictive power. The main disadvantage is that they are more difficult to interpret.

```{admonition} Ingredients: regression or classification trees
- Input: features of data samples
- Output: target values (regression) or class labels (classification) of data samples
- Model: divide the feature space into multiple simple regions, and make a prediction of the target value or class label for each region by averaging the target values or selecting the most common class label of the data samples in that region
  - Hyperparameter(s): maximum depth of tree, maximum number of leaves, and/or minimum number of samples in a leaf
  - Parameter(s): decision rules for each region consisting of a feature and a threshold
- Loss function: mean squared error / residual sum of squares (regression) or  Gini index / entropy (classification)
- Learning algorithm: greedy search for the best splitting rule across all features and thresholds at each step
```

```{admonition} System transparency: regression or classification trees
System logic
- Condition to produce certain output: to produce an output $y$ or a class label $c$, we need to find the region in the feature space producing a value closest to $y$ or containing the most samples of class $c$, then go from that region to the root of the tree to find the decision rules that lead to that region, and find any input features $x$ that satisfy those decision rules.
```

Ensemble learning (bagging, random forests, and boosting) is primarily a machine learning process so we consider its process transparency.

```{admonition} Process transparency: bagging, random forests, and boosting
- **Starting point**: a standardised dataset for a machine learning task with a performance metric defined and a "weak learner" (building block) model chosen to be trained
- Train multiple weak learning models (e.g. trees) on different subsets of the data, e.g. bootstrapped subsets of the data (bagging), and/or random subsets of the features (random forests), and/or different subsets of the data with different weights (boosting)
- Combine the predictions of the weak learning models to produce a single model for a single consensus prediction
- **End point**: a trained model for a single consensus prediction
```
