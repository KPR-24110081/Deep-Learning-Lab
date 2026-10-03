# Experiment 7: Autoencoders and Variational Autoencoders

This experiment explores unsupervised representation learning through autoencoders and variational autoencoders (VAEs). The focus is on reconstructing images, denoising corrupted inputs, analyzing latent spaces, and comparing different model architectures.

## Objective

- Understand the principles of autoencoder-based compression and reconstruction.
- Compare fully connected and convolutional autoencoders.
- Study denoising behavior under noisy inputs.
- Implement a VAE and analyze generative latent representations.
- Evaluate reconstruction quality and latent-space structure.

## Dataset

The experiment is based on image datasets commonly used for reconstruction and denoising tasks, with emphasis on MNIST-like digit data and noisy variants. The notebook analyzes how autoencoders handle compressed latent representations and noise suppression.

## Model types explored

- Fully connected autoencoder
- Convolutional autoencoder
- Variational autoencoder (VAE)

## Core concepts covered

- Encoder-decoder architecture
- Latent embeddings
- Reconstruction loss
- Denoising capability
- Latent dimension sensitivity
- Variational latent sampling
- Image generation from learned latent space

## Evaluation metrics

- MSE
- MAE
- SSIM
- Reconstruction error distributions
- Noise sensitivity analysis
- Latent dimension vs reconstruction fidelity

## Files in this folder

- `DL_Lab_7.ipynb` — notebook with autoencoder and VAE experiments
- `Ex_7.pdf` — report/exported writeup
- `plots/` — visual outputs and model analysis
- `README.md` — experiment summary

## Visualizations included

- Clean vs noisy images
- Clean vs noisy vs denoised comparison
- Fully connected autoencoder loss
- Convolutional autoencoder loss
- Original vs reconstructed images
- High-error image analysis
- Latent dimension vs MSE
- Latent dimension vs SSIM
- Noise level vs MAE/MSE/SSIM
- VAE generated images
- VAE latent space visualization
- VAE latent interpolation
- VAE training loss

## Outcome

The experiment demonstrates that autoencoders can effectively learn compressed data representations and remove noise, while VAEs extend this idea by learning a probabilistic latent space that supports generative sampling and latent interpolation.
