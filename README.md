# Mathematical Foundations of Convolutional Neural Networks using MNIST

## Overview

This project explores the mathematical foundations of Convolutional Neural Networks (CNNs) through handwritten digit recognition on the MNIST dataset.

Rather than treating CNNs as black-box models, the goal of this project was to understand how convolution, pooling, activation functions, backpropagation, and gradient-based optimization work mathematically and how these components contribute to image classification performance.

The project combines theoretical derivations with practical implementation using TensorFlow/Keras.

---

## Objectives

* Understand the mathematical foundations of CNNs
* Derive convolution, pooling, and backpropagation operations
* Implement a CNN architecture from first principles
* Evaluate CNN performance on handwritten digit classification
* Connect theoretical concepts with practical deep learning implementation

---

## Dataset

### MNIST Handwritten Digits Dataset

The MNIST dataset contains:

* 70,000 grayscale images
* 10 digit classes (0–9)
* Image size: 28 × 28 pixels

The dataset serves as a benchmark for evaluating image classification algorithms and understanding CNN behavior.

---

## CNN Architecture

The implemented CNN consists of:

### Feature Extraction

* Convolution Layer (32 filters)
* ReLU Activation
* Convolution Layer (64 filters)
* ReLU Activation
* Max Pooling
* Dropout Regularization

### Classification

* Flatten Layer
* Fully Connected Layer (128 neurons)
* ReLU Activation
* Dropout Regularization
* Softmax Output Layer

Total parameters:

* 1,199,882 trainable parameters

---

## Mathematical Concepts Explored

### Convolution

Feature extraction using learnable kernels:

$$
S(i,j)=(I*K)(i,j)
$$

Used to detect edges, textures, and spatial patterns within images.

### Stride

Investigated how filter movement influences feature map generation and computational complexity.

### Padding

Studied the effect of preserving spatial information during convolution operations.

### Pooling

Implemented Max Pooling to:

* Reduce feature map size
* Reduce computational cost
* Improve translation robustness

### Backpropagation

Derived gradients for:

* Fully connected layers
* Convolutional layers
* Pooling layers

using the chain rule and gradient descent optimization.

---

## Training Configuration

* Framework: TensorFlow / Keras
* Optimizer: Adadelta
* Learning Rate Scheduler: Exponential Decay
* Batch Size: 64
* Epochs: 5
* Loss Function: Categorical Cross-Entropy
* Activation Functions: ReLU and Softmax

---

## Results

### Final Performance

| Metric            | Value  |
| ----------------- | ------ |
| Training Accuracy | 98.78% |
| Test Accuracy     | 99.12% |
| Validation Loss   | 0.029  |

The model achieved over 99% test accuracy on MNIST while maintaining a relatively simple architecture.

---

## Key Insights

* CNNs automatically learn hierarchical visual features through convolutional operations.
* Pooling layers reduce computational complexity while preserving important information.
* Backpropagation enables efficient optimization of convolutional filters.
* Understanding mathematical foundations is essential for interpreting and improving deep learning models.
* Model performance depends not only on architecture design but also on optimization and feature learning dynamics.

---

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn

---

## Skills Demonstrated

* Deep Learning
* Computer Vision
* Convolutional Neural Networks
* Backpropagation
* Gradient Descent
* Mathematical Modeling
* TensorFlow
* Keras
* Image Classification
* Feature Extraction
* Model Training & Evaluation

---

## Author

**Tsukasa Miyaji**
University of California, Los Angeles (UCLA)

