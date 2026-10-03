# Experiment 4: Transfer Learning with MobileNetV2

This experiment explores transfer learning using a pretrained MobileNetV2 model for CIFAR-10 image classification. The workflow includes feature extraction, fine-tuning, and evaluation of training performance before and after optimization.

## Objective

- Use a pretrained ImageNet model as a feature extractor.
- Adapt MobileNetV2 to CIFAR-10 classification.
- Compare performance before and after fine-tuning.
- Evaluate improvements in accuracy and generalization.

## Dataset

- Dataset: CIFAR-10
- Training samples: 50,000
- Testing samples: 10,000
- Image size: 32 × 32 × 3
- Classes: 10

## Workflow

- Load CIFAR-10 data
- Normalize and preprocess images
- Load pretrained MobileNetV2 model
- Freeze base layers for initial training
- Add and train a classification head
- Unfreeze later layers for fine-tuning
- Measure performance improvements
- Analyze misclassified examples and training curves

## Key results

| Metric | Result |
| --- | ---: |
| Accuracy before fine-tuning | 85.78% |
| Accuracy after fine-tuning | 87.99% |
| Improvement | +2.21 percentage points |
| Precision | 87.99% |
| Recall | 87.99% |
| F1-score | 87.94% |

## Files in this folder

- `Ex_4.ipynb` — main implementation notebook
- `Ex-4.pdf` — report
- `plots/` — generated graphs and visual diagnostics
- `README.md` — experiment summary

## Generated analysis

- Sample image visualization
- Training vs validation accuracy
- Training vs validation loss
- Fine-tuning accuracy comparison
- Confusion matrix
- Misclassified image review

## Outcome

Transfer learning with MobileNetV2 proved effective for CIFAR-10, and fine-tuning the deeper layers led to measurable gains in classification accuracy and convergence quality.
