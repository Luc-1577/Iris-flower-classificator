# Neural Network for Iris Dataset Classification

This project implements a simple neural network using PyTorch to classify the Iris dataset into three species: Setosa, Versicolor, and Virginica.

## Overview

The Iris dataset is a well-known dataset in machine learning, containing 150 samples of iris flowers with four numerical features: sepal length, sepal width, petal length, and petal width. This project trains a neural network to classify these samples into their respective species.

## Installation

Ensure you have Python installed (recommended version: 3.8+). Then, install the required libraries manually:

```bash
pip install torch scikit-learn matplotlib
```

## Model Architecture

The neural network consists of:

- **Input layer:** 4 features
- **Hidden layer 1:** 8 neurons
- **Hidden layer 2:** 8 neurons
- **Output layer:** 3 neurons (corresponding to the three iris species)
- **Activation function:** ReLU

## Training

The model is trained using:

- **Loss function:** CrossEntropyLoss
- **Optimizer:** Adam with a learning rate of 0.01
- **Epochs:** 100

During training, the model prints the error rate every 10 epochs.

## Evaluation

After training, the model is tested on a separate test set (20% of the data). The final error rate is computed without gradient adjustments to assess performance.

## Results

The trained model achieves high accuracy, correctly classifying 29 out of 30 test samples.
