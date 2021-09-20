Traffic Sign Classification using CNN
===

## Table of contents
* [Introduction](#introduction)
* [Dataset](#dataset)
* [Results](#results)
* [Libraries](#libraries)

## Introduction
<b>Motivation</b> - To display my interest in image recognition, especially for practical applications of machine learning using realistic data. 

A focus of this project is to create a versatile model, using a CNN, with the ability to accurately classify traffic signs from small images in low lighting (at night, obscured in shadow) and low quality (blurred, low resolution).
Visual comparison of different models with various filter dimensions on training and validation sets to determine best model.

## Dataset
The dataset used for this project was obtained from a [popular Kaggle dataset for the German Traffic Sign Recognition Benchmark (GTSRB) challenge](https://www.kaggle.com/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign) 
The dataset consists of:
* 86,989 (~87,000) images in the training set
* 12,630 images in the test set
* ratio of training:test size is 87%
* Images are of size 32x32
* 43 different types of traffic signs

### Visualization of data
Notice that many of the images displaying the traffic signs are blurry, partially obscured, and dimly-lit. These features permeate through the many images in this dataset and is the main reason I chose this particular dataset - it is very realistic and thus the resulting model trained on this data is very applicable in real-world scenarios.

## Results
### Training and Validation Accuracy comparison between different models
![SVM Confusion Matrix](./Results/svm_confusion_matrix.JPG)
### Predictions with Best Model (images from test set)
The following shows the predicted label by the best model (chosen from the comparison above), as well as the true label below it. As you can see, the predictions are all correct for this set of images! This result matches the high accuracy that was observed for the training and validation sets (see above graph)
![SVM Quadratic Kappa Score](./Results/svm_qwk.JPG)



## Libraries
* tensorflow
* keras
* pandas
* numpy
* matplotlib
