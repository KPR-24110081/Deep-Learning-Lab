# Experiment 2: Multi-Layer Perceptron for Fashion-MNIST Classification

This experiment implements a Multi-Layer Perceptron (MLP) to classify clothing images from the Fashion-MNIST dataset. The workflow includes data preparation, model training, hyperparameter tuning, and evaluation using multiple performance metrics.

## Objective

- Build an MLP in TensorFlow/Keras for image classification.
- Train and evaluate the model on Fashion-MNIST.
- Perform hyperparameter optimization using randomized search.
- Compare baseline and optimized model performance.

## Dataset

- Dataset: Fashion-MNIST
- Classes: 10 clothing categories
- Training samples: 60,000
- Test samples: 10,000
- Image size: 28 × 28 grayscale

Classes include:

- T-shirt/top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle boot

## Model architecture

The model uses a shallow neural network with dense layers:

```text
Input (784) -> Dense(128, ReLU) -> Dense(64, ReLU) -> Dense(10, Softmax)
```

## Hyperparameter tuning

The experiment explores tuning across several values, including:

- Number of neurons in hidden layers
- Optimizer choice
- Batch size
- Number of epochs

## Evaluation metrics

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Classification report

## Files in this folder

- `Ex_2.ipynb` — notebook with implementation and analysis
- `Ex_2.pdf` — report
- `hyperparameter_results.csv` — optimization results
- `plots/` — performance and diagnostic plots
- `README.md` — documentation

## Visualizations included

- Sample images
- Class distribution
- Training and validation accuracy
- Training and validation loss
- Confusion matrix
- Hyperparameter search summary
- Baseline vs optimized model comparison

## Outcome

The MLP achieved strong classification performance on Fashion-MNIST, and hyperparameter optimization helped improve the model’s ability to generalize effectively to unseen data.
