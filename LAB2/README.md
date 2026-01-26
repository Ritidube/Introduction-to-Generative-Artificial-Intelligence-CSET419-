Experiment 2: Training a Basic GAN for Image Generation Aim

To design, implement, and train a Generative Adversarial Network (GAN) to generate realistic synthetic handwritten digit images using the MNIST dataset, and to evaluate the quality of generated images using Inception Score (IS), and visual comparison.

Objective

The objectives of this experiment are to:

      1. Implement a Generator network that produces fake images from random noise.
      2. Implement a Discriminator network that classifies images as real or fake.
      3. Train both networks in an adversarial manner.
      4. Generate synthetic MNIST images after training.
      5. Evaluate the trained GAN using:
      6. Inception Score (IS)
      7. Side-by-side comparison of real and generated images.
      
Dataset Used

    MNIST Dataset
    60,000 training images
    28 × 28 grayscale handwritten digit images
    Automatically downloaded using Keras dataset utilities
Generative Adversarial Network (GAN)

    Initialize the Generator and Discriminator networks.
    
    Load and normalize the MNIST dataset.
    
    For each training epoch:
    
                Sample random noise vectors.
                
                Generate fake images using the Generator.
                
                Train the Discriminator using both real and fake images.
                
                Train the Generator to fool the Discriminator.
    
    Save generated image samples at regular intervals.
    
    After training:
    
              Generate 100 synthetic images.
              
              Evaluate the GAN using FID and Inception Score.
              
              Perform a visual comparison of real and generated images.

Implementation Details

    Images are normalized to the range [-1, 1]
    
    Binary Cross-Entropy loss function is used
    
    Adam optimizer with a learning rate of 0.0002
    
    Batch size: 128
    
    Noise dimension: 100
    
    Number of epochs: 50
    
    Generated samples are saved every 5 epochs

Results

    The GAN successfully learned the distribution of handwritten digits.
    
    Generated images became clearer and more realistic with increasing epochs.
    
    Inception Score indicated good diversity in generated samples.
    
    Visual comparison confirmed that generated images resemble real MNIST digits.
