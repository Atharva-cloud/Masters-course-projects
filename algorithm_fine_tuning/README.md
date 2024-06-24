
Prototype Selection for Nearest Neighbor Classification
One way to speed up nearest neighbor classification is to replace the training set by a carefully chosen subset of "prototypes". Instead of retaining the entire training set for nearest neighbor classification, we aim to select a small but representative subset to search for nearest neighbors. This reduces the search space, resulting in faster classification. However, the challenge lies in selecting effective prototypes to ensure good classification performance on the test data.

In this project, we focus on developing a strategy for choosing prototypes from the training set with the ultimate goal of achieving high classification performance on test data. We need to identify the properties that make a set of examples effective for nearest neighbor classification, formalize these properties, and use them to automatically select prototypes. For this project, assume that 1-NN (1-Nearest Neighbor) will be used.

You will implement your algorithm and test it on the MNIST dataset, which can be found at the following link: [MNIST Dataset on Kaggle]([url](https://www.kaggle.com/datasets/hojjatk/mnist-dataset)).
