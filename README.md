# Handwritten Digit Recognition — CNN (MNIST)

A Convolutional Neural Network built with TensorFlow/Keras to classify handwritten digits (0–9) with **~99% test accuracy**.

---

## Overview

This project implements an end-to-end deep learning pipeline for digit recognition using the MNIST dataset — covering preprocessing, model training, evaluation, and model export.

---

## Key Features

- Custom CNN with Batch Normalization & Dropout  
- Optimized training using EarlyStopping & ReduceLROnPlateau  
- Achieves ~99% accuracy on test data  
- Visualization of training curves & confusion matrix  
- Analysis of misclassified samples  
- Model saved in `.keras` and `.h5` formats  

---

## Tech Stack

- TensorFlow / Keras  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn  
- Jupyter Notebook  

---

## Dataset

- MNIST: 70,000 grayscale images (28×28)  
- 10 classes (digits 0–9)  
- Loaded via `keras.datasets.mnist`  

---

## Model Architecture

```
Input (28×28×1)
→ Conv2D(32) ×2 → BatchNorm → MaxPool → Dropout
→ Conv2D(64) ×2 → BatchNorm → MaxPool → Dropout
→ Dense(256) → BatchNorm → Dropout
→ Output (Softmax)
```

---

## Results

| Metric | Value |
|---|---|
| Accuracy | ~99% |
| Loss | < 0.05 |
| Epochs | ≤ 10 |

---

## Usage

```bash
jupyter notebook Handwritten.ipynb
```

Model is automatically trained and saved on execution.

---

## Project Structure

```
├── Handwritten.ipynb
└── README.md
```
