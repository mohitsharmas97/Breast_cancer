# Breast Cancer Classification using a Neural Network

This repository contains a deep learning model trained to classify breast cancer tumors as either malignant or benign based on diagnostic features. The model is built with Keras (TensorFlow) and provides a solid example of a binary classification task.

##  Project Overview

The goal of this project is to accurately predict breast cancer diagnosis from numerical data. It uses a trained Artificial Neural Network (ANN) that takes 10 specific features from a tumor analysis and outputs a probability indicating the likelihood of the tumor being malignant.

---

## Model Details

The model is a `Sequential` neural network with the following architecture:

* **Input Layer**: Expects a vector of 10 input features.
* **Hidden Layer 1**: A `Dense` layer with 116 neurons and a `ReLU` activation function.
* **Hidden Layer 2**: A `Dense` layer with 8 neurons and a `ReLU` activation function.
* **Output Layer**: A `Dense` layer with a single neuron and a `sigmoid` activation function, which outputs a probability between 0 and 1.

The model was compiled with:
* **Optimizer**: `adam`
* **Loss Function**: `binary_crossentropy`
* **Metrics**: `accuracy`

---

##  Dataset

The model was trained on the **Breast Cancer Wisconsin (Diagnostic) Data Set** from the UCI Machine Learning Repository, accessed via Kaggle.

From the original 30 features, this model uses the following 10 for prediction:
- `concave points_worst`
- `concave points_mean`
- `radius_worst`
- `perimeter_worst`
- `area_worst`
- `concavity_mean`
- `concavity_worst`
- `radius_mean`
- `perimeter_mean`
- `area_mean`

---
