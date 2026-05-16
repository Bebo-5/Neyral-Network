# Handwritten Digit Recognition using MLP Neural Network

## Project Description
This project implements a Multilayer Perceptron (MLP) Neural Network for handwritten digit recognition using the MNIST dataset.  
The project was developed using PyTorch and includes data preprocessing, model training, evaluation, experimentation, and visualization.

The objective of the project is to classify handwritten digits (0–9) with high accuracy using deep learning techniques.

---

## Dataset
The project uses the MNIST dataset:

- Dataset Name: MNIST Handwritten Digits
- Number of Classes: 10
- Image Size: 28x28 grayscale images

Dataset Link:  
https://pytorch.org/vision/stable/generated/torchvision.datasets.MNIST.html

The dataset is automatically downloaded using torchvision.

---

## Technologies Used

- Python
- PyTorch
- NumPy
- Matplotlib
- Torchvision

---

## Data Preprocessing

The following preprocessing steps were applied:

- Converting images to tensors
- Normalization using:
  
Splitting dataset into:
Training Set
Validation Set
Testing Set
Model Architecture

The implemented model is a Multilayer Perceptron (MLP) consisting of:

Input Layer:
784 neurons (28×28 image flattened)
Hidden Layers:
Experiment 1: [128, 64]
Experiment 2: [512, 256]
Output Layer:
10 neurons (digits 0–9)
Activation Function
ReLU
Loss Function
CrossEntropyLoss
Optimizer
Adam Optimizer
Experiments

Two experiments were conducted to compare model performance.

Experiment 1 (Baseline)
Hidden Layers: [128, 64]
Learning Rate: 0.001
Dropout: No
Batch Normalization: No
Experiment 2 (Enhanced)
Hidden Layers: [512, 256]
Learning Rate: 0.0005
Dropout: Yes
Batch Normalization: Yes
Results
Experiment	Test Accuracy	Final Loss
Experiment 1	97.67%	0.1002
Experiment 2	98.27%	0.0584
Best Model

Experiment 2 achieved the best performance with:

Accuracy: 98.27%
Loss: 0.0584
Visualizations

The project includes:

Training vs Validation Loss Curves
Training vs Validation Accuracy Curves

These visualizations help monitor model performance during training.

Regularization Techniques

The following enhancement techniques were used:

Dropout

Used to reduce overfitting.

Batch Normalization

Used to improve training stability and convergence speed.

Project Structure
