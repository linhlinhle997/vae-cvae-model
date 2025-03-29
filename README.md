# VAE & CVAE Models

## Introduction

This project implements two types of autoencoders for data generation:
- **VAE (Variational Autoencoder)**: Trained on **MNIST** for image generation.
- **CVAE (Conditional Variational Autoencoder)**: Trained on **audio data** for conditional generation.

Both models run on **Google Colab** for easy execution.

## What is a VAE?
A **Variational Autoencoder (VAE)** is a generative model that learns to encode input data into a **latent space** and then reconstruct it. Unlike regular autoencoders, VAEs introduce a probabilistic approach, allowing them to generate new data.

### How VAE Works:
- **Encoder**: Converts input data into a probability distribution.
- **Latent Space**: A compressed representation used for sampling.
- **Decoder**: Reconstructs data from the latent representation.
- **Reparameterization Trick**: Helps smooth learning of the latent variables.
- **Loss Function**: Combines **Reconstruction Loss** (for accuracy) and **KL Divergence** (for a smooth latent space).

## What is a CVAE?
A **Conditional Variational Autoencoder (CVAE)** is an extension of VAE that includes **conditional labels** as extra inputs. This allows for more controlled generation of data.

### How CVAE Works:
- **Conditional Inputs**: Labels are used to guide the generation process.
- **Encoder**: Maps input + label to a probability distribution in latent space.
- **Latent Space**: Learns meaningful representations based on conditions.
- **Decoder**: Reconstructs data using the latent vector and condition.
- **Reparameterization Trick**: Ensures smooth learning.
- **Loss Function**: Balances **Reconstruction Loss** and **KL Divergence** for structured generation.
- **Targeted Generation**: Generates specific outputs based on conditions.

## Features
- Train **VAE** on the MNIST dataset for image generation.
- Train **CVAE** on an audio dataset for **conditional** audio generation.
- Generate new data by sampling from the latent space.
- Visualize and evaluate reconstruction quality.

## How to Use
1. **Open Google Colab**
2. **Upload the notebook** or run it directly from the repository.
3. **Run all cells** to:
   - Install dependencies.
   - Download and prepare the dataset.
   - Train the model and view results.

## Results
- **VAE (MNIST)**: Generates new handwritten digits.
- **CVAE (Audio)**: Generates audio samples based on given conditions.

