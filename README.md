# Waste Classification Using CNN

This project aims to classify waste images into **Organic** or **Recyclable** categories using a Convolutional Neural Network (CNN). The model is trained on the [TechSash Waste Classification Dataset](https://www.kaggle.com/techsash/waste-classification-data) from Kaggle.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Model Architecture](#model-architecture)
4. [Training](#training)
5. [Results](#results)
6. [Deployment](#deployment)
7. [How to Run](#how-to-run)

## Project Overview
- **Objective**: Automate waste classification using deep learning.
- **Tools Used**: TensorFlow/Keras, OpenCV, Pandas, NumPy, Matplotlib.

## Dataset
- Source: [TechSash Waste Classification Dataset](https://www.kaggle.com/techsash/waste-classification-data).
- Contains 22,500 images split into TRAIN and TEST sets.
- Balanced dataset with 55.69% Organic and 44.31% Recyclable images.

## Model Architecture
- **CNN Layers**: 3 Convolutional Layers (32, 64, 128 filters) + MaxPooling.
- **Fully Connected Layers**: 256 and 64 neurons with Dropout.
- **Output Layer**: Sigmoid activation for binary classification.

## Training
- **Optimizer**: Adam.
- **Loss Function**: Binary Cross-Entropy.
- **Early Stopping**: Patience=20 to prevent overfitting.
- Achieved ~90% validation accuracy.

## Results
- Training and validation curves show minimal overfitting.
- Model successfully classifies waste images into Organic or Recyclable categories.

## Deployment
The model can be deployed using Streamlit for real-time waste classification. Use the following code to run the Streamlit app:

```bash
streamlit run app.py



How to Run

    Clone the repository:
    bash

    git clone [https://github.com/Aryan-Katiyar-15/Waste_Classification.git]

    Install dependencies:
    bash

    pip install -r requirements.txt

    Run the Streamlit app:
    bash

    streamlit run app.py