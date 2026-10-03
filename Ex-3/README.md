# Experiment 3: Convolutional Neural Network for CIFAR-10 Classification

This experiment introduces the fundamentals of Convolutional Neural Networks (CNNs), including convolution, stride, padding, pooling, and feature map extraction. The model is trained on the CIFAR-10 dataset for image classification.

## Objective

- Understand the role of convolutional filters in feature extraction.
- Study the effect of stride and padding on output dimensions.
- Compare max pooling and average pooling.
- Train a CNN for CIFAR-10 classification.
- Interpret feature maps and classification outcomes.

## Dataset

- Dataset: CIFAR-10
- Classes: 10
- Training images: 50,000
- Test images: 10,000
- Image size: 32 × 32 × 3

Classes include:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

## Core concepts covered

- Convolution operation
- Kernel size comparison
- Stride and padding variations
- Feature map generation
- Pooling and dimensionality reduction
- CNN training and validation

## Model architecture

```text
Input
  ↓
Conv2D + ReLU
  ↓
MaxPooling
  ↓
Conv2D + ReLU
  ↓
MaxPooling
  ↓
Flatten
  ↓
Dense
  ↓
Softmax
```

## Evaluation metrics

- Accuracy
- Loss curves
- Confusion matrix
- Class distribution analysis

## Files in this folder

- `Ex_3.ipynb` — notebook implementing the experiments
- `Ex_3 .pdf` — project report
- `plots/` — figure outputs and visual analyses
- `README.md` — experiment documentation

## Generated visualizations

- Class distribution
- Sample images
- Convolution comparison plots
- Feature maps
- Pooling comparison
- Stride and padding diagrams
- Training and validation loss curves
- Training and validation accuracy curves
- Confusion matrix

## Outcome

The experiment successfully demonstrated how CNNs learn spatial hierarchies and how different architectural components influence the representational power and performance of the classifier.
