# Fashion MNIST Image Classification using CNN

## Project Overview

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify Fashion MNIST images into 10 clothing categories.

## Dataset

- 70,000 Images
- 10 Categories
- Image Size: 28×28 pixels
- Grayscale Images

## pre-requisite Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- OpenCV

## CNN Architecture

Input Layer (28x28x1)

↓

Conv2D (32 Filters, ReLU)

↓

MaxPooling2D

↓

Flatten

↓

Dense (785 Units)

↓

Dense (10 Units, Softmax)

## Results

Model achieved an overall classification accuracy of **91.10%** on the Fashion MNIST test dataset. 

### Key Performance Metrics
* **Overall Accuracy:** 91.10%
* **Macro Average F1-Score:** 0.91
* **Weighted Average F1-Score:** 0.91

### Analysis & Observations
* **Strongest Performers:** The model excelled at identifying **Class 1** (98% F1-score), **Class 5** (98% F1-score), and **Class 8** (98% F1-score).
* **Weakest Performer:** **Class 6** showed the lowest performance with an F1-score of 77% and a recall of 79%, indicating the model frequently confuses 6s with other digits (likely 0s or 5s).
* **Target Areas for Improvement:** Future iterations will focus on spatial features to better differentiate between Class 6, Class 4 (83% recall), and Class 2 (85% recall).
