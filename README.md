# Melanoma Detection
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Table of Contents
* [Problem Statement](#problem-statement)
* [Project Pipeline](#project-pipeline)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

## Problem Statement
### Business Understanding
This dataset comprises 2357 images of malignant and benign oncological diseases sourced from the International Skin Imaging Collaboration (ISIC). The images are categorized based on their ISIC classifications. While most subsets contain an equal number of images, melanoma and nevus images exhibit slight dominance.
The data set contains the following diseases:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion
### Business Goal:
The objective is to develop a multi-class classification model using a custom convolutional neural network within the TensorFlow framework.
### Business Risk:
The primary risk lies in the misclassification of skin cancer types.

## Project Pipeline
- Data Reading/Data Understanding → Define the paths for training and testing image directories.
- Dataset Creation→ Generate training and validation datasets from the training directory using a batch size of 32 and Resize images to 180x180 pixels.
- Dataset visualisation → Implement code to visualize a single instance of each of the nine classes within the dataset.
- Model Building & training :
  - Design a CNN model capable of accurately classifying the nine disease classes.
  - Rescale images to normalize pixel values between 0 and 1 during model construction.
  - Select an appropriate optimizer and loss function for model training.
  - Train the model for approximately 20 epochs.
  - Analyze model performance and identify any evidence of overfitting or underfitting.
- Data Augmentation (Addressing Overfitting/Underfitting):
  - Implement a suitable data augmentation strategy to mitigate overfitting or underfitting observed in the initial model.
- Model Building & Training (Augmented Data):
  - Construct a CNN model for classifying the nine disease classes.
  - Rescale images to normalize pixel values between 0 and 1 during model construction.
  - Choose an appropriate optimizer and loss function for model training.
  - Train the model for approximately 20 epochs.
  - Evaluate model performance and assess whether the previous issue (overfitting/underfitting) has been resolved.
- Class Distribution Analysis: Examine the current class distribution in the training dataset
  - Identify the class with the least number of samples.
  - Determine the classes with the highest proportion of samples.
- Handling class imbalances: Address class imbalances in the training dataset using the Augmentor library.
- Model Building & training on the rectified class imbalance data :
  - Create a CNN model for classifying the nine disease classes.
  - Rescale images to normalize pixel values between 0 and 1 during model building.
  - Select an appropriate optimizer and loss function for model training.
  - Train the model for approximately 30 epochs.
  - Analyze model performance and determine whether the issues have been successfully resolved.

## Technologies Used
- TensorFlow version: 2.17.1
- Keras version: 3.5.0
- Matplotlib version: 3.10.0
- NumPy version: 1.26.4
- Pandas version: 2.2.2
- PIL version: 11.1.0
- Augmentor version: 0.2.12
## Acknowledgements
- Shivam Garg
## Contact
Created by [@Bhaskara-patnaik] - feel free to contact me!
