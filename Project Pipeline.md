# Skin Cancer Detection using Custom CNN

## Overview

This project aims to build a convolutional neural network (CNN) from scratch to accurately detect melanoma and other skin cancer types. Melanoma is a deadly form of skin cancer that accounts for 75% of skin cancer deaths. Early detection can save lives, and this solution aims to assist dermatologists by automating the detection process from skin images.

## Dataset

The dataset consists of 2357 images of nine different types of skin cancer, sourced from the International Skin Imaging Collaboration (ISIC). The dataset includes the following classes:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

You can download the dataset [here](https://drive.google.com/file/d/1xLfSQUGDl8ezNNbUkpuHOYvSpTyxVhCs/view).

## Project Pipeline

1. **Data Reading and Understanding**
   - Define paths for training and testing images.
   
2. **Dataset Creation**
   - Create training and validation datasets with a batch size of 32.
   - Resize images to 180x180 pixels.

3. **Dataset Visualization**
   - Visualize one instance of all nine classes present in the dataset.

4. **Model Building and Training**
   - Create a CNN model to detect the nine classes.
   - Rescale images to normalize pixel values between 0 and 1.
   - Choose an appropriate optimizer and loss function.
   - Train the model for 20 epochs.
   - Analyze if the model is overfitting or underfitting.
   
5. **Data Augmentation**
   - Apply data augmentation to resolve underfitting or overfitting.
   
6. **Model Building and Training on Augmented Data**
   - Train the model for another 20 epochs using augmented data.
   - Analyze improvements and identify any remaining issues.

7. **Class Distribution Analysis**
   - Examine the class distribution in the training dataset.
   - Identify classes with the least number of samples and those that dominate.

8. **Handling Class Imbalances**
   - Use the Augmentor library to rectify class imbalances.
   
9. **Final Model Building and Training**
   - Train the model for 30 epochs on the rectified class imbalance data.
   - Analyze the final model performance.

## Results and Findings

- **Initial Training:** Findings on overfitting/underfitting, model performance, etc.
- **After Augmentation:** Changes in model performance post data augmentation.
- **Class Imbalance Rectification:** Impact of handling class imbalances on model accuracy and reliability.

## Requirements

- Python 3.x
- TensorFlow
- NumPy
- Pandas
- Matplotlib
- Augmentor

## Installation

```bash
pip install tensorflow numpy pandas matplotlib Augmentor
