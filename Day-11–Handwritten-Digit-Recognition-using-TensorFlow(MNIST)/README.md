# Day 11 – Handwritten Digit Recognition using TensorFlow (MNIST)

📅 **Date:** 30 June 2026

## 🎯 Objective

Build and evaluate a Deep Learning model for handwritten digit recognition using the MNIST dataset. Compare the performance of Artificial Neural Networks (ANNs) with traditional Machine Learning algorithms such as Logistic Regression and Support Vector Machines (SVM) using Principal Component Analysis (PCA).

---

# 📚 Topics Covered

## Dataset

- MNIST Handwritten Digit Dataset
- Training Dataset
- Testing Dataset
- Image Normalization

---

## TensorFlow & Keras

- Sequential API
- Functional API
- Dense Layers
- Flatten Layer
- ReLU Activation
- Softmax Activation

---

## Neural Network Design

- Input Layer
- Hidden Layer
- Output Layer
- Model Summary
- Trainable Parameters

---

## Model Training

- Adam Optimizer
- Sparse Categorical Crossentropy
- Accuracy Metric
- Validation Split
- Epochs

---

## Model Evaluation

- Test Accuracy
- Test Loss
- Classification Report
- Confusion Matrix

---

## Machine Learning Comparison

- Logistic Regression
- Principal Component Analysis (PCA)
- Support Vector Machine (SVM)

---

# 🛠️ Practical Activities

### 1. Imported Required Libraries

Imported TensorFlow, Matplotlib, Seaborn, NumPy and Scikit-learn.

---

### 2. Loaded MNIST Dataset

Loaded the handwritten digit dataset using TensorFlow.

Normalized pixel values from **0–255** to **0–1** for faster convergence.

---

### 3. Visualized Sample Images

Displayed sample handwritten digits to understand the dataset.

---

### 4. Built ANN using Sequential API

Architecture:

Input (28×28)

↓

Flatten Layer

↓

Dense (128, ReLU)

↓

Dense (10, Softmax)

---

### 5. Built ANN using Functional API

Implemented the same neural network using TensorFlow Functional API.

---

### 6. Compiled the Model

Optimizer:

- Adam

Loss Function:

- Sparse Categorical Crossentropy

Metric:

- Accuracy

---

### 7. Trained the Model

- 10 Epochs
- Validation Split = 20%

Observed improvement in training and validation accuracy.

---

### 8. Evaluated the Model

Generated:

- Test Accuracy
- Test Loss

---

### 9. Classification Report

Calculated:

- Precision
- Recall
- F1-score
- Support

for all digit classes.

---

### 10. Confusion Matrix

Visualized prediction performance using Seaborn heatmap.

---

### 11. Deep ANN

Implemented another neural network with two hidden layers.

Architecture:

784

↓

254

↓

128

↓

10

---

### 12. Logistic Regression

Applied Logistic Regression directly on flattened MNIST images.

---

### 13. PCA

Reduced dimensionality from

784 Features

↓

100 Features

---

### 14. Support Vector Machine

Applied SVM on PCA-transformed features.

Compared its performance with ANN.

---

# 📂 Files

- MNIST_Neural_Network_Predictin_with_Tensorflow.ipynb
- README.md
- notes.md
- requirements.txt

---

# 🎯 Learning Outcomes

After completing this notebook, I can:

- Load and preprocess image datasets.
- Build ANN models using Sequential API.
- Build ANN models using Functional API.
- Train Deep Learning models.
- Evaluate classification models.
- Interpret confusion matrices.
- Understand PCA for dimensionality reduction.
- Compare Deep Learning with classical Machine Learning models.

---

# 🚀 Outcome

Successfully implemented handwritten digit recognition using TensorFlow and compared ANN performance with Logistic Regression and Support Vector Machines, gaining practical experience in image classification and model evaluation.
