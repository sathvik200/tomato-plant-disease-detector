# Tomato Leaf Disease Detection - Data Preprocessing

## Overview

This project focuses on preprocessing tomato leaf images for a machine learning/deep learning-based disease detection system. The dataset contains images of healthy and diseased tomato leaves, which are processed and converted into NumPy arrays for model training.

## Features

* Loads tomato leaf images from dataset folders
* Automatically extracts disease labels from folder names
* Handles invalid or corrupted image files
* Converts images into NumPy arrays
* Normalizes pixel values for model training
* Saves processed images and labels for future use

## Technologies Used

* Python
* OpenCV
* NumPy
* Jupyter Notebook

## Dataset

The dataset consists of tomato leaf images belonging to different disease categories, such as:

* Tomato Healthy
* Tomato Early Blight
* Tomato Late Blight
* Tomato Leaf Mold
* Tomato Septoria Leaf Spot
* Tomato Mosaic Virus
* Tomato Yellow Leaf Curl Virus

*(Actual classes depend on the dataset used.)*

## Workflow

1. Load tomato leaf images from the dataset.
2. Extract disease labels from folder names.
3. Ignore unreadable or corrupted images.
4. Convert images and labels into NumPy arrays.
5. Normalize image pixel values.
6. Save processed data for future model training.

## Output

The preprocessing pipeline generates:

* `images.npy` – Processed image dataset
* `labels.npy` – Disease labels

## Future Improvements

* Image resizing and augmentation
* Label encoding
* Dataset splitting (train/validation/test)
* CNN model training
* Disease prediction system
* Streamlit web application deployment

## Author

Sathvik Karanth

Machine Learning Enthusiast | Test Engineer | Aspiring Data Scientist
