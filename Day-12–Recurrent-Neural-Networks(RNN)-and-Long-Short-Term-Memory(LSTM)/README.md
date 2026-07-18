# Day 12 – Recurrent Neural Networks (RNN) and Long Short-Term Memory (LSTM)

📅 Date: **01 July 2026**

---

# 🎯 Objective

Understand Recurrent Neural Networks (RNNs), their architecture, working mechanism, applications, limitations, and the motivation behind Long Short-Term Memory (LSTM). Learn how LSTM overcomes the vanishing gradient problem using gated memory cells.

---

# 📚 Topics Covered

## Introduction to Recurrent Neural Networks (RNN)

- What is Sequential Data?
- Why Feed Forward Neural Networks cannot handle sequence data
- Need for Recurrent Neural Networks
- Basic Architecture of RNN
- Hidden State (Memory)
- Time Steps

---

## Sequence Data

Examples of Sequential Data:

- Speech Recognition
- Text Generation
- Sentiment Analysis
- DNA Sequence Analysis
- Machine Translation
- Video Activity Recognition
- Time Series Forecasting

---

## Applications of RNN

- Language Modelling
- Text Generation
- Machine Translation
- Speech Recognition
- Image Captioning
- Face Detection
- Time Series Forecasting
- Video Processing

---

## Working of RNN

Studied:

- Hidden State
- Input Sequence
- Output Sequence
- State Update
- Information Flow Across Time Steps

Also understood:

- Forward Propagation
- Backpropagation Through Time (BPTT)

---

## Types of RNN

### One-to-One

- Single Input
- Single Output

Example:

Traditional Feed Forward Network

---

### One-to-Many

One input produces multiple outputs.

Example:

- Image Captioning

---

### Many-to-One

Multiple inputs generate one output.

Example:

- Sentiment Analysis

---

### Many-to-Many

Multiple inputs produce multiple outputs.

Examples:

- Language Translation
- Video Classification

---

## Advantages of RNN

- Captures temporal dependencies
- Supports variable-length sequences
- Shares parameters across time steps
- Learns sequential features automatically
- Effective for time-series forecasting
- Flexible architectures (BiRNN, LSTM, GRU)

---

## Limitations of RNN

- Vanishing Gradient Problem
- Exploding Gradient Problem
- Difficulty learning long-term dependencies
- Sequential computation (slow training)
- Limited context window
- Difficult to parallelize

---

## Variants of RNN

### Bidirectional RNN (BiRNN)

Processes sequence in:

- Forward Direction
- Backward Direction

Useful for:

- NLP
- Speech Recognition
- Time Series

---

### Long Short-Term Memory (LSTM)

Introduced to overcome:

- Vanishing Gradients
- Long-Term Dependency Problems

Uses gated memory cells for efficient information flow.

---

## Introduction to LSTM

Why LSTM?

Standard RNN:

❌ Cannot remember long-term information.

LSTM:

✅ Stores useful information.

✅ Removes unnecessary information.

✅ Handles long-term dependencies.

---

## LSTM Architecture

Components:

- Cell State (Ct)
- Hidden State (Ht)
- Forget Gate
- Input Gate
- Output Gate

---

## Gates in LSTM

### Forget Gate

Purpose:

Removes unnecessary information from memory.

Output Range:

0 → Forget

1 → Keep

---

### Input Gate

Determines which new information should be stored in memory.

Uses:

- Sigmoid Activation
- Tanh Activation

---

### Output Gate

Controls what information should be passed to the next hidden state.

Produces:

Current Output

Next Hidden State

---

## Applications of LSTM

- Language Modelling
- Text Generation
- Image Captioning
- Speech Recognition
- Handwriting Recognition
- Music Generation
- Language Translation
- Time Series Prediction

---

# 🛠️ Practical Learning

- Understood sequential data.
- Explored RNN architecture.
- Learned hidden state propagation.
- Studied Forward and Backward Propagation.
- Compared different RNN architectures.
- Understood vanishing and exploding gradients.
- Learned why LSTM was introduced.
- Explored LSTM gates and memory cell.

---

# 📂 Learning Resources

- RNN and LSTM Complete Notes.pdf

---

# 🎯 Learning Outcomes

After completing this session, I can:

- Explain how RNN processes sequential data.
- Differentiate Feed Forward Networks and RNNs.
- Explain different RNN architectures.
- Describe the vanishing gradient problem.
- Explain how LSTM solves long-term dependency issues.
- Describe Forget, Input, and Output Gates.
- Identify real-world applications of RNN and LSTM.

---

# 🚀 Outcome

Built a strong conceptual understanding of sequence modeling using Recurrent Neural Networks and Long Short-Term Memory networks. Learned how gated memory enables LSTMs to preserve long-term information, making them effective for NLP, speech recognition, machine translation, and time-series forecasting.
