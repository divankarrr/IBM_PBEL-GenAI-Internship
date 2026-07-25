# Day 17 Notes

## What are Diffusion Models?

Diffusion Models are Generative AI models that learn to generate new images by gradually removing noise from random Gaussian noise.

Instead of generating an image directly, they learn the reverse of a noise corruption process.

---

# Forward Diffusion Process

The forward process gradually adds Gaussian noise to an image until it becomes pure noise.

Formula:

xt = √αt · x₀ + √(1 − αt) · ε

Where:

- x₀ → Original Image
- xt → Noisy Image
- ε → Random Gaussian Noise
- αt → Noise Schedule

---

# Noise Scheduling

Noise scheduling controls how much noise is added at each timestep.

Common schedules:

- Linear
- Cosine
- Quadratic

---

# Beta Schedule

Beta determines the amount of noise added during each timestep.

Small beta:

- Less noise

Large beta:

- More noise

---

# Alpha

Alpha = 1 − Beta

Alpha represents how much original information remains after adding noise.

---

# Alpha Hat

Alpha Hat is the cumulative product of alpha values.

It represents the total amount of original signal preserved after multiple timesteps.

---

# Reverse Diffusion Process

The model learns to remove noise one step at a time.

Instead of predicting the image, it predicts the noise that was added.

---

# Loss Function

Mean Squared Error (MSE)

Loss = ||Actual Noise − Predicted Noise||²

The objective is to minimize the difference between the true noise and the predicted noise.

---

# U-Net Architecture

U-Net is the backbone of most diffusion models.

Main components:

- Encoder
- Bottleneck
- Decoder
- Skip Connections

Benefits:

- Preserves image details
- Captures local and global features

---

# Time Embeddings

Time embeddings inform the network about the current diffusion timestep.

This helps the model learn different denoising operations for different noise levels.

---

# Stable Diffusion

Stable Diffusion performs diffusion in latent space instead of pixel space.

Components:

### VAE

Compresses images into latent vectors.

### U-Net

Removes noise from latent representations.

### Text Encoder

Converts text prompts into embeddings for text-to-image generation.

---

# Practical Implementation

Implemented:

- MNIST Dataset loading
- Image normalization
- Beta schedule creation
- Alpha and Alpha Hat calculation
- Simple U-Net model
- Forward diffusion
- Reverse denoising training loop
- MSE Loss optimization

---

# Applications

- AI Image Generation
- Text-to-Image Generation
- Image Editing
- Inpainting
- Image Super Resolution
- Medical Imaging
- Creative Design

---

# Key Takeaways

✔ Diffusion Models generate images by reversing a noise process.

✔ Forward diffusion gradually corrupts images with Gaussian noise.

✔ Reverse diffusion reconstructs images by removing noise.

✔ U-Net is the core neural network used for denoising.

✔ Stable Diffusion operates in latent space using a VAE, U-Net, and Text Encoder.

✔ PyTorch provides an effective framework for implementing diffusion models.
