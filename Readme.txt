# Cooked vs Uncooked Chicken Image Classification

This repository contains a deep learning project aimed at classifying images of chicken as either **cooked** or **uncooked**. The classification model uses **TensorFlow** and **Keras** with **MobileNetV2** as a base for transfer learning. The dataset is publicly available and is organized into training, validation, and test sets.

## Dataset Overview
The dataset contains images of chicken in two categories:
- **Cooked Chicken**
- **Uncooked Chicken**

- **Total Images**: 362
  - **Training Set**: 212 images of cooked chicken, 153 images of uncooked chicken
  - **Validation Set**: 5 images of cooked chicken, 10 images of uncooked chicken
  - **Test Set**: 31 images (mixed cooked and uncooked chicken)
- **File Formats**: `.jpg`, `.jpeg`, `.png`
- **Image Size**: Resized to 224x224 pixels for model compatibility.
- **Image Augmentation**: Includes rotation, zoom, width/height shift, shear, and horizontal flip.

## Model Overview
The model is based on the **MobileNetV2** architecture, which is pre-trained on ImageNet. The model is fine-tuned for binary classification (cooked vs uncooked) by adding custom layers for classification.

### Model Features:
- **Transfer Learning**: Using MobileNetV2 for feature extraction.
- **Custom Layers**: Global average pooling, dense layers, and a dropout layer for better performance.
- **Callbacks**: Early stopping and learning rate reduction on plateau to improve model convergence.

## Intended Use
This repository can be used for:
- **Image Classification**: Train and evaluate models to classify chicken images as cooked or uncooked.
- **Benchmarking**: Test various deep learning models and compare performance.
- **Educational Use**: Learn how to work with image datasets, deep learning models, and TensorFlow.
