# Experiment 4: Transfer Learning using MobileNetV2

## Objective

To implement transfer learning using a pretrained MobileNetV2 model on the CIFAR-10 dataset and evaluate its performance before and after fine-tuning.

---

## Dataset

* **Dataset:** CIFAR-10
* **Training Samples:** 50,000
* **Testing Samples:** 10,000
* **Image Size:** 32 × 32 × 3
* **Classes:** 10

---

## Tasks Performed

* CIFAR-10 Dataset Preparation
* Dataset Normalization
* Sample Image Visualization
* Transfer Learning using MobileNetV2
* ImageNet Pretrained Model Loading
* Convolutional Base Freezing
* Classification Head Construction
* Model Training
* Fine-Tuning
* Model Evaluation
* Accuracy, Precision, Recall and F1-score Calculation
* Confusion Matrix Visualization
* Misclassified Image Analysis
* Training and Validation Accuracy Visualization
* Training and Validation Loss Visualization

---

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Results

The MobileNetV2 transfer learning model achieved an accuracy of **85.78%** before fine-tuning.

After fine-tuning the final portion of the pretrained network, the model achieved an accuracy of **87.99%**, resulting in an improvement of **2.21 percentage points**.

| Metric                      |                 Result |
| --------------------------- | ---------------------: |
| Before Fine-Tuning Accuracy |                 85.78% |
| After Fine-Tuning Accuracy  |                 87.99% |
| Improvement                 | 2.21 percentage points |
| Precision                   |                 87.99% |
| Recall                      |                 87.99% |
| F1-score                    |                 87.94% |
| Total Parameters            |              2,423,242 |
| Initial Training Time       |         243.89 seconds |
| Fine-Tuning Time            |         186.98 seconds |
| Total Training Time         |         430.87 seconds |

---

## Repository Structure

```text
Ex-4/
│   ├── Ex_4.ipynb
│   ├── Report.pdf
│   ├── README.md
│   └── plots/
│       ├── sample_images.png
│       ├── training_validation_accuracy.png
│       ├── training_validation_loss.png
│       ├── fine_tuning_accuracy.png
│       ├── fine_tuning_loss.png
│       ├── confusion_matrix.png
│       └── misclassified_images.png
```

---

## Author

K. Prithvi<br>
24011101047<br>
B.Tech AI & DS - A<br>
Shiv Nadar University Chennai

