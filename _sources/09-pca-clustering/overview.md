# Principal Component Analysis & Clustering
<!-- # Principal Component Analysis & $K$-Means Clustering -->

<!-- Capitalise initials. As compact as possible, prefer ONE line. -->
<!-- We use **UK** English spelling. -->
<!-- File names should be all lowercase, with words separated by hyphens (-), and no spaces.  Each chapter must include an "overview.md" and "quiz-sum-ref.md"-->

<!-- ```{admonition} Status
Ready for review and feedback
``` -->

```{admonition} Objectives
- Understand principal component analysis (PCA) for dimensionality reduction.
- Apply PCA to real-world problems and interpret the results.
- Understand $K$-means and hierarchical clustering for data grouping.
- Apply $K$-means and hierarchical clustering to real-world problems and interpret the results.
```

**Expected time to complete**: 3 hours

The previous chapters have introduced various regression and classification methods, which are all supervised learning methods. In supervised learning, we typically have access to a set of $N$ observations (samples), with each having $D$ features $x_1, x_2, \ldots, x_D$ and a corresponding response $y$. The goal of supervised learning is to predict $y$ using $x_1, x_2, \ldots, x_D$.

This chapter will instead focus on unsupervised learning for the setting in which we have only a set of features $x_1, x_2, \ldots, x_D$ measured on $N$ observations. The task here is not to predict a response, because we do not have an associated response variable $y$. Rather, the goal is to discover or explore interesting things about the features $x_1, x_2, \ldots, x_D$ by learning their lower-dimensional representations or groupings. For example, is there an informative way to visualise the data samples via their two-dimensional or three-dimensional representations? Can we discover interesting subgroups among the $N$ observations? Unsupervised learning answers such questions. Here, we will focus on [principal component analysis (PCA)](https://en.wikipedia.org/wiki/Principal_component_analysis) for data visualisation or data pre-processing (typically before supervised learning methods are applied) and [$K$-means](https://en.wikipedia.org/wiki/K-means_clustering) / [hierarchical clustering](https://en.wikipedia.org/wiki/Hierarchical_clustering) for discovering subgroups in data.

<!-- Q or M for low-dim? Textook use M -->
```{admonition} Ingredients: principal component analysis
- Input: high-dimensional ($D$) features of data samples
- Output: lower-dimensional ($M<D$) features of data samples
- Model: linear (simple weighted) transformation (mapping) of data samples from high-dimensional space to lower-dimensional space
  - Hyperparameter: $M$, the number of principal components, i.e. the lower dimension
  - Parameter(s): a $D \times M$ transformation matrix mapping the original $D$-dimensional input to the transformed $M$-dimensional output
- Loss function: maximise the variance of the lower-dimensional features in the transformed space
- Learning algorithm: eigendecomposition or singular value decomposition
```

```{admonition} Transparency: principal component analysis
System logic
- Condition to produce certain output: to produce a certain lower-dimensional representation $ \mathbf{y} $, we can use the inverse of the same transformation matrix to project the lower-dimensional representation $ \mathbf{y} $ back to the original high-dimensional space to obtain a reconstructed input $ \hat{\mathbf{x}} $. This reconstructed input $ \hat{\mathbf{x}} $ is the input that produces the output $ \mathbf{y} $ with the transformation matrix.
```

```{admonition} Ingredients: $K$-means clustering
- Input: features of data samples
- Output: cluster memberships for each sample, assigned from $k=1, 2, \cdots, K$
- Model: find $K$ cluster centres in the feature space so that samples in the same cluster are as similar to each other as possible
  - Hyperparameter(s): $K$, the number of clusters
  - Parameter(s): the $K$ cluster centres in the feature space, i.e. in terms of the $D$ features, so there are $K \times D$ parameters
- Loss function: minimise the sum of squared distances between data samples and their assigned cluster centres
- Learning algorithm: repeated cluster membership assignment and cluster centre update after an initial random assignment of cluster centres
```

```{admonition} Transparency: $K$-means clustering
System logic
- Condition to produce certain output: to produce a certain cluster assignment $k$ (i.e. an output $y=k$), locate a data point $\mathbf{x}$ whose distance to the centre of the $k$th cluster is smaller than its distance to any other cluster centres then this $\mathbf{x}$ belongs to cluster $k$.
```
<!-- - What input to produce certain output:
- How to produce certain output: -->
