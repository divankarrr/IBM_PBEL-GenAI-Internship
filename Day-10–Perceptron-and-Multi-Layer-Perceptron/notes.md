# Day 10 Notes

# Artificial Neural Network (ANN)

Artificial Neural Networks are computational models inspired by the biological neurons of the human brain.

A neural network learns patterns by adjusting weights during training.

---

# Basic Structure of a Neuron

Input

↓

Weighted Sum

↓

Bias Addition

↓

Activation Function

↓

Output

---

# Perceptron

A Perceptron is the simplest neural network consisting of a single neuron.

Equation:

y = f(wx + b)

Where:

- x = Input
- w = Weight
- b = Bias
- f = Activation Function

Applications:

- Binary Classification
- Linear Decision Boundary

---

# Limitations of Perceptron

Cannot solve:

- XOR Problem
- Nonlinear Classification

Reason:

Perceptron can only learn linear decision boundaries.

---

# Multi-Layer Perceptron (MLP)

MLP introduces hidden layers between input and output.

Architecture:

Input Layer

↓

Hidden Layer

↓

Output Layer

Advantages:

- Learns nonlinear functions.
- Better prediction accuracy.
- Automatic feature learning.

---

# Forward Propagation

Data flows through the network as:

Input

↓

Hidden Layer

↓

Output Layer

Each layer performs:

Weighted Sum

↓

Activation Function

---

# Activation Functions

## Sigmoid

Formula:

σ(x)=1/(1+e⁻ˣ)

Range:

0 to 1

Pros:

- Probability interpretation.

Cons:

- Vanishing Gradient.

---

## Tanh

Range:

-1 to 1

Advantages:

- Zero-centered outputs.

Still suffers from gradient saturation.

---

## ReLU

Formula:

max(0,x)

Advantages:

- Fast computation.
- Sparse activation.
- Most popular hidden-layer activation.

Disadvantage:

Dead neurons for negative inputs.

---

## Leaky ReLU

Formula:

max(0.01x,x)

Advantages:

- Solves dead neuron problem.
- Allows small gradients for negative inputs.

---

# Universal Approximation Theorem

A sufficiently large MLP with one hidden layer can approximate any continuous function.

This explains why neural networks are capable of solving complex nonlinear problems.

---

# Neural Network Architectures

### Single Output

Applications:

- House Price Prediction
- Binary Classification

---

### Multiple Outputs

Applications:

- Image Classification
- Multi-label Classification

---

### Deep Networks

Multiple hidden layers learn increasingly abstract features.

---

# Feature Learning

Unlike traditional ML, neural networks automatically learn useful features.

Hidden layers behave like feature detectors.

Early layers:

- Edges
- Shapes

Later layers:

- Objects
- Concepts

---

# Kernel Methods vs Neural Networks

Kernel Methods:

- Fixed feature mapping.
- Slower during prediction.
- Stores training samples.

Neural Networks:

- Learn feature mapping automatically.
- Faster inference.
- Better scalability.

---

# Why Deep Learning Works Better

Traditional ML:

- Manual feature engineering.
- Limited complexity.

Deep Learning:

- Automatic feature learning.
- Hierarchical representations.
- Better nonlinear modeling.

---

# Key Takeaways

✔ Perceptrons solve only linear problems.

✔ MLPs solve nonlinear problems using hidden layers.

✔ Activation functions introduce nonlinearity.

✔ ReLU is the most widely used activation function.

✔ Hidden layers automatically learn features.

✔ Neural Networks outperform traditional linear models on complex tasks.

✔ Deep Learning eliminates the need for manual feature engineering in many applications.
