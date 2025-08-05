# Image-to-Text Generation Using Diffusion Models, CNNs, and GANs

This project investigates deep generative and discriminative models for the task of translating visual input into natural language descriptions. Using the CIFAR-10 dataset, I compare the ability of CNNs, GANs, and diffusion models.

<img width="719" height="812" alt="image" src="https://github.com/user-attachments/assets/f382cad1-f358-4d3e-99f4-df3ca3a08e1a" />


## Objectives

- Evaluate performance of three model families in visual-to-text transformation.
- Benchmark text quality using confusion matrix
- Explore hybrid architectures that combine visual encoding with language generation.

## Dataset

- **CIFAR-10** (Canadian Institute for Advanced Research):
  - 60,000 labeled 32x32 color images in 10 classes.
  - 50,000 training and 10,000 testing samples.
  - Includes airplanes, birds, cats, dogs, trucks, etc.

### Model Architectures

- **Convolutional Neural Networks (CNNs):**
  - Serve as encoders for feature extraction
  - Outputs flattened to specfic classifiaction

- **Generative Adversarial Networks (GANs):**
  - Generator learns latent image-to-caption mapping by generating noise
  - Discriminator classifies real vs generated captions
  - Training involves adversarial loss 

- **Diffusion Models:**
  - Start from noise and denoise iteratively using a learned reverse process
  - Captions generated via conditional denoising pipeline
  - Yield highly detailed outputs

