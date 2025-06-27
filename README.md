# FII-NX1Intl-Jana-Mohamed
# CleanWaterAI — Water Potability Classifier 💧

## Overview

This project builds a simple neural network model to classify water samples as **Potable** (safe to drink) or **Not Potable** based on various water quality features.

The goal is to support **SDG 6: Clean Water and Sanitation** by helping identify safe drinking water quickly.

---

## Dataset

- The model uses the [Water Potability dataset](https://www.kaggle.com/datasets/adityakadiwal/water-potability) from Kaggle.
- Dataset contains 9 features like pH, hardness, solids, chloramines, etc.
- Target label: `Potability` (1 = Potable, 0 = Not Potable)
- Missing values are filled with feature means during preprocessing.

---

## Model

- Simple Multi-Layer Perceptron (MLP) built with PyTorch.
- Architecture: Input layer → 2 hidden layers → output layer with sigmoid activation.
- Binary classification trained with binary cross-entropy loss.
- Training done for 20 epochs with Adam optimizer.

---

## Usage

1. Load the dataset (`water_potability.csv`).
2. Preprocess data (fill missing, scale features).
3. Train the model (`CleanWaterAI_pt1.ipynb`).
4. Save the trained model weights (`water_model.pt`).
5. Load the model for predictions (`CleanWaterAI_pt2.ipynb`).
6. Use the function `predict_potability()` to predict on new samples.

---

## Requirements

- Python 3.x
- PyTorch
- pandas
- scikit-learn

Install dependencies via:
```bash
pip install torch pandas scikit-learn
