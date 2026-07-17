# Day 11 Notes

# MNIST Dataset

MNIST is one of the most popular benchmark datasets for image classification.

Dataset contains:

- 60,000 Training Images
- 10,000 Testing Images

Each image size:

28 × 28 pixels

Classes:

0–9

---

# Data Normalization

Original pixel values:

0–255

Normalized values:

0–1

Formula:

Normalized Pixel = Pixel / 255

Benefits:

- Faster training
- Stable gradient updates
- Better convergence

---

# Flatten Layer

Input Image:

28 × 28

↓

Flatten

↓

784 Features

Purpose:

Convert a 2D image into a 1D vector before feeding it to Dense layers.

---

# Dense Layer

Fully connected neural network layer.

Example:

Dense(128, activation="relu")

Every neuron receives input from all neurons in the previous layer.

---

# Activation Functions

## ReLU

Formula:

max(0,x)

Advantages:

- Fast
- Solves vanishing gradients better than Sigmoid
- Most common hidden-layer activation

---

## Softmax

Converts output values into probability distribution.

Output:

10 probabilities

Highest probability → Predicted digit

---

# Sequential API

Used when layers are arranged sequentially.

Simple and beginner-friendly.

---

# Functional API

Allows flexible architectures.

Useful for:

- Multiple Inputs
- Multiple Outputs
- Skip Connections
- Complex Networks

---

# Model Compilation

Optimizer:

Adam

Loss:

Sparse Categorical Crossentropy

Metric:

Accuracy

---

# Model Training

Model learns by updating weights over multiple epochs.

Validation Split:

20%

Purpose:

Evaluate performance during training.

---

# Model Evaluation

Important metrics:

- Accuracy
- Loss

Higher Accuracy

Lower Loss

indicates better learning.

---

# Classification Report

Contains:

Precision

Recall

F1-score

Support

These metrics help analyze performance for each digit class.

---

# Confusion Matrix

Shows:

Actual Class

vs

Predicted Class

Diagonal values represent correct predictions.

Off-diagonal values indicate misclassifications.

---

# PCA (Principal Component Analysis)

Purpose:

Reduce dimensionality while preserving maximum information.

Example:

784 Features

↓

100 Principal Components

Advantages:

- Faster training
- Reduced memory usage
- Removes redundant information

---

# Logistic Regression

Traditional Machine Learning algorithm.

Works well on linearly separable problems.

Requires flattened image vectors.

---

# Support Vector Machine (SVM)

Finds an optimal decision boundary with maximum margin.

Advantages:

- Effective in high-dimensional spaces.
- Good classification performance.

Disadvantages:

- Computationally expensive on very large datasets.

---

# ANN vs Logistic Regression

| ANN | Logistic Regression |
|------|---------------------|
| Learns nonlinear patterns | Learns linear decision boundaries |
| Hidden layers | No hidden layers |
| Higher accuracy on images | Lower performance on complex image tasks |
| Automatic feature learning | Manual feature representation |

---

# Key Learnings

✔ MNIST is a standard dataset for image classification.

✔ Images must be normalized before training.

✔ Flatten converts images into vectors.

✔ ReLU improves learning speed.

✔ Softmax is used for multiclass classification.

✔ Sequential API is simple, while Functional API provides flexibility.

✔ PCA reduces feature dimensions.

✔ Deep Learning generally outperforms traditional ML methods on image classification tasks.
