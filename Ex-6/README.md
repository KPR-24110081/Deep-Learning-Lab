# Experiment 6: Recurrent Neural Networks for Sequential Data

This experiment studies sequence modeling using recurrent architectures, including RNN, LSTM, and GRU models. The work focuses on temporal pattern recognition using sequential activity data and compares model performance across architectures and sequence lengths.

## Objective

- Understand how recurrent neural networks handle sequential data.
- Compare simple RNN, LSTM, and GRU models for temporal classification.
- Evaluate the effect of sequence length on model performance.
- Explore seq2seq-style sequence modeling as an extension.

## Dataset

The experiment is based on a human activity / time-series dataset that captures sequential motion patterns over time. The data is treated as temporal sequences for classification of activities such as sitting, walking, and laying.

## Model types explored

- Recurrent Neural Network (RNN)
- Long Short-Term Memory (LSTM)
- Gated Recurrent Unit (GRU)
- Seq2Seq-based sequence modeling

## Core topics covered

- Temporal sequence processing
- Hidden state propagation
- Long-term dependency learning
- Sequence-to-sequence learning concepts
- Model comparison by accuracy and F1-score
- Sequence length sensitivity analysis

## Evaluation metrics

- Training loss
- Validation loss
- Training accuracy
- Validation accuracy
- Confusion matrix
- Accuracy comparison
- F1-score comparison
- Model parameter and runtime comparison

## Files in this folder

- `Ex_6.ipynb` — main experiment and model analysis
- `Ex_6.pdf` — report/exported writeup
- `figures/` — all generated plots and comparison charts
- `README.md` — experiment documentation

## Generated visualizations

- Temporal activity plots
- RNN training/validation loss
- RNN training/validation accuracy
- RNN confusion matrix
- LSTM training/validation loss and accuracy
- LSTM confusion matrix
- GRU training/validation loss and accuracy
- GRU confusion matrix
- Model accuracy/F1 comparison
- Parameter comparison
- Training-time comparison
- Sequence length vs test F1-score
- Seq2Seq training/validation loss

## Outcome

The results show that LSTM and GRU models significantly outperform a plain RNN on sequential patterns, with GRU often offering a favorable balance between performance and computational cost. Sequence length analysis emphasizes the importance of temporal context in recurrent modeling.
