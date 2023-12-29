# Resume Classifier 

## Overview
This project implements a resume classifier using only the visual characteristics of an image. The model is trained to accurately classify whether a given image is a resume or not without utilizing OCR or any textual features.

## Contents

- [Dataset](#dataset)
- [Data Augmentation and Preprocessing](#data-augmentation-and-preprocessing)
- [Model Selection](#model-selection)
- [Model Training](#model-training)
- [Testing and Evaluation](#testing-and-evaluation)
- [Results](#results)


## Dataset

The dataset consists of resume and non-resume images in JPG and PNG formats. Images are organized into two folders: `resume` and `non_resume`.

## Data Augmentation and Preprocessing

Data augmentation techniques are applied to enhance model robustness. The `ImageDataGenerator` is used for real-time data augmentation during training. Preprocessing steps include resizing and normalization.

## Model Selection

The MobileNetV2 architecture is chosen as the backbone for the model. It offers a balance between efficiency and accuracy. The model includes a GlobalAveragePooling2D layer and two Dense layers for binary classification.

## Model Training

The model is trained on the augmented training and validation dataset. Hyperparameters such as batch size, epochs, and augmentation factor are experimented with to optimize performance. Training progress is monitored using callbacks.

## Testing and Evaluation

The trained model is evaluated on a separate test set. Evaluation metrics, including accuracy, precision, recall, and F1-score, are calculated. A confusion matrix visually represents the model's performance on the test set.

## Results and Discussion

The model achieves 85% accuracy, and the confusion matrix provides insights into its performance.

