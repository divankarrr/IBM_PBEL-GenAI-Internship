# Day 15 Notes

## What are Generative Models?

Generative Models learn the probability distribution of data and generate new samples that resemble the training data.

Examples:

- Human Face Generation
- Music Generation
- AI Art
- Text Generation
- Data Augmentation

---

# Types of Generative Models

### 1. Explicit Density Models

Example:

- Naïve Bayes

---

### 2. Latent Variable Models

Example:

- Variational Autoencoder (VAE)

---

### 3. Implicit Models

Example:

- Generative Adversarial Networks (GAN)

---

# What is GAN?

GAN stands for **Generative Adversarial Network**.

It consists of two competing neural networks:

- Generator (G)
- Discriminator (D)

The Generator tries to create realistic fake data, while the Discriminator tries to distinguish between real and fake data.

---

# Generator

Input:

Random Noise (z)

Output:

Fake Data

Goal:

Generate highly realistic samples.

---

# Discriminator

Input:

Real or Fake Data

Output:

Probability

Real = 1

Fake = 0

Goal:

Correctly classify input samples.

---

# GAN Architecture

Random Noise

↓

Generator

↓

Fake Image

↓

Discriminator

↓

Real / Fake Prediction

---

# Training Process

1. Generate random noise.
2. Generator creates fake samples.
3. Discriminator receives both real and fake samples.
4. Compute discriminator loss.
5. Update discriminator weights.
6. Update generator weights.
7. Repeat until convergence.

---

# Minimax Objective

Generator:

Minimize discriminator's ability to detect fake samples.

Discriminator:

Maximize classification accuracy.

Both networks improve together through adversarial training.

---

# GAN Loss Functions

## Discriminator Loss

- Maximize probability for real images.
- Minimize probability for fake images.

---

## Generator Loss

- Fool the discriminator.
- Produce realistic outputs.

---

# Challenges of GAN

## Mode Collapse

Generator repeatedly produces similar outputs.

---

## Training Instability

Generator and discriminator may fail to converge.

---

## Vanishing Gradient

Weak gradients prevent effective learning.

---

# GAN Variants

## Vanilla GAN

Basic adversarial learning framework.

---

## DCGAN

Uses Convolutional Neural Networks.

Advantages:

- Better image quality
- Stable training

Applications:

- Face Generation
- Image Generation

---

## CycleGAN

Image-to-image translation without paired datasets.

Examples:

- Horse ↔ Zebra
- Summer ↔ Winter

Applications:

- Style Transfer
- Domain Adaptation

---

## Conditional GAN (cGAN)

Uses additional labels to guide generation.

Examples:

Digit = 5 → Generate handwritten digit "5"

Applications:

- Controlled image synthesis
- Text-to-image generation

---

# Applications of GAN

- Face Generation
- Image Generation
- AI Art
- Super Resolution
- Medical Imaging
- Data Augmentation
- Video Generation
- Fashion Design
- Game Development

---

# Key Takeaways

✔ GANs are one of the most important Generative AI architectures.

✔ A GAN consists of a Generator and a Discriminator trained together.

✔ The Generator creates realistic synthetic data from random noise.

✔ The Discriminator distinguishes between real and fake samples.

✔ GAN training follows a minimax optimization strategy.

✔ Common GAN challenges include mode collapse, training instability, and vanishing gradients.

✔ Advanced GAN variants such as DCGAN, CycleGAN, and Conditional GAN extend GANs for image generation, style transfer, and controlled content generation.
