# Day 16 Notes

## Variational Autoencoder (VAE)

A Variational Autoencoder is a probabilistic generative model that learns the distribution of training data and generates new samples.

---

## VAE Components

### Encoder

- Receives input data.
- Learns Mean (μ) and Variance (σ).
- Represents data as a probability distribution instead of a fixed vector.

---

### Latent Space

Latent Vector:

z ~ N(μ, σ²)

Stores compressed information for generating new samples.

---

### Reparameterization Trick

Formula:

z = μ + σ × ε

where

ε ~ N(0,1)

Purpose:

Allows backpropagation while introducing randomness.

---

### Decoder

Converts latent vectors back into reconstructed data.

---

## VAE Loss

### Reconstruction Loss

Measures reconstruction quality.

Examples:

- Mean Squared Error (MSE)
- Binary Cross Entropy (BCE)

---

### KL Divergence

Encourages the latent distribution to resemble a standard normal distribution.

Benefits:

- Smooth latent space
- Better interpolation
- Improved sample generation

---

### Final Loss

Total Loss = Reconstruction Loss + KL Divergence Loss

---

## Advantages

- Generates realistic samples.
- Smooth latent representation.
- Useful for anomaly detection.

---

## Limitation

- Generated outputs can be blurry.

---

# Autoregressive Models

Generate sequences token by token.

Each prediction depends on previously generated tokens.

Examples:

- RNN
- LSTM
- GRU

---

## Challenges

- Vanishing Gradient
- Difficulty learning long-term dependencies

---

# GPT

GPT = Generative Pre-trained Transformer

A decoder-only Transformer model for autoregressive language generation.

---

## GPT Workflow

1. Token Embedding
2. Positional Encoding
3. Masked Self-Attention
4. Feed Forward Network
5. Next Token Prediction

---

## GPT Advantages

- Parallel processing
- Better long-context understanding
- Faster training than RNN-based models

---

# Text Generation Techniques

## Greedy Search

Chooses the highest-probability token.

Simple but repetitive.

---

## Beam Search

Maintains multiple candidate sequences.

Produces better quality than greedy search.

---

## Random Sampling

Samples tokens according to their probability.

More diverse but less predictable.

---

## Temperature Sampling

Controls randomness.

- Low Temperature → Conservative output
- High Temperature → Creative output

---

## Top-K Sampling

Selects from the K most probable tokens.

Balances diversity and quality.

---

## Top-P (Nucleus) Sampling

Chooses tokens until cumulative probability exceeds threshold P.

Produces natural and coherent text.

---

# Key Takeaways

✔ VAEs are probabilistic generative models.

✔ The encoder learns a probability distribution instead of fixed features.

✔ The reparameterization trick enables gradient-based optimization.

✔ Autoregressive models generate sequences one token at a time.

✔ GPT is a decoder-only Transformer that predicts the next token using masked self-attention.

✔ Modern LLMs use advanced decoding strategies such as Top-K, Top-P, Beam Search, and Temperature Sampling to generate high-quality text.
