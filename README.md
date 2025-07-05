# Feedforward Neural Network for Multi-Class Classification

## Project Overview

This project implements a simple yet effective **Feedforward Neural Network (FNN)** using **TensorFlow/Keras** to perform a multi-class classification task. The model is trained on a dataset with 14 input features and aims to classify samples into one of three distinct categories.

The project emphasizes handling class imbalance, model interpretability, and systematic training and evaluation using standard deep learning workflows.

---

## Key Features

- Developed a **Fully Connected Neural Network (FNN)** with the following architecture:
  - **Input Layer:** 14 features
  - **Hidden Layer:** Dense layer with 9 neurons and ReLU activation
  - **Output Layer:** Dense layer with 3 neurons and softmax activation for multi-class classification

- **Model Compilation:**
  - Optimizer: `Adam`
  - Loss Function: `Sparse Categorical Crossentropy` (for integer-encoded class labels)
  - Metrics: `Accuracy`

- **Handling Class Imbalance:**
  - Applied custom class weights: `{0: 1, 1: 5.6, 2: 9.4}` to address skewed class distribution and improve model robustness across all classes.

- **Training Setup:**
  - Batch Size: 32
  - Epochs: 200
  - 20% validation split for performance monitoring during training

- **Evaluation:**
  - Final model evaluated on test data
  - Predictions extracted using softmax output and `argmax` for class label assignment

- **Data Preprocessing:**
  - Standardization applied using `StandardScaler`
  - Train-test split implemented to ensure unbiased evaluation

---

---

## ⚙Python Libraries Used

- Python 3.x
- TensorFlow / Keras
- NumPy, Pandas
- Scikit-learn
- Matplotlib, Seaborn (for potential visualizations)

---

## Potential Improvements

Hyperparameter tuning using Grid Search or Random Search

Addition of more complex network architectures (e.g., additional hidden layers, dropout)

Evaluation using advanced metrics like F1-score, precision-recall curves

Enhanced visualizations for deeper performance insights

---
