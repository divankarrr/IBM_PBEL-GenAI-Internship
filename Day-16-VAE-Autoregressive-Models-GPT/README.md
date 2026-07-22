# Day 16 – Variational Autoencoders (VAE), Autoregressive Models & GPT

📅 **Date:** 06 July 2026

## 🎯 Objective

Understand advanced Generative AI models including Variational Autoencoders (VAEs), Autoregressive Models, and Generative Pre-trained Transformers (GPT). Learn how these models generate new data and explore different text generation techniques used in Large Language Models.

---

# 📚 Topics Covered

## Introduction to Variational Autoencoders (VAE)

A Variational Autoencoder (VAE) is a probabilistic generative model that learns the underlying distribution of data and generates new samples by sampling from a latent space.

### Key Characteristics

- Learns data distribution
- Generates new similar data
- Introduces probability and randomness into traditional autoencoders

---

## VAE Architecture

### Encoder

- Input: Image/Text
- Produces Mean (μ) and Variance (σ)

Instead of encoding data into a fixed vector, the encoder learns a probability distribution.

---

### Latent Space

The latent vector is sampled from:

z ~ N(μ, σ²)

The latent space stores compressed feature representations that enable the generation of new data.

---

### Reparameterization Trick

Instead of sampling directly,

z = μ + σ × ε

where

ε ~ N(0,1)

This allows gradients to flow during backpropagation.

---

### Decoder

Input:

Latent Vector (z)

Output:

Reconstructed Image/Text

The decoder reconstructs data from the latent representation.

---

## VAE Loss Functions

### Reconstruction Loss

Measures how closely the reconstructed output matches the original input.

Common losses:

- Mean Squared Error (MSE)
- Binary Cross Entropy (BCE)

---

### KL Divergence Loss

Regularizes the latent space by encouraging it to follow a standard normal distribution.

Benefits:

- Smooth latent space
- Meaningful interpolation
- Better sampling

---

### Final Loss

Total Loss = Reconstruction Loss + KL Divergence Loss

---

## Advantages of VAE

- Generates new samples
- Smooth latent space
- Useful for anomaly detection
- Suitable for image generation

---

## Limitation

- Generated images may appear blurry

---

# Autoregressive Models

Autoregressive models generate sequences one token at a time.

Probability formulation:

P(x) = P(x₁) × P(x₂|x₁) × P(x₃|x₁,x₂) ...

Each prediction depends on previously generated tokens.

---

## Working

1. Input the first token
2. Predict the next token
3. Feed the prediction back
4. Repeat until sequence completion

---

## Models Based on Autoregression

- Recurrent Neural Networks (RNN)
- Long Short-Term Memory (LSTM)
- Gated Recurrent Units (GRU)

---

## Challenges

- Vanishing Gradient
- Long-Term Dependency Problems

---

# Generative Pre-trained Transformer (GPT)

GPT is a Transformer Decoder-based language model designed for autoregressive text generation.

---

## GPT Architecture

### Token Embeddings

Converts words into dense vector representations.

---

### Positional Encoding

Adds sequence order information.

---

### Masked Self-Attention

Allows each token to attend only to previous tokens, preserving autoregressive behavior.

---

### Feed Forward Network

Processes contextual representations produced by attention.

---

## Training Objective

Predict the next word:

P(wₜ | w₁, w₂, … , wₜ₋₁)

---

## GPT vs RNN

| Feature | RNN | GPT |
|---------|-----|-----|
| Parallel Processing | No | Yes |
| Long-Term Context | Limited | Strong |
| Training Speed | Slower | Faster |
| Context Understanding | Limited | Better |

---

# Text Generation Techniques

## Greedy Search

Always selects the highest-probability token.

Pros:

- Fast
- Deterministic

Cons:

- Repetitive output

---

## Beam Search

Maintains multiple candidate sequences and selects the best overall result.

Pros:

- Better quality
- More stable

Cons:

- Less diverse

---

## Random Sampling

Samples tokens according to their probability distribution.

Pros:

- More creative

Cons:

- May produce less coherent text

---

## Temperature Sampling

Controls randomness during generation.

Low Temperature:

- Safer
- More deterministic

High Temperature:

- More creative
- More diverse

---

## Top-K Sampling

Selects the next token only from the K most probable tokens.

Balances quality and diversity.

---

## Top-P (Nucleus) Sampling

Selects tokens whose cumulative probability exceeds a threshold P.

Produces more natural and context-aware outputs.

---

# 🛠️ Practical Learning

- Understood the architecture of VAEs.
- Learned probabilistic latent representations.
- Studied the reparameterization trick.
- Explored VAE loss functions.
- Learned autoregressive sequence generation.
- Studied GPT architecture and decoder-only Transformers.
- Compared GPT with RNNs.
- Explored popular text generation decoding strategies.

---

# 📂 Files

- VAE,AUTOREGRESSIVE,GPT,TYPES.ipynb
- README.md
- notes.md
- requirements.txt

---

# 🎯 Learning Outcomes

After completing this session, I can:

- Explain the architecture of VAEs.
- Describe latent space and reparameterization.
- Explain reconstruction and KL divergence losses.
- Understand autoregressive sequence generation.
- Explain GPT architecture.
- Compare GPT and RNN.
- Differentiate Greedy, Beam, Top-K, Top-P, and Temperature Sampling.

---

# 🚀 Outcome

Developed a strong understanding of probabilistic generative models and modern Transformer-based language models, providing a solid foundation for advanced Generative AI systems.
