# Experiment 3 — Convolutional Neural Network

## Objective

To understand the working principle of Convolutional Neural Networks (CNNs) by implementing convolution, stride, padding, pooling, feature-map visualization, and image classification using the CIFAR-10 dataset.

## Dataset

The CIFAR-10 dataset was used for this experiment.

- Number of classes: 10
- Training images: 50,000
- Image dimensions: 32 × 32 × 3
- Image type: RGB
- Classes:
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

The dataset files are not included in this repository because of their large size.

## Tasks Performed

### Task 1 — Dataset Exploration

- Loaded the CIFAR-10 dataset.
- Displayed sample images.
- Verified dataset dimensions.
- Plotted the class distribution.

### Task 2 — Convolution

Convolution was implemented and compared using:

- 3 × 3 kernel
- 5 × 5 kernel
- 7 × 7 kernel

The resulting feature-map dimensions were analyzed.

### Task 3 — Stride and Padding

The effects of the following configurations were studied:

- Stride = 1
- Stride = 2
- Same Padding
- Valid Padding

### Task 4 — Feature Map Visualization

A convolution layer with multiple filters was used to generate and visualize feature maps. Eight feature maps were displayed.

### Task 5 — Pooling

The following pooling methods were compared:

- Max Pooling
- Average Pooling

Their output dimensions and classification performance were analyzed.

### Task 6 — CNN Construction and Training

The CNN architecture used was:

```text
Input
  ↓
Conv2D
  ↓
ReLU
  ↓
MaxPooling
  ↓
Conv2D
  ↓
ReLU
  ↓
MaxPooling
  ↓
Flatten
  ↓
Dense
  ↓
Softmax
