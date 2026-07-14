# Day 08 Notes

## What is TensorFlow?

TensorFlow is an open-source Machine Learning and Deep Learning framework developed by Google.

It is used for:

- Deep Learning
- Computer Vision
- Natural Language Processing
- Recommendation Systems
- Time Series Forecasting

---

## What is Keras?

Keras is TensorFlow's high-level API used for building neural networks.

Advantages:

- Easy to learn
- Fast model development
- Modular design
- Built into TensorFlow

---

## Sequential Model

A Sequential model is a linear stack of neural network layers.

Example:

Input Layer

↓

Hidden Layer

↓

Output Layer

---

## Dense Layer

A Dense layer is a fully connected neural network layer where every neuron is connected to every neuron in the next layer.

Example:

```python
Dense(64, activation="relu")
```

---

## What are Tensors?

Tensors are multidimensional arrays used to represent data.

Types:

- Scalar (0D)
- Vector (1D)
- Matrix (2D)
- Higher-order Tensor (3D+)

Example:

```python
tf.constant([1,2,3])
```

---

## TensorFlow Data Types

Common data types:

- tf.int32
- tf.int64
- tf.float32
- tf.float64
- tf.bool
- tf.string
- tf.complex64

---

## Computational Graph

A computational graph represents mathematical operations as nodes connected by tensors.

Advantages:

- Faster execution
- Graph optimization
- Efficient memory management

---

## TensorFlow 2.x

Uses Eager Execution.

Operations execute immediately.

Example:

```python
x = tf.constant(5)
y = tf.constant(10)
print(x + y)
```

---

## TensorFlow 1.x

Used Sessions to execute computational graphs.

Example:

```python
with tf.Session():
```

TensorFlow 2.x no longer requires Sessions.

---

## TensorFlow 1.x vs TensorFlow 2.x

| TensorFlow 1.x | TensorFlow 2.x |
|---------------|----------------|
| Uses Sessions | Eager Execution |
| Static Graph | Dynamic Execution |
| More Complex | Beginner Friendly |
| Slower Development | Faster Development |

---

## Key Learnings

✔ TensorFlow is the most popular Deep Learning framework.

✔ Keras simplifies neural network development.

✔ Tensors are the core data structure in TensorFlow.

✔ TensorFlow 2.x executes operations eagerly.

✔ Computational graphs improve execution efficiency.

✔ TensorFlow 2.x is easier to learn than TensorFlow 1.x.
