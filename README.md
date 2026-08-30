# Deep Learning Laboratory

This repository contains the implementation of Deep Learning Laboratory experiments completed as part of the **B.Tech Artificial Intelligence & Data Science** curriculum at **Shiv Nadar University Chennai**.

## Experiments

| Experiment | Topic |
| ---------- | ----- |
| Experiment 1 | Single Layer Perceptron for Binary Classification |
| Experiment 2 | Multi-Layer Perceptron using TensorFlow |
| Experiment 3 | Convolutional Neural Network using CIFAR-10 |
| Experiment 4 | Transfer Learning and Fine-Tuning using MobileNetV2 |
| Experiment 5 | Comprehensive Study of CNN Training, Regularization, Optimization, Hyperparameter Tuning, Transfer Learning and Cross-Validation |

## Repository Structure

```text
Deep-Learning-Lab/
│
├── README.md
├── LICENSE
│
├── Ex-1/
│   ├── Ex_1.ipynb
│   ├── data_banknote_authentication.txt
│   ├── Ex-1.pdf
│   ├── README.md
│   └── plots/
│       ├── histogram.eps
│       ├── heatmap.eps
│       ├── scatter.eps
│       ├── boxplot.eps
│       ├── training_error.eps
│       ├── weight_evolution.eps
│       ├── bias_evolution.eps
│       ├── learning_rate.eps
│       ├── confusion_matrix.eps
│       ├── decision_boundary.eps
│       ├── normalization.eps
│       ├── step_vs_sigmoid.eps
│       └── xor.eps
│
├── Experiment-02-MLP-FashionMNIST/
│   ├── Ex_2.ipynb
│   ├── Ex_2.pdf
│   ├── README.md
│   ├── hyperparameter_results.csv
│   └── plots/
│       ├── class_distribution.png
│       ├── confusion_matrix.png
│       ├── hyperparameter_search_results.png
│       ├── Model_Accuracy_Comparison.png
│       ├── sample_images.png
│       ├── Training_and_Validation_Accuracy.png
│       └── Training_and_Validation_Loss.png
│
├── Experiment-03-CNN-CIFAR10/
│   ├── Ex_3.ipynb
│   ├── README.md
│   └── figures/
│       ├── class_distribution.png
│       ├── confusion_matrix.png
│       ├── convolution_comparison.png
│       ├── feature_maps.png
│       ├── pooling_comparison.png
│       ├── sample_images.png
│       ├── stride_padding.png
│       ├── training_validation_accuracy.png
│       └── training_validation_loss.png
│
├── Ex-4/
│   ├── Ex_4.ipynb
│   ├── Ex_4.tex
│   ├── Report.pdf
│   ├── README.md
│   └── plots/
│       ├── sample_images.png
│       ├── training_validation_accuracy.png
│       ├── training_validation_loss.png
│       ├── fine_tuning_accuracy.png
│       ├── confusion_matrix.png
│       └── misclassified_images.png
│
└── Ex-5/
    ├── Ex_5.ipynb
    ├── Ex_5.tex
    ├── Report.pdf
    ├── README.md
    └── plots/
        ├── plot1_initialization_training_loss.png
        ├── plot2_initialization_validation_accuracy.png
        ├── plot3_regularization_accuracy.png
        ├── plot4_regularization_loss.png
        ├── plot5_batch_normalization.png
        ├── plot6_optimizer_training_loss.png
        ├── plot7_optimizer_validation_accuracy.png
        ├── plot8_learning_rate.png
        ├── plot9_batch_size.png
        ├── plot10_dropout_rate.png
        ├── plot11_feature_extraction_vs_finetuning.png
        ├── plot12_finetuning_loss.png
        ├── plot13_5fold_cross_validation.png
        ├── plot14_confusion_matrix.png
        └── plot15_misclassified_images.png
