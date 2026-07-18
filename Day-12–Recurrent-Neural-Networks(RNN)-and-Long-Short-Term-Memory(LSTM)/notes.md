# Day 12 Notes

# Recurrent Neural Network (RNN)

A Recurrent Neural Network (RNN) is a type of neural network designed to process sequential or time-dependent data.

Unlike Feed Forward Neural Networks, RNNs maintain a hidden state (memory) that carries information from previous time steps.

---

# Why RNN?

Traditional Neural Networks:

- Independent inputs
- No memory

RNN:

- Sequential inputs
- Maintains memory
- Captures temporal dependencies

---

# Sequence Data Examples

- Speech Recognition
- Sentiment Analysis
- Language Translation
- DNA Analysis
- Video Activity Recognition
- Time-Series Forecasting
- Music Generation

---

# Applications of RNN

- Language Modeling
- Text Generation
- Speech Recognition
- Image Captioning
- Face Detection
- Time-Series Prediction
- Machine Translation

---

# Hidden State

The hidden state stores information from previous time steps and is updated at every step.

Hidden State = Memory of the network.

---

# Working of RNN

Input Sequence

↓

Hidden State

↓

Output

↓

Updated Hidden State

↓

Next Time Step

---

# Forward Propagation

Processes input sequence one time step at a time.

Updates hidden state continuously.

---

# Backpropagation Through Time (BPTT)

Updates weights by propagating gradients backward across all time steps.

---

# Types of RNN

## One-to-One

One Input → One Output

Example:

Simple Neural Network

---

## One-to-Many

One Input → Multiple Outputs

Example:

Image Captioning

---

## Many-to-One

Multiple Inputs → One Output

Example:

Sentiment Analysis

---

## Many-to-Many

Multiple Inputs → Multiple Outputs

Example:

Language Translation

---

# Advantages of RNN

✔ Captures temporal dependencies.

✔ Supports variable-length sequences.

✔ Shares weights across time.

✔ Automatic feature extraction.

✔ Effective for sequence prediction.

---

# Limitations of RNN

## Vanishing Gradient

Gradients become very small.

Result:

Model forgets long-term information.

---

## Exploding Gradient

Gradients become extremely large.

Result:

Unstable training.

---

## Other Limitations

- Slow training
- Limited context window
- Difficult parallelization

---

# Bidirectional RNN (BiRNN)

Processes sequence in both forward and backward directions.

Useful when future context improves prediction.

Applications:

- NLP
- Speech Recognition

---

# Long Short-Term Memory (LSTM)

LSTM is an advanced RNN architecture designed to solve long-term dependency problems.

Key Feature:

Memory Cell

---

# LSTM Components

- Cell State (Ct)
- Hidden State (Ht)
- Forget Gate
- Input Gate
- Output Gate

---

# Forget Gate

Purpose:

Removes unnecessary information.

Output:

0 → Forget

1 → Keep

---

# Input Gate

Adds useful information to memory.

Uses:

Sigmoid + Tanh

---

# Output Gate

Determines what information is passed to the next hidden state.

---

# Why LSTM is Better

| RNN | LSTM |
|------|------|
| Short-term memory | Long-term memory |
| Vanishing gradients | Handles vanishing gradients |
| Simple architecture | Gated architecture |
| Limited sequence learning | Better long-sequence learning |

---

# Applications of LSTM

- NLP
- Machine Translation
- Text Generation
- Image Captioning
- Speech Recognition
- Handwriting Recognition
- Music Generation
- Financial Forecasting

---

# Key Takeaways

✔ RNNs are designed for sequential data.

✔ Hidden states enable memory across time steps.

✔ Standard RNNs struggle with long-term dependencies due to vanishing gradients.

✔ LSTMs introduce memory cells and three gates—Forget, Input, and Output—to regulate information flow.

✔ LSTMs are widely used in NLP, speech processing, and time-series forecasting because they retain important information over long sequences.
