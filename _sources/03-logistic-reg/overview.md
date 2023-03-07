# Logistic Regression

<!-- Capitalise initials. As compact as possible, prefer ONE line. -->
<!-- We use **UK** English spelling. -->
<!-- File names should be all lowercase, with words separated by hyphens (-), and no spaces.  Each chapter must include an "overview.md" and "quiz-sum-ref.md"-->

<!-- ```{admonition} Status
Ready for review and feedback
``` -->

```{admonition} Objectives
- Understand the basic concepts of logistic regression.
- Apply logistic regression to real data.
- Evaluate the performance of a logistic regression model.
- Interpret the results of a logistic regression.
```

**Expected time to complete**: 2.5 hours

The linear regression model discussed in {doc}`Linear regression <../02-linear-reg/overview>` assumes that the response variable $y$ is quantitative. But in many situations, the response variable is instead qualitative. In this chapter, we will study approaches for predicting qualitative responses, a process that is known as _classification_. There are many possible classification techniques, or classifiers, that can be used to predict a qualitative response. In this chapter, we will focus on logistic regression, which is a classification technique that is commonly used for binary classification, i.e. to predict a binary response, a response with only two possible outcomes such as pass/fail, win/lose, alive/dead or healthy/sick.
<!-- Logistic regression is an extension of linear regression that is used when the response variable is categorical. It is also known as _logit regression_ or _logit model_. In this chapter, we will learn how to use logistic regression to make predictions and understand the relationship between variables. We will learn the basic concepts of logistic regression and apply it to real data. We will also learn how to evaluate the performance of a logistic regression model and interpret the results. -->

```{admonition} Ingredients
- Input: features of data samples.
- Output: class labels of data samples.
- Model: transform the class label probability ranging from 0 to 1 to a range from -$\infty$, to $\infty$ using the [logit function](https://en.wikipedia.org/wiki/Logit) and fit a line (or plane/hyperplane), i.e. a linear regression model, to the transformed training data and map the value on the fitted line (or plane/hyperplane) for the test data to its corresponding class label probability via the [logistic (sigmoid, inverse logit) function](https://en.wikipedia.org/wiki/Logistic_function).
  - Hyperparameter(s): None (unless using regularisation).
  - Parameter(s): the intercept(s) and slope(s) of the fitted line (or plane/hyperplane), also known as the bias(es) and weight(s), respectively.
- Loss function: maximise the joint likelihood (probability) of the class labels for the training data points.
- Learning algorithm: Gradient descent on the negative log likelihood (or cross-entropy).
```

```{admonition} System transparency
System logic
- Condition to produce certain output: to produce a positive label with a probability $p$, or equivalently a negative label with a probability $(1-p)$, transform the probability $p$ to a real value $\mathrm{logit}(p)$ via the logit function, locate this value $\mathrm{logit}(p)$ on the fitted line (or plane/hyperplane) and then find the corresponding input $x$ (or $\mathbf{x}$) value.
```
<!-- find a data point $x$ such that $\mathbb{P}(c|\mathbf{x}, \boldsymbol{\beta}) > 0.5$ where $\boldsymbol{\beta}$ is the vector of parameters of the logistic regression model. -->
<!-- - What input to produce certain output:
- How to produce certain output: -->
