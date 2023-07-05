# Diabetic Retinopathy Detection Model
This repository contains a machine-learning model for detecting diabetic retinopathy using image analysis techniques. The model utilizes the numpy and pandas libraries for data preprocessing and K-means clustering with PP centers for image segmentation. It also incorporates Support Vector Machine (SVM) with Radial Basis Function (RBF) and K-Nearest Neighbors (KNN) algorithms for classification.
## Dataset
The dataset used in this project was downloaded from Kaggle and consists of images related to diabetic retinopathy. The dataset is divided into two classes: "effected" and "non-effected." The "effected" images are marked with corresponding labels indicating the presence of diabetic retinopathy, while the "non-effected" images do not exhibit any signs of the condition.

## Preprocessing
Prior to training the model, the dataset undergoes a preprocessing phase. This step includes various techniques such as resizing the images, converting them to grayscale, and applying necessary transformations to enhance feature extraction capabilities.

## Image Visualization
To gain insights into the dataset, a random image is selected and visualized after the preprocessing steps. This allows users to observe the effect of the preprocessing techniques on the image and understand the characteristics of the diabetic retinopathy images.

## Wavelet Transform
The 2-D array containing the preprocessed images is subjected to Discrete Wavelet Transform (DWT). This technique decomposes the images into multiple frequency bands, enabling the extraction of important features for classification purposes.

## Image Visualization (Post Wavelet Transform)
After performing the DWT, another random image from the transformed dataset is selected and visualized. This provides an opportunity to observe the changes in the image representation after applying the wavelet transform.

## K-means Clustering
K-means clustering algorithm with PP centers (non-random initialization) and neighbors is applied to segment the final image obtained after the wavelet transform. This step helps in categorizing different regions of interest within the image.

## Model Training
The segmented images are used for model training. Two classification algorithms, namely SVM with RBF and KNN, are employed to train the model on the segmented image data. These algorithms learn patterns and features from the training data to make predictions on new, unseen images.

## Evaluation Results
The final accuracy achieved on predicting the presence of diabetic retinopathy over the remaining dataset is 96.62% using SVM with RBF. Additionally, a separate evaluation using the KNN algorithm yielded an accuracy of 94.38%. These results indicate the effectiveness of the trained model in detecting diabetic retinopathy.
