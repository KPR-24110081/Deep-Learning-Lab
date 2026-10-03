# Experiment 1: Single-Layer Perceptron for Binary Classification

This experiment focuses on implementing a single-layer perceptron from scratch for binary classification. The model is trained on the Banknote Authentication dataset and evaluated using standard classification metrics and visual diagnostics.

## Objective

- Implement a perceptron model without using high-level classification libraries.
- Train the model on a binary classification dataset.
- Analyze learning behavior through loss, weight updates, and decision boundaries.
- Compare the custom implementation with a scikit-learn perceptron baseline.

## Dataset

- Dataset: Banknote Authentication
- Source: UCI Machine Learning Repository
- Samples: 1,372
- Features: 4
- Classes: 2 (genuine vs forged banknotes)

## Workflow

- Dataset loading and exploration
- Exploratory data analysis
- Data preprocessing and normalization
- Perceptron implementation from scratch
- Training and evaluation
- Visualization of learning curves and decision boundary
- Comparison with scikit-learn perceptron

## Key concepts covered

- Linear decision boundaries
- Perceptron learning rule
- Weight and bias evolution over training epochs
- Feature normalization effects
- Binary classification metrics

## Evaluation metrics

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

## Files in this folder

- `Ex_1.ipynb` — main implementation and analysis notebook
- `Ex_1.pdf` — report/exported document
- `data_banknote_authentication.txt` — dataset file
- `plots/` — generated visualizations
- `README.md` — experiment documentation

## Generated visualizations

- Histogram
- Correlation heatmap
- Scatter plots
- Box plots
- Training error curve
- Weight evolution
- Bias evolution
- Learning rate analysis
- Decision boundary
- Step vs sigmoid comparison
- XOR visualization
- Normalization effect analysis

## Outcome

The perceptron was successfully trained and validated on a binary classification task, demonstrating the fundamental principles of perceptron learning and the role of feature scaling in model convergence.
