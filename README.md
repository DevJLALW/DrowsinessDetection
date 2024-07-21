# DrowsinessDetection - WIP
This project aims to detect drowsiness by analyzing eye states (open or closed) using a deep learning model. The model is trained on grayscale eye images using transfer learning with MobileNetV2.

## Datasets
1. MRL Eye Dataset
Description: Contains images of eyes in grayscale.
Purpose: Used for training and validating the drowsiness detection model.

## Model Architecture
Base Model: MobileNetV2 (pretrained on ImageNet)
Input Size: 224x224 RGB images
Output: Binary classification (Open/Closed eyes)
Training Epochs: 20 epochs with callbacks for checkpoint saving and learning rate adjustment.

## Downloading Datasets
MRL Eye Dataset: Download from Kaggle and unzip it.

## Model Training
Data Preparation: The dataset is processed and augmented using a custom data generator that converts grayscale images to RGB.
Model Definition: MobileNetV2 is used with additional dense layers for binary classification.

## Training: 
The model is trained with early stopping and learning rate reduction strategies.

## Testing the Model
Preprocessing: The eye images are resized and normalized.
Prediction: The trained model predicts the eye state (Open/Closed) and annotates the results.
Visualization: The results are saved and displayed.
