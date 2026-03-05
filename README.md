# Multiclass Image Classification using CNN and Transfer Learning

## Overview

This project implements a **Custom Convolutional Neural Network (CNN)** and a **pretrained MobileNetV2 model** to perform multiclass image classification on the **CIFAR-10 dataset**.
The objective is to compare the performance of a custom CNN model with a transfer learning approach.

---

## Dataset

The **CIFAR-10 dataset** contains **60,000 color images** of size **32×32 pixels** across **10 different classes**.

Classes included:

* Airplane
* Automobile
* Bird
* Cat
* Deer
* Dog
* Frog
* Horse
* Ship
* Truck

Dataset split:

* **50,000 images** for training
* **10,000 images** for testing

---

## Techniques Used

### 1. Data Preprocessing

* Normalization of pixel values (0–255 → 0–1)
* One-hot encoding of labels
* Train–validation split

### 2. Data Augmentation

To reduce overfitting, the following techniques were applied:

* Random horizontal flipping
* Random rotation
* Random zoom

### 3. Custom CNN Architecture

The custom CNN consists of:

* Convolutional layers
* MaxPooling layers
* Fully connected layers
* Softmax output layer for multiclass classification

### 4. Transfer Learning

A pretrained **MobileNetV2** model trained on ImageNet was used.
The convolutional base was frozen and additional dense layers were added for classification.

---

## Evaluation Metrics

Model performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

---

## Results

* **Custom CNN Accuracy:** ~61%
* **MobileNetV2 Transfer Learning Accuracy:** ~34%

The custom CNN performed better on the CIFAR-10 dataset due to the small image size (32×32), while MobileNetV2 is optimized for larger images.

---

## Tools and Libraries

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Project Structure

```
├── Assignment-2 Report.pdf
├── Assignment_2.ipynb
├── README.md
```

---

## Author

**Raj Tilak Singh**
MCA (AI & ML) – Semester 2
K.R. Mangalam University
Academic Session: 2025–2027
