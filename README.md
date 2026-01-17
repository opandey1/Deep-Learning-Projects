# CIFAR-10 & CIFAR-100 CNN Optimization

## 📌 Project Overview
This project explores the architectural optimization of Convolutional Neural Networks (CNNs) for image classification. Starting from a simple baseline, I iteratively improved the model architecture and training pipeline to achieve high performance on **CIFAR-10 (>90%)** and a strong baseline on **CIFAR-100 (~73%)**.

## 🚀 Key Improvements
* **Architecture:** Evolved from a shallow 3-layer CNN to a Deep VGG-Style network with **Global Average Pooling**.
* **Optimization:** Switched from Adam to **SGD with Nesterov Momentum** and implemented **Cosine Annealing Learning Rate**.
* **Regularization:** Utilized Weight Decay, Label Smoothing, and Data Augmentation to prevent overfitting.

## 📊 Results Summary

| Dataset | Accuracy | Key Technique |
| :--- | :--- | :--- |
| **CIFAR-10** | **~78.5%** (Baseline) | Adam Optimizer |
| **CIFAR-10** | **>90.0%** (Final) | Deep CNN + SGD + Cosine Scheduler |
| **CIFAR-100** | **72.8%** | Label Smoothing + Extended Training |

## 📂 Repository Structure
* `notebooks/`: Contains the Jupyter Notebooks for training and evaluation.
* `reports/`: Detailed PDF reports analyzing the loss curves, confusion matrices, and hyperparameter choices.

## 🛠️ Requirements
* Python 3.x
* PyTorch & Torchvision
* Matplotlib