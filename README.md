# Lung Cancer Detection Using VGG16
This project uses the VGG16 architecture to classify lung images into different categories: Lung adenocarcinoma, Lung benign tissue, and Lung squamous cell carcinoma.

## Overview
The goal of this project is to build a Convolutional Neural Network (CNN) model using the pre-trained VGG16 architecture to detect different types of lung tissues in medical images. The model classifies images into three categories:<br>

Lung adenocarcinoma <br>
Lung benign tissue <br>
Lung squamous cell carcinoma<br>

## Dataset
The dataset contains images of lung tissues, categorized into the three mentioned types. It is structured in folders for each category:<br>
Lung adenocarcinoma<br>
Lung benign tissue<br>
Lung squamous cell carcinoma<br>

## Model Architecture
Base Model: VGG16 pre-trained on ImageNet, with frozen layers.<br>
Additional Layers:<br>
BatchNormalization<br>
MaxPooling2D<br>
Dense (1024, 512, 256 units)<br>
Dropout (0.3 rate)<br>
Output layer with softmax activation (4 units)<br>
The model is trained with sparse_categorical_crossentropy loss and adam optimizer.<br>

## Results
The model achieves an accuracy of **98%** on the test set. The performance is evaluated using the confusion matrix and classification report.
