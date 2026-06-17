# Tomato Leaf Disease Detection using Deep Learning

## Overview

This project uses a Convolutional Neural Network (CNN) to classify tomato leaf diseases from images. The dataset is preprocessed, converted into NumPy arrays, and used to train a deep learning model capable of identifying different tomato plant diseases.

## Features

* Image preprocessing and normalization
* Automatic label extraction from dataset folders
* Label encoding and one-hot encoding
* CNN-based image classification
* Early stopping to reduce overfitting
* Best model checkpoint saving
* Model evaluation on unseen test data

## Project Structure

```text
PLANT DISEASE PREDICTOR/
│
├── Data Conversion.ipynb      # Dataset preprocessing
├── Model Training.ipynb       # CNN model training
├── README.md
│
├── PlantVillage/              # Dataset (ignored by Git)
├── images.npy                 # Processed image data
├── labels.npy                 # Processed labels
└── best_model.h5              # Trained model
```

## Dataset

The project uses tomato leaf images belonging to multiple disease categories and healthy leaves.

Examples include:

* Healthy
* Early Blight
* Late Blight
* Leaf Mold
* Septoria Leaf Spot
* Tomato Mosaic Virus
* Tomato Yellow Leaf Curl Virus

## Data Preprocessing

The preprocessing notebook performs:

* Image loading using OpenCV
* Label extraction from folder names
* Image normalization
* Conversion to NumPy arrays
* Saving processed data as:

  * `images.npy`
  * `labels.npy`

## Model Architecture

The CNN architecture consists of:

* Conv2D (32 filters) + MaxPooling
* Conv2D (64 filters) + MaxPooling
* Conv2D (128 filters) + MaxPooling
* Flatten Layer
* Dropout Layer
* Dense Layer (128 neurons)
* Softmax Output Layer

## Training

The model is trained using:

* Optimizer: Adam
* Loss Function: Categorical Crossentropy
* Validation Split: 20%
* Early Stopping
* Model Checkpointing

## Evaluation

The best-performing model is automatically saved as:

```text
best_model.h5
```

The saved model is then evaluated on the test dataset to measure classification accuracy.

## Technologies Used

* Python
* NumPy
* OpenCV
* TensorFlow / Keras
* Scikit-Learn
* Jupyter Notebook

## Future Improvements

* Data augmentation
* Transfer learning using VGG16, ResNet50, or EfficientNet
* Hyperparameter tuning
* Streamlit web application deployment
* Real-time disease detection from uploaded images
