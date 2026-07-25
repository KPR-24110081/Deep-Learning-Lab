# Experiment 02 - Multi-Layer Perceptron for Fashion-MNIST Classification

## Objective

Implement a Multi-Layer Perceptron (MLP) using TensorFlow/Keras to classify images from the Fashion-MNIST dataset. The experiment also includes hyperparameter optimization using RandomizedSearchCV to improve the model's performance.

---

## Dataset

**Fashion-MNIST**

- 70,000 grayscale images
- 28 × 28 pixels
- 10 clothing categories
- 60,000 training images
- 10,000 testing images

Classes:

- T-shirt/Top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle Boot

---

## Tools & Technologies

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- SciKeras

---

## Model Architecture

```
Input Layer (784)

↓

Dense(128, ReLU)

↓

Dense(64, ReLU)

↓

Dense(10, Softmax)
```

---

## Hyperparameter Optimization

RandomizedSearchCV was used to optimize:

- Hidden Layer 1 Neurons
- Hidden Layer 2 Neurons
- Optimizer
- Batch Size
- Number of Epochs

---

## Performance Evaluation

The following evaluation metrics were computed:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

## Generated Visualizations

- Sample Images
- Class Distribution
- Training Accuracy vs Epoch
- Validation Accuracy vs Epoch
- Training Loss vs Epoch
- Validation Loss vs Epoch
- Confusion Matrix
- Hyperparameter Search Results
- Baseline vs Optimized Model Comparison

---

## Repository Contents

```
Experiment-02-MLP-FashionMNIST/

│── Ex_2.ipynb
│── Report.pdf
│── README.md
│── hyperparameter_results.csv
│── plots/
```

---

## Learning Outcomes

- Implemented an MLP using TensorFlow/Keras.
- Applied image preprocessing techniques.
- Trained and evaluated a neural network for image classification.
- Performed hyperparameter optimization using RandomizedSearchCV.
- Analyzed model performance through multiple evaluation metrics and visualizations.
