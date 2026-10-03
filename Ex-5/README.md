# Experiment 5: Comprehensive CNN Study

This experiment covers a broad set of CNN-related topics, including initialization strategies, regularization, normalization, optimizer comparison, transfer learning, fine-tuning, and cross-validation. It provides a structured investigation into how architecture and training choices affect deep model performance.

## Objective

- Study the effect of different weight initialization methods.
- Analyze overfitting using regularization techniques.
- Compare optimization algorithms.
- Evaluate batch normalization and dropout effects.
- Explore transfer learning and fine-tuning with MobileNetV2.
- Validate final model performance using cross-validation and a held-out test set.

## Dataset

- Dataset: Oxford-IIIT Pet Dataset
- Number of classes: 37
- Image type: RGB
- Input size: 224 × 224 × 3
- Task: Multi-class image classification

## Experiments included

### 1. Weight initialization
- Zero initialization
- Random initialization
- Xavier/Glorot initialization
- He initialization

### 2. Regularization and overfitting
- No regularization
- L2 regularization
- Dropout
- Batch normalization

### 3. Optimizer comparison
- SGD
- Momentum
- RMSProp
- Adam

### 4. Transfer learning and fine-tuning
- Feature extraction with a pretrained MobileNetV2 base
- Partial unfreezing and fine-tuning

### 5. Cross-validation
- 5-fold validation for model selection

## Files in this folder

- `DL_Lab_5_Part_1.ipynb` — first set of experiments and analysis
- `DL_Lab_5_Part_2.ipynb` — second part including transfer learning and validation
- `Ex_5 .pdf` — report document
- `plots/` — figures from the experiments
- `README.md` — documentation

## Key findings

- He initialization provided good convergence behavior.
- Regularization and normalization helped control overfitting and improved training stability.
- Adam consistently achieved strong validation performance compared with other optimizers.
- Transfer learning significantly improved performance on the pet classification task.
- Cross-validation supported robust model selection and helped reduce variance.

## Generated plots

- Initialization training loss
- Validation accuracy plots
- Regularization accuracy and loss curves
- Batch normalization comparison
- Optimizer performance plots
- Learning rate and batch size sensitivity
- Dropout comparison
- Transfer learning vs fine-tuning comparison
- 5-fold validation summary
- Confusion matrix

## Outcome

The experiment demonstrates that careful training design, regularization, and transfer learning are essential for building robust CNNs in real-world image classification settings.
