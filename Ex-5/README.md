# Experiment 5 — Comprehensive CNN Study

This experiment presents a comprehensive study of **Convolutional Neural Network (CNN) training, regularization, optimization, hyperparameter tuning, transfer learning, fine-tuning, and cross-validation** using **MobileNetV2** on the **Oxford-IIIT Pet Dataset**.

The experiment was completed as part of the **Deep Learning Laboratory** for the B.Tech Artificial Intelligence & Data Science curriculum at **Shiv Nadar University Chennai**.

---

## Objective

The objectives of this experiment are to:

- Study the effect of different weight initialization techniques.
- Analyze overfitting and the effect of regularization.
- Investigate the impact of Batch Normalization.
- Compare different optimization algorithms.
- Perform systematic CNN hyperparameter tuning.
- Study transfer learning using a pretrained MobileNetV2 model.
- Compare feature extraction and fine-tuning.
- Perform 5-fold cross-validation for model selection.
- Evaluate the final selected model on an independent test set.

---

## Dataset

### Oxford-IIIT Pet Dataset

The experiment uses the **Oxford-IIIT Pet Dataset**, containing images from **37 different cat and dog breeds**.

| Property | Value |
|---|---|
| Dataset | Oxford-IIIT Pet |
| Number of Classes | 37 |
| Image Type | RGB |
| Input Size | `224 × 224 × 3` |
| Task | Multi-class Image Classification |

The dataset is divided into training, validation, and test sets. The independent test set is kept separate during model selection and is used only for the final evaluation.

---

## Model Architecture

The experiment uses **MobileNetV2 pretrained on ImageNet**.

MobileNetV2 is a lightweight CNN architecture based on:

- Inverted residual blocks
- Depthwise separable convolutions
- Pointwise `1 × 1` convolutions
- Linear bottlenecks
- Batch Normalization
- ReLU6 activation

The pretrained network is adapted to the 37-class pet classification task by replacing the original classification head.

---

## Experiments

### 1. Weight Initialization

Four initialization strategies were compared:

- Zero Initialization
- Random Initialization
- Xavier/Glorot Initialization
- He Initialization

#### Results

| Initialization | Final Validation Accuracy | Best Validation Accuracy | Training Time |
|---|---:|---:|---:|
| Zero | 91.30% | 91.30% | 41.96 s |
| Random | 90.35% | 90.35% | 41.71 s |
| Xavier/Glorot | 91.17% | 91.17% | 41.40 s |
| He | 91.17% | **91.58%** | 41.91 s |

He initialization achieved the highest peak validation accuracy, while Zero initialization achieved the highest final validation accuracy.

---

### 2. Regularization and Overfitting

Different regularization strategies were investigated to study their effect on overfitting and generalization.

The experiments included:

- No Regularization
- L2 Regularization
- Dropout
- Batch Normalization

Training and validation accuracy/loss curves were used to analyze the generalization gap.

---

### 3. Batch Normalization

Batch Normalization was investigated to study its effect on:

- Training stability
- Convergence
- Validation performance
- Sensitivity to initialization

---

### 4. Optimization Algorithms

The following optimizers were compared:

- SGD
- Momentum
- RMSProp
- Adam

#### Results

| Optimizer | Final Loss | Best Validation Accuracy | Epoch to Converge | Training Time |
|---|---:|---:|---:|---:|
| SGD | 3.079395 | 23.37% | 5 | 42.872 s |
| Momentum | 0.470831 | 89.13% | 5 | 42.320 s |
| RMSProp | 0.046401 | 89.81% | 5 | 42.350 s |
| Adam | **0.043456** | **90.49%** | 5 | 42.808 s |

Adam achieved the highest validation accuracy and the lowest final loss among the tested optimizers.

---

### 5. CNN Hyperparameter Tuning

The following hyperparameters were investigated:

- Learning Rate
- Batch Size
- Dropout Rate
- Optimizer
- Fine-Tuning Learning Rate
- Frozen / Partially Unfrozen Layers

The experiments were performed by changing one hyperparameter at a time while keeping the remaining settings fixed.

---

### 6. Transfer Learning

Two transfer-learning strategies were compared.

#### Feature Extraction

The pretrained MobileNetV2 base is frozen and used as a fixed feature extractor.

```text
Pretrained MobileNetV2
          ↓
      Freeze Base
          ↓
    New Classifier
