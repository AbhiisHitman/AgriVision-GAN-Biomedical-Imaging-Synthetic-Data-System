Overview

This project focuses on addressing data scarcity and class imbalance in medical imaging by generating high-quality synthetic images using Generative Adversarial Networks (GANs). The generated dataset is used to improve the performance of deep learning models for classification tasks.

Problem Statement

Medical imaging datasets are often limited in size and suffer from class imbalance, which negatively impacts the performance and generalization of deep learning models. Collecting large-scale labeled medical data is expensive and time-consuming.

Solution

This project uses a GAN-based approach to generate synthetic medical images that augment the original dataset. The expanded dataset is then used to train convolutional neural networks (CNNs) for improved classification performance.

Key Features
GAN-based synthetic image generation
Dataset expansion by 28.9× (50,000+ images generated)
Improved classification using transfer learning (DenseNet-121)
High-performance metrics on augmented dataset
End-to-end pipeline from data generation to model evaluation
Methodology
1. Data Preparation
Preprocessed input medical imaging dataset
Handled normalization and resizing for training
2. GAN Training
Implemented DCGAN architecture
Trained generator and discriminator networks
Generated synthetic images to augment dataset
3. Model Training
Applied transfer learning using CNN architectures
Fine-tuned DenseNet-121 for classification
4. Evaluation
Evaluated model using accuracy and AUC-ROC
Compared performance before and after augmentation
Results
Generated over 50,000 synthetic images
Achieved 28.9× dataset expansion
Accuracy: 99.46%
AUC-ROC: 0.9999
Project Structure
agrivision-gan-synthetic-data/
├── agrivision_gan.ipynb
├── outputs/
│   ├── generated_samples.png
│   ├── training_graph.png
├── README.md
├── requirements.txt
Outputs
Generated Samples

Training Performance

Tech Stack
Python
PyTorch
NumPy
Matplotlib
Scikit-learn
DCGAN
CNN (DenseNet-121)
How to Run
Clone the repository

Install dependencies:

pip install -r requirements.txt

Launch the notebook:

jupyter notebook agrivision_gan.ipynb
