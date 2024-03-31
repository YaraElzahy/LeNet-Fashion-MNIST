# Fashion MNIST - Transfer Learning

## Overview

Fashion MNIST, led by Yara Elzahy, focuses on classifying clothing items from Zalando's dataset. With 60,000 grayscale images of 10 clothing types, the project aims to predict item types, addressing challenges in image processing, architecture adjustment, and hyperparameter optimization.

## Project Details

- **Author:** Yara Elzahy
- **ID:** 20398570

### Problem Statement

Fashion MNIST tackles classifying clothing items, mapping 0-9 integers to specific labels. With images resized to 28x28 pixels, each pixel ranges from 0 to 255, representing darkness. The objective is to predict clothing types, overcoming challenges in image handling, model architecture, and parameter optimization.

### Data Description

The dataset comprises 60,000 images of clothing items, with each image containing 784 pixel values and a corresponding class label. Each pixel represents darkness, and labels range from T-shirt/top (0) to Ankle boot (9).

## Project Pipeline

The project pipeline includes:

1. **Data Preparation:** Reading, exploring, visualizing, and preprocessing the data.
2. **Training a CNN Neural Network:** Adjusting data shapes, building LeNet-5 model, and hyperparameter tuning.
3. **Transfer Learning:** Utilizing pre-trained models (ResNet152V2, EfficientNetB1, VGG16) and evaluating performance.

## Results

- **LeNet-5 Model:**
  - Validation Accuracy: 89.82%
  - Hyperparameter Tuning: Validation Accuracy dropped to 89.40%.

- **10-Fold Cross Validation:**
  - Consistent accuracy across folds suggests low variance, indicating the model avoids overfitting.

- **Transfer Learning:**
  - ResNet152V2: Validation Accuracy: 72.31%
  - EfficientNetB1: Validation Accuracy: 10.01%
  - VGG16: Validation Accuracy: 10.00%

## Conclusion

- Transfer learning led to decreased accuracy, suggesting a domain mismatch.
- Pre-trained models may converge but remain stuck at local minima, hindering performance improvement compared to training from scratch.
