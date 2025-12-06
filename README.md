🧠 MNIST Digit Generation using GAN (Generative Adversarial Network)

This project implements a Generative Adversarial Network (GAN) from scratch in TensorFlow/Keras to generate handwritten digits similar to the MNIST dataset.
The GAN consists of a Generator and Discriminator trained in an adversarial setup, enabling the model to learn the distribution of real digit images and generate new synthetic samples.

✨ Features

✔ Trains a custom GAN using MNIST
✔ Generator built with Dense + BatchNorm + LeakyReLU
✔ Discriminator built with Dense + LeakyReLU layers
✔ Adversarial training loop implemented manually
✔ Generates new 28×28 grayscale digit images
✔ Live image sampling every few epochs
✔ Clean and simple implementation for beginners & students

🧠 Tech Stack

Python

TensorFlow / Keras

NumPy

Matplotlib

📌 How It Works
1️⃣ Load & Normalize MNIST

Images are scaled to the range [-1, 1] for GAN stability.

2️⃣ Generator Network

Takes 100-dim noise → outputs a 28×28×1 digit image.

3️⃣ Discriminator Network

Classifies images as real or fake.

4️⃣ GAN Model

Freezes the discriminator and trains the generator to fool it.

5️⃣ Training Loop

Train discriminator on real + fake images

Train generator through GAN

Sample and display generated images at intervals

📁 Project Structure
├── main.ipynb / main.py     # Full GAN implementation
├── sample_images()          # Continuously generates digit samples
└── README.md

🚀 Future Improvements

Upgrade to DCGAN (Convolutional layers)

Add model checkpoints

Generate high-resolution images

Create UI using Streamlit
