# Day 10 – Perceptron and Multi-Layer Perceptron (MLP)

📅 **Date:** 29 June 2026

## 🎯 Objective

Understand the evolution from the single-layer Perceptron to Multi-Layer Perceptrons (MLPs), explore neural network architectures, activation functions, nonlinear learning, feature representation, and understand why deep neural networks outperform traditional linear models.

---

# 📚 Topics Covered

## Introduction to Artificial Neural Networks

- Biological inspiration behind Neural Networks
- Artificial Neuron
- Inputs, Weights and Bias
- Weighted Sum
- Activation Function
- Output Generation

---

## Perceptron

Studied the architecture of a single-layer Perceptron.

### Components

- Input Layer
- Weights
- Bias
- Activation Function
- Output

### Applications

- Binary Classification
- Linear Classification Problems

---

## Limitations of Perceptron

Learned why a single-layer Perceptron cannot solve nonlinear problems.

Examples:

- XOR Problem
- Complex Decision Boundaries

---

## Multi-Layer Perceptron (MLP)

Introduced hidden layers to overcome the limitations of the Perceptron.

Architecture:

Input Layer

↓

Hidden Layer(s)

↓

Output Layer

MLPs can model nonlinear relationships between input and output.

---

## Neural Network Architecture

Studied:

- Input Layer
- Hidden Layer
- Output Layer
- Weight Matrices
- Bias Terms

Observed how information flows through a neural network during forward propagation.

---

## Activation Functions

Studied different activation functions and their properties.

### Sigmoid

- Output Range: 0 to 1
- Used for Binary Classification
- Suffers from Vanishing Gradient

---

### Tanh

- Output Range: -1 to 1
- Zero-centered
- Better than Sigmoid for hidden layers

---

### ReLU (Rectified Linear Unit)

- Most commonly used activation
- Faster convergence
- Efficient computation
- Can suffer from Dead Neuron Problem

---

### Leaky ReLU

Improved version of ReLU.

Advantages:

- Allows small gradients for negative values
- Reduces dead neuron problem

---

## Why MLP Can Learn Nonlinear Functions

Learned how hidden layers and nonlinear activation functions enable neural networks to approximate complex nonlinear decision boundaries.

Key Concept:

> A sufficiently large single hidden-layer MLP can approximate any continuous function (Universal Approximation Theorem).

---

## Neural Network Architectures

Studied multiple architectures:

### Single Hidden Layer – Single Output

Applications:

- Regression
- Binary Classification

---

### Single Hidden Layer – Multiple Outputs

Applications:

- Multi-class Classification
- Multi-label Classification
- Vector-valued Regression

---

### Multiple Hidden Layers

Deep Neural Networks consisting of:

- Multiple hidden layers
- Multiple outputs
- Hierarchical feature learning

---

## Neural Networks as Feature Learners

Learned that hidden layers automatically learn useful feature representations from raw input data.

Instead of manually designing features, neural networks learn features directly from data.

---

## Kernel Methods vs Neural Networks

Compared:

Kernel Methods

vs

Deep Neural Networks

Observed:

- Kernel methods use predefined basis functions.
- Neural Networks learn basis functions automatically.
- Neural Networks require less memory during inference.
- Deep learning scales better for large datasets.

---

## Feature Learning

Understood how neurons act as pattern detectors.

Each hidden neuron learns:

- Shapes
- Patterns
- Features
- Representations

Higher layers combine lower-level features into more abstract concepts.

---

## Why Neural Networks Perform Better

Compared with traditional linear models.

Neural Networks:

- Learn multiple features simultaneously.
- Capture complex nonlinear relationships.
- Generalize better.
- Learn hierarchical representations.

---

# 🛠️ Practical Learning

✔ Studied Perceptron architecture.

✔ Understood why Perceptrons fail on nonlinear problems.

✔ Learned MLP architecture.

✔ Explored activation functions.

✔ Compared Sigmoid, Tanh, ReLU and Leaky ReLU.

✔ Studied Universal Approximation.

✔ Explored feature learning.

✔ Compared Kernel Methods with Neural Networks.

---

# 📂 Learning Resources

- Perceptron and MLP.pdf

---

# 🎯 Learning Outcomes

After completing this session, I can:

- Explain how Perceptrons work.
- Describe the limitations of single-layer networks.
- Explain Multi-Layer Perceptrons.
- Select suitable activation functions.
- Understand forward information flow.
- Explain automatic feature learning.
- Compare Neural Networks with Kernel Methods.
- Understand why Deep Learning performs better than traditional ML models.

---

# 🚀 Outcome

Built a strong conceptual understanding of Artificial Neural Networks and Multi-Layer Perceptrons, preparing for upcoming topics such as Backpropagation, Optimization Algorithms, and Deep Neural Network training.
