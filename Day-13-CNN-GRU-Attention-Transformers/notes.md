# Day 13 Notes

# Convolutional Neural Network (CNN)

CNN is a Deep Learning architecture mainly used for image-related tasks.

Applications:

- Image Classification
- Object Detection
- Face Recognition
- Medical Image Analysis

---

# Why CNN?

Traditional Neural Networks treat every pixel independently.

CNN automatically learns spatial features such as:

- Edges
- Corners
- Textures
- Shapes
- Objects

---

# CNN Architecture

Image

↓

Convolution

↓

ReLU

↓

Pooling

↓

Flatten

↓

Dense Layer

↓

Output

---

# Convolution Layer

Applies filters (kernels) to the input image to extract important features.

Output:

Feature Maps

---

# Filter (Kernel)

A small matrix that scans across an image.

Examples:

- Edge Detection
- Vertical Lines
- Horizontal Lines
- Texture Detection

---

# Stride

Stride determines how many pixels the filter moves after each operation.

Large stride:

- Faster computation
- Less detail

Small stride:

- More detailed features
- Higher computation

---

# Padding

Padding adds extra pixels around the image.

Purpose:

- Preserve image dimensions
- Prevent loss of edge information

Types:

- Valid Padding
- Same Padding

---

# Max Pooling

Reduces image dimensions while keeping the most important features.

Advantages:

- Reduces computation
- Reduces overfitting
- Preserves dominant features

---

# Flatten Layer

Converts 2D feature maps into a 1D vector before passing them to Dense layers.

---

# Fully Connected Layer

Performs final classification based on extracted features.

---

# Gated Recurrent Unit (GRU)

GRU is a simplified version of LSTM.

Uses:

- Update Gate
- Reset Gate

Advantages:

- Faster training
- Fewer parameters
- Lower memory usage

---

# GRU vs LSTM

| GRU | LSTM |
|------|------|
| 2 Gates | 3 Gates |
| Faster | Slightly slower |
| Less memory | More memory |
| Simpler architecture | More complex |

---

# Attention Mechanism

Allows the model to focus on the most relevant parts of the input sequence.

Components:

- Query
- Key
- Value

Benefits:

- Better long-range dependency learning
- Improved translation and summarization

---

# Transformer

Transformer is a neural network architecture based entirely on attention mechanisms.

Advantages:

- Parallel computation
- Faster training
- Better context understanding

Components:

- Encoder
- Decoder
- Self-Attention
- Positional Encoding

---

# Hugging Face Transformers

Provides pretrained Transformer models for NLP.

Example:

```python
from transformers import pipeline

classifier = pipeline("sentiment-analysis")
```

Supports:

- Sentiment Analysis
- Translation
- Text Generation
- Summarization
- Question Answering

---

# Key Takeaways

✔ CNNs automatically learn image features.

✔ Convolution extracts patterns using filters.

✔ Pooling reduces dimensionality while retaining important information.

✔ GRU simplifies recurrent learning with fewer gates than LSTM.

✔ Attention helps models focus on relevant information.

✔ Transformers outperform traditional RNNs on many NLP tasks.

✔ Hugging Face makes it easy to use pretrained Transformer models.
