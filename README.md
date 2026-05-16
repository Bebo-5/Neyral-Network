# Handwritten Digit Recognition using MLP Neural Network

## Overview
This project implements a Multilayer Perceptron (MLP) Neural Network using PyTorch to classify handwritten digits from the MNIST dataset.  
The project includes data preprocessing, model training, evaluation, experimentation, and visualization of results.

---

# Dataset

Dataset: MNIST Handwritten Digits Dataset

- 70,000 grayscale images
- Image size: 28 × 28 pixels
- 10 classes (digits from 0 to 9)

Dataset Link:  
https://pytorch.org/vision/stable/generated/torchvision.datasets.MNIST.html

---

# Features

- Data preprocessing and normalization
- Training / Validation / Testing split
- Multilayer Perceptron (MLP) implementation
- Multiple experiments for comparison
- Accuracy and loss tracking
- Visualization of training results
- Dropout and Batch Normalization support

---

# Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib

---

# Data Preprocessing

The following preprocessing steps were applied:

- Converting images to tensors
- Normalization using:

```python
transforms.Normalize((0.1307,), (0.3081,))
Splitting dataset into:
Training set
Validation set
Testing set
Model Architecture

The implemented model is a Multilayer Perceptron (MLP) containing:

Input Layer:
784 neurons
Hidden Layers:
Configurable hidden layers
Output Layer:
10 neurons
Activation Functions
ReLU
Tanh
Sigmoid
Loss Function
CrossEntropyLoss
Optimizer
Adam Optimizer
Experiments
Experiment 1 (Baseline)
Parameter	Value
Hidden Layers	[128, 64]
Learning Rate	0.001
Dropout	No
Batch Normalization	No
Experiment 2 (Enhanced)
Parameter	Value
Hidden Layers	[512, 256]
Learning Rate	0.0005
Dropout	Yes
Batch Normalization	Yes
Results
Experiment	Accuracy	Final Loss
Experiment 1	97.67%	0.1002
Experiment 2	98.27%	0.0584
Best Model

Experiment 2 achieved the best performance.

Visualizations

The project includes:

Training vs Validation Loss Curves
Training vs Validation Accuracy Curves

These visualizations help analyze model learning performance.

Regularization Techniques

The following techniques were used:

Dropout

Used to reduce overfitting.

Batch Normalization

Used to improve training stability and model convergence.

Project Structure
How to Run the Project
1. Clone the Repository
https://github.com/Bebo-5/Neyral-Network
2. Navigate to Project Folder
cd your-repository-name
3. Install Required Libraries
pip install torch torchvision matplotlib numpy
4. Run the Notebook or Python File
python main.p
