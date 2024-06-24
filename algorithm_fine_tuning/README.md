
### Prototype Selection for Nearest Neighbor Classification

One way to speed up nearest neighbor classification is to replace the training set by a carefully chosen subset of "prototypes". Instead of retaining the entire training set for nearest neighbor classification, we aim to select a small but representative subset to search for nearest neighbors. This reduces the search space, resulting in faster classification. However, the challenge lies in selecting effective prototypes to ensure good classification performance on the test data.

In this project, we focus on developing a strategy for choosing prototypes from the training set with the ultimate goal of achieving high classification performance on test data. We need to identify the properties that make a set of examples effective for nearest neighbor classification, formalize these properties, and use them to automatically select prototypes. For this project, assume that 1-NN (1-Nearest Neighbor) will be used.

We will implement your algorithm and test it on the MNIST dataset.



### Coordinate Descent

In this project, we consider a standard unconstrained optimization problem:

\[ \min L(w) \]

where \( L(\cdot) \) is a cost function and \( w \in \mathbb{R}^d \). In class, several approaches such as gradient descent and stochastic gradient descent were explored under differentiability conditions on \( L(w) \). Here, we explore a different and simpler approach: coordinate descent.

The coordinate descent method involves the following steps:

1. Initialize \( w \) somehow.
2. Repeat: pick a coordinate \( i \in \{1, 2, \ldots, d\} \), and update the value of \( w_i \) to reduce the loss.

