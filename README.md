# Vanilla GAN Image Generation

This project implements a Vanilla Generative Adversarial Network (GAN) using PyTorch to generate images.

## Project Overview

A GAN consists of two neural networks:

- **Generator** - Creates fake images from random noise.
- **Discriminator** - Determines whether an image is real or generated.

Both networks are trained together so that the Generator gradually learns to create more realistic images.

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib


## Model Architecture

### Generator

The Generator takes a random noise vector of size 100 and generates a `64 × 64` RGB image.

```text
Random Noise (100)
        ↓
Linear Layer
        ↓
256
        ↓
512
        ↓
1024
        ↓
64 × 64 × 3
        ↓
Generated Image