Brain Tumor Classification Using Logistic Regression

This project aims to classify brain MRI images into four categories: glioma, meningioma, notumor, and pituitary. The goal is to build a simple yet effective baseline model using Logistic Regression to predict the type of brain tumor from MRI scans.

Project Overview
Dataset: The project uses MRI brain images categorized into four classes. Each class contains an equal number of images to ensure balanced training.
Classes:
Glioma – a type of tumor that occurs in the brain and spinal cord.
Meningioma – a tumor that arises from the meninges (protective layers around the brain and spinal cord).
Notumor – images with no brain tumor.
Pituitary – a tumor in the pituitary gland.
Methodology
Data Loading and Preprocessing:
Images are loaded using PIL, converted to grayscale, and resized to 64x64 pixels.
Images are flattened into 1D arrays suitable for Logistic Regression.
Data is split into training and testing sets (80% train, 20% test).
Feature Scaling:
StandardScaler is applied to normalize the data, which improves the model’s performance.
Model Training:
Logistic Regression is used as a baseline classifier for multi-class classification.
Multi-class is handled using the multinomial option with a suitable number of iterations (max_iter=1000).
Evaluation:
Model performance is evaluated using accuracy, confusion matrix, and classification report, which includes precision, recall, and F1-score for each class.
Results
The Logistic Regression model provides a baseline accuracy for predicting brain tumor types.
This baseline can be improved using more advanced models like CNNs in the future.
Usage
You can test the model with any new MRI image using the provided prediction function, which outputs the predicted tumor class.
