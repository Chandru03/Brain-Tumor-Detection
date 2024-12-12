# Brain Tumor Detection using ResNet-50

This project aims to detect brain tumors from MRI images using a Convolutional Neural Network (CNN) based on the ResNet-50 architecture. The model classifies images into four categories: glioma, meningioma, no tumor, and pituitary.

## Model Performance Summary

- **Training Accuracy:** 99.39%
- **Validation Accuracy:** 87.82%
- **Test Accuracy:** 91.99%
- **Test Loss:** 0.28

## Model Details

- **Architecture:** ResNet-50 v1.5
- **Pre-trained on:** ImageNet
- **Input Image Size:** 224x224 pixels
- **Normalized Pixel Values:** [0, 1]

## Callbacks Used

- **ModelCheckpoint:** Save the best model based on validation loss
- **EarlyStopping:** Stop training if validation loss doesn't improve for 10 epochs

## Training Process

- **Epochs:** Stopped at 20 epochs due to early stopping
- **Batch Size:** 16
- **Optimizer:** Adam with learning rate 0.001
- **Loss Function:** Sparse Categorical Crossentropy

## Getting Started

### Prerequisites

- Python 3.x
- TensorFlow
- NumPy
- OpenCV
- Matplotlib
- Kaggle API (for dataset)
