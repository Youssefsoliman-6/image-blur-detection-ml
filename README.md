# Image Blur Detection Using Classical Machine Learning

## Overview
This project focuses on detecting and classifying image blur using classical image processing and machine learning techniques. Images are categorized into three classes: **sharp**, **defocus blur**, and **motion blur**.

Unlike deep learning approaches, this project relies on handcrafted features and traditional classifiers, making it computationally efficient and suitable for resource-constrained environments.

## Objectives
- Detect whether an image is sharp or blurred
- Distinguish between defocus blur and motion blur
- Apply classical machine learning instead of deep learning
- Evaluate and compare different classifiers

## Dataset
- Grayscale images resized to **256×256**
- Three classes:
  - Sharp
  - Defocus Blur
  - Motion Blur
- Dataset split:
  - 80% Training
  - 20% Testing (stratified)

## Feature Extraction
The following handcrafted features are extracted:
- **Variance of Laplacian** – measures image sharpness
- **Sobel Edge Strength** – captures edge intensity
- **FFT High-Frequency Energy** – detects motion blur
- **Image Entropy** – measures texture information

## Machine Learning Models
- **Support Vector Machine (SVM)** with RBF kernel (primary model)
- **Random Forest Classifier** (baseline comparison)

## Evaluation Metrics
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix

## Results
The SVM model achieved strong classification performance, especially in distinguishing sharp images from blurred ones. Most classification errors occurred between motion blur and defocus blur.

## Technologies Used
- Python
- OpenCV
- NumPy
- Scikit-learn
- Matplotlib

## Author
**Youssef Soliman**
