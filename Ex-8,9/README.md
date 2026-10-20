# Experiment 8 & 9: Attention Mechanisms in ResNet50

This experiment investigates the effect of different attention mechanisms and their insertion positions in an ImageNet-pretrained ResNet50 model. The focus is on improving image classification, comparing model performance, analyzing attention maps, and understanding the computational cost of different attention architectures.

## Objective

- Understand how attention mechanisms enhance feature representations in convolutional neural networks.
- Compare channel attention, spatial attention, channel–spatial attention, and self-attention.
- Study the effect of inserting attention at different ResNet50 stages.
- Analyze multi-position attention, attention ordering, and spatial-attention kernel sizes.
- Compare classification performance, model complexity, and inference time.
- Visualize attention responses and interpret model predictions using Grad-CAM.

## Dataset

The experiment uses the TensorFlow Flowers dataset, which contains 3,670 images belonging to five classes: daisy, dandelion, roses, sunflowers, and tulips.

The images are resized to 224 × 224 × 3 and processed using the preprocessing function for ImageNet-pretrained ResNet50. The dataset is divided into training, validation, and testing subsets using a 70:15:15 split.

## Model types explored

- Baseline ResNet50
- Channel Attention
- Spatial Attention
- Channel–Spatial Attention
- Self-Attention
- Squeeze-and-Excitation (SE)
- Efficient Channel Attention (ECA)
- Convolutional Block Attention Module (CBAM)

## Core concepts covered

- Transfer learning with pretrained ResNet50
- Channel-wise feature recalibration
- Spatial attention maps
- Scaled dot-product self-attention
- Attention insertion positions (P1, P2, P3, and P4)
- Multi-position attention
- Channel–spatial attention ordering
- Spatial-attention kernel-size comparison
- Feature-map analysis
- Grad-CAM visualization
- Model complexity and inference efficiency

## Evaluation metrics

- Classification accuracy
- Macro precision
- Macro recall
- Macro F1-score
- Total and trainable parameters
- Average inference time per image
- Confusion matrices
- Qualitative attention-map analysis

## Files in this folder

- `DL_Lab_8_9.ipynb.zip` — compressed notebook containing the attention experiments
- `Ex_8_9.pdf` — experiment report
- `figures/` — generated plots and visualizations
- `README.md` — experiment summary

## Visualizations included

- Sample flower images
- Class distribution
- Training and validation accuracy
- Training and validation loss
- Model accuracy comparison
- Macro F1-score comparison
- Attention-position comparison
- Attention-order comparison
- Spatial kernel-size comparison
- Confusion matrices
- Feature maps before and after attention
- Channel-attention weights
- Spatial-attention maps and overlays
- Self-attention response
- Grad-CAM visualizations
- Qualitative model comparisons
- Additional attention-mechanism comparisons

## Outcome

The experiment demonstrates how attention mechanisms influence image classification performance and feature representations in ResNet50. In the recorded attention-type comparison, channel attention achieved the highest test accuracy among the evaluated configurations. The position study showed that the effect of attention depends on where it is inserted in the network. The visualizations provide additional insight into model responses, while parameter counts and inference times help assess the trade-off between classification performance and computational cost.
