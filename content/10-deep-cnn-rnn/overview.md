# Neural Networks and Deep Learning

<!-- Capitalise initials. As compact as possible, prefer ONE line. -->
<!-- We use **UK** English spelling. -->
<!-- File names should be all lowercase, with words separated by hyphens (-), and no spaces.  Each chapter must include an "overview.md" and "quiz-sum-ref.md"-->

<!-- ```{admonition} Status
Ready for review and feedback
``` -->

```{admonition} Objectives
- Understand the concept of neural networks (NNs) and deep learning models.
- Understand the concept of convolutional NNs (CNNs) and recurrent NNs (RNNs).
- Apply convolutional NNs to image classification.
- Apply recurrent NNs to text classification.
```

**Expected time to complete**: 6 hours

In this chapter, we will give a light introduction to [neural networks](https://en.wikipedia.org/wiki/Neural_network) and [deep learning](https://en.wikipedia.org/wiki/Deep_learning) models including [convolutional neural networks (CNNs)](https://en.wikipedia.org/wiki/Convolutional_neural_network) and [recurrent neural networks (RNNs)](https://en.wikipedia.org/wiki/Recurrent_neural_network). Neural networks are a class of machine learning models that are inspired by the structure and function of biological neural networks. They are used to learn complex functions from large amounts of data. Deep learning models are neural networks with multiple hidden layers. CNNs are deep learning models that are used for image classification and object detection. RNNs are deep learning models that are used for sequence modelling and time series forecasting.

Neural networks and deep learning models are commonly considered to be black-box models that are not transparent. However, by examining the three criteria of [system transparency](https://pykale.github.io/transparentML/01-intro/ml-transp.html#system-transparency), we can see that neural networks and deep learning models can often satisfy the first two criteria of system transparency. We can explicitly define how to transform inputs to outputs but the conditions to produce certain outputs are often difficult to explain. Therefore, we consider neural networks and deep learning models to be partially transparent models, or semi-transparent models.

Neural networks can be used for both supervised and unsupervised learning. We will focus on supervised learning in this chapter.

<!-- We will also introduce the concept of transfer learning. -->

```{admonition} Ingredients: neural networks
- Input: features of data samples
- Output: target values (regression) or class labels (classification) of data samples
- Model: pass the input through multiple layers of "neurons", where each neuron is a linear function (weighted sum plus bias) followed by a nonlinear activation function to produce an output for the next layer of neurons (or the final output after the last layer of neurons)
  - Hyperparameter(s): number of layers, number of neurons in each layer, activation function, and/or learning rate
  - Parameter(s): weights and biases of each neuron
- Loss function: mean squared error / residual sum of squares (regression) or cross-entropy (classification), or other loss functions
- Learning algorithm: gradient descent (or other optimisation algorithms)
```

```{admonition} Transparency
System logic
- Condition to produce certain output: due to the complexity of the model, it is difficult to explain the conditions to produce certain output. Although there are some methods to explain the output of neural networks and deep learning models such as the [local interpretable model-agnostic explanations (LIME)](https://homes.cs.washington.edu/~marcotcr/blog/lime/), such explanations are approximate and may not be accurate.
```

<!-- - What input to produce certain output:
- How to produce certain output: -->
