# CIFAR-10-Image-Classifier-with-Convolutional-Neural-Networks

# Project Overview

This project implements a **Convolutional Neural Network (CNN)** from scratch using PyTorch to classify images from the **CIFAR-10 dataset**. The model achieves competitive accuracy by learning hierarchical features through multiple convolutional layers, making it an excellent demonstration of deep learning fundamentals for image classification tasks.

CIFAR-10 is a well-known benchmark dataset consisting of **60,000 32×32 color images** across **10 different classes**: airplanes, automobiles, birds, cats, deer, dogs, frogs, horses, ships, and trucks.

## Key Features

->  **Custom CNN Architecture** with 3 convolutional layers and fully connected layers
->  **Training and Evaluation Pipeline** with loss tracking and accuracy metrics
->  **Data Augmentation** using PyTorch transforms (normalization, tensor conversion)
->  **Model Persistence** - Save and load trained models
->  **Prediction Interface** - Test on custom 32×32 images with accuracy evaluation

##  Model Architecture

CNN Architecture:
->Conv Layer 1: 3 → 32 filters, 3×3 kernel, ReLU, MaxPool 2×2
-> Conv Layer 2: 32 → 64 filters, 3×3 kernel, ReLU, MaxPool 2×2
-> Conv Layer 3: 64 → 128 filters, 3×3 kernel, ReLU, MaxPool 2×2
-> Flatten Layer
-> Fully Connected Layers:
-> Linear: 128×4×4 → 256 neurons, ReLU
-> Linear: 256 → 10 neurons (output classes)
