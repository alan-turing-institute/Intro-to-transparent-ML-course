# Cross-Validation and Bootstrap

<!-- Capitalise initials. As compact as possible, prefer ONE line. -->
<!-- We use **UK** English spelling. -->
<!-- File names should be all lowercase, with words separated by hyphens (-), and no spaces.  Each chapter must include an "overview.md" and "quiz-sum-ref.md"-->

<!-- ```{admonition} Status
Ready for review and feedback
``` -->

```{admonition} Objectives
- Understand the concepts and processes of cross-validation and bootstrap.
- Evaluate the performance of machine learning models using cross-validation.
- Quantify the uncertainty associated with a machine learning model using bootstrap.
```

**Expected time to complete**: 2.5 hours

As shown in previous chapters, the performance of a machine learning model is evaluated using a performance metric. The discussions in [multiple hypothesis testing](https://pykale.github.io/transparentML/04-hypo-test-sw-dev/hypothesis-testing.html#multiple-hypothesis-testing) imply that if we compute the performance metric using only a single split of the data into training and test sets, we may not have high confidence in the results and subsequent conclusions drawn from them, particularly when the performance metric is sensitive to the particular split of the data. We'd better take into account the variability in the data.

In this chapter, we will learn about two [resampling methods](https://en.wikipedia.org/wiki/Resampling_(statistics)), cross-validation and bootstrap, to evaluate the performance of a machine learning model more rigorously and quantify the uncertainty associated with it. As the name "resampling" suggests, both methods involve resampling the data. They repeatedly draw samples from a training set and refit a model of interest on each set of drawn samples to obtain additional information about the fitted model. For example, to estimate the variability of a linear regression fit, we can repeatedly draw different samples from the training data, fit a linear regression to each new sample set, and then examine the extent to which the resulting fits differ. This approach allows us to obtain information that would not be available from fitting the model only once using the original training sample.

```{admonition} Process transparency: $K$-fold cross-validation
- **Starting point**: a standardised dataset for a machine learning task with a performance metric defined and a machine learning model chosen to address a practical need/problem
- Determine the number of folds $K$ to use in cross-validation
- Split the dataset into $K$ folds
- For each fold $k$:
    - Train the model on the remaining $K-1$ folds
    - Evaluate the model on fold $k$
- Compute the average performance metric across the $K$ folds
- **End point**: Report the average performance metric and its standard deviation
```

```{admonition} Process transparency: bootstrap
- **Starting point**: a standardised dataset for a machine learning task with a performance metric defined and a machine learning model chosen to address a practical need/problem
- Determine the number of bootstrap samples $B$ to use
- For each bootstrap sample $b$:
    - Draw a bootstrap sample from the dataset
    - Train the model on the bootstrap sample
    - Evaluate the model on the bootstrap sample
- Compute the average performance metric across the $B$ bootstrap samples
- **End point**: Report the average performance metric and its standard deviation
```
