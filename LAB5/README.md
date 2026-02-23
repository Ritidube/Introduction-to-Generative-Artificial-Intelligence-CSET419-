Image-to-Image Translation (CNN vs GAN)
CSET419 – Generative AI Lab 5
Overview

    This project implements image reconstruction using:
        Baseline Encoder–Decoder CNN
        GAN-based Encoder–Decoder
The objective is to compare reconstruction quality using pixel-wise loss (CNN) and adversarial learning (GAN).
The experiment is performed on the CIFAR-10 dataset (32×32 RGB images).

Models

    1. Baseline CNN

            Encoder–Decoder architecture

            Trained using MSE / L1 loss

            Produces smooth but slightly blurry outputs
    
    2. GAN Model

            Generator (Encoder–Decoder)

            Discriminator (Real vs Fake classifier)

            Uses Adversarial + L1 loss

            Produces sharper and more realistic images

Observations

    CNN minimizes pixel error → causes smoothing.

    GAN improves edge clarity and texture details.

    GAN outputs appear more visually realistic than CNN outputs.
