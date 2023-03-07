# GLM and SVM

<!-- Capitalise initials. As compact as possible, prefer ONE line. -->
<!-- We use **UK** English spelling. -->
<!-- File names should be all lowercase, with words separated by hyphens (-), and no spaces.  Each chapter must include an "overview.md" and "quiz-sum-ref.md"-->

<!-- ```{admonition} Status
Ready for review and feedback
``` -->

```{admonition} Objectives
- Understand linear, poisson, and logistic regression as generalised linear models (GLMs).
- Apply GLMs to real-world problems and interpret the results.
- Understand the basic concepts of support vector machine (SVM).
- Apply SVM to real-world problems and interpret the results.
```
<!-- - Evaluate the performance of a classifier using ROC curve and confusion matrix. -->

**Expected time to complete**: 4 hours

In this chapter, we will study [generalised linear models (GLMs)](https://en.wikipedia.org/wiki/Generalized_linear_model) and [support vector machines (SVMs)](https://en.wikipedia.org/wiki/Support_vector_machine).

GLM is a a flexible generalisation of [linear regression](https://pykale.github.io/transparentML/02-linear-reg/overview.html) to allow the linear model to be related to the response variable in a more complex way (via a link function) than a simple linear relationship. The [logistic regression](https://pykale.github.io/transparentML/03-logistic-reg/overview.html) in Chapter 3 is such a generalised linear model. In this chapter, we will study another GLM, the [poisson regression](https://en.wikipedia.org/wiki/Poisson_regression) that can predict count data.

SVM is a supervised machine learning model that was developed for classification problems but can be used for regression problems as well. In binary classification, it embodies the idea of finding a hyperplane that best separates the classes by maximising the margin between the hyperplane and the nearest data points from the two classes. SVM has been shown to perform well in a variety of settings, and is often considered one of the best "out of the box" classifiers.

<!-- SVM is an approach for classification that was developed in the computer science community in the 1990s and that has grown in popularity since then.  -->

```{admonition} Ingredients: Poisson regression
- Input: features of data samples
- Output: target values of data samples in the form of counts (non-negative integers)
- Model: transform the target values (counts) to its log, fit a line (or plane/hyperplane) to the transformed training data, and map the estimated value on the fitted line (or plane/hyperplane) for the test data to a count value via the exponential function.
  - Hyperparameter(s): None.
  - Parameters: the intercept(s) and slope(s) of the fitted line (or plane/hyperplane), also known as the bias(es) and weight(s), respectively
- Loss function: maximise the likelihood (probability) of the log of the target values for the training data samples.
- Learning algorithm: Gradient descent on the negative log likelihood of the training data samples
```

```{admonition} Transparency: Poisson regression
System logic
- Condition to produce certain output: to produce an output count $y$, take the log of $y$, locate this $\log(y)$ value on the fitted line (or plane/hyperplane) and then find the corresponding input $x$ (or $\mathbf{x}$) value.
```

```{admonition} Ingredients: SVM for binary classification
- Input: features of data samples.
- Output: binary class labels of data samples.
- Model: fit a plane/hyperplane to the training data to separate the data points by their class labels with the largest margin.
  - Hyperparameter(s): a tuning/regularisation parameter $\Omega$ for controlling the trade-off between the margin and the tolerance of misclassification (margin violation). If a kernel is used, other hyperparameters include the kernel type and the kernel parameters.
  - Parameter(s): the intercept ($\beta_0$) and coefficients ($\alpha_1, \alpha_2, \ldots, \alpha_N$) for each training data sample.
- Loss function: maximises the margin and minimises the misclassification (margin violation).
- Learning algorithm: quadratic programming.
```

```{admonition} Transparency: SVM for binary classification
System logic
- Condition to produce certain output: to produce a class label $y$, find out on which side of the fitted hyperplane this class label is located, and then all corresponding data points $x$ (or $\mathbf{x}$) on this side of the hyperplane will be likely candidates to produce a label $y$, the further away from the hyperplane, the more likely/confident.
```
<!-- - What input to produce certain output:
- How to produce certain output: -->
