# Autoencoder and Variational Autoencoder for Image Reconstruction

## Practical No. 03 – Generative AI

**Student Name:** Mit Jangid  
**PRN:** 202401110072  
**Batch:** A1

## 📌 Project Overview

This project implements and compares two deep learning models, a Convolutional Autoencoder and a Variational Autoencoder (VAE), for handwritten digit image reconstruction and generation.

The models are trained using the MNIST dataset, which contains grayscale images of handwritten digits from 0 to 9.

The project explores how neural networks learn compressed latent representations and use them to reconstruct existing images or generate new digit-like images.

## 📂 Dataset

**Dataset:** MNIST Handwritten Digits

- 60,000 training images
- 10,000 testing images
- Image dimensions: 28 × 28 pixels
- 10 digit classes (0–9)
- Grayscale images

Pixel values are normalized to the range [0, 1].

## 🧠 Models Implemented

### 1. Convolutional Autoencoder

- Encoder compresses input images into a 32-dimensional latent representation.
- Decoder reconstructs the original images.
- Uses convolutional and transposed convolutional layers.
- Trained using Binary Cross-Entropy loss.

### 2. Variational Autoencoder (VAE)

- Encoder learns the latent mean and log-variance.
- Uses a 16-dimensional latent space.
- Implements the reparameterization trick.
- Decoder reconstructs images from sampled latent vectors.
- Uses reconstruction loss and KL divergence.

## ⚙️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

## 📊 Evaluation and Visualizations

The implementation includes:

1. Original vs reconstructed image comparison.
2. Autoencoder reconstruction results.
3. VAE reconstruction results.
4. New handwritten digit generation.
5. Mean Squared Error (MSE) comparison.
6. Training and validation loss graphs.
7. KL divergence analysis.
8. Latent space visualization using PCA.

## 📁 Repository Structure

```text
GenAI-Practical-03/
│
├── Mit_Jangid_Autoencoder_VAE_MNIST.ipynb
└── README.md
```

## ▶️ How to Run

1. Clone or download this repository.
2. Open the `.ipynb` notebook in Google Colab.
3. Select a GPU runtime if available.
4. Run all cells sequentially.
5. Observe the reconstruction results, generated images and evaluation graphs.

## 📈 Results

The notebook generates the actual reconstruction metrics, training curves, image comparisons and VAE-generated samples.

The quantitative comparison is available in the notebook output.

## 🎯 Conclusion

The practical demonstrates the working of deterministic and probabilistic latent representations using Autoencoders and Variational Autoencoders.

The Convolutional Autoencoder focuses on image reconstruction, whereas the VAE learns a probabilistic latent space that also enables generation of new handwritten digit-like images.

## 📚 References

1. MNIST Handwritten Digits Dataset – http://yann.lecun.com/exdb/mnist/
2. Kingma, D. P. and Welling, M. (2014). Auto-Encoding Variational Bayes.
3. TensorFlow Documentation – https://www.tensorflow.org/
