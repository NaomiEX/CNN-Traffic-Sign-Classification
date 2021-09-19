Traffic Sign Classification using CNN
===

## Table of contents
* [Introduction](#introduction)
* [Dataset](#dataset)
* [Kaggle Placement](#kaggle-results)
* [Results](#results)
* [Libraries](#libraries)

## Introduction
<b>Motivation</b> - To display my interest in image recognition, especially for practical applications of machine learning using realistic data. 

A focus of this project was to create a versatile model, using a CNN, with the ability to accurately classify traffic signs from small images in low lighting (at night, obscured in shadow) and low quality (blurred, low resolution).
Visual comparison of different models with various filter dimensions on training and validation sets to determine best model.

## Dataset
The dataset used for this project was obtained from a [popular Kaggle dataset for the German Traffic Sign Recognition Benchmark (GTSRB) challenge](https://www.kaggle.com/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign) 

## Kaggle Results
With the model built from the Random Forest Classifier, I **won the Kaggle competition with 172 participating teams**.
[Full leaderboard](https://www.kaggle.com/c/mum-fit1043-s1-2021/leaderboard)
![Leaderboard](./Results/kaggle_results.JPG)

## Results
### SVM model (Confusion Matrix)
![SVM Confusion Matrix](./Results/svm_confusion_matrix.JPG)
### SVM model (Quadratic Kappa Score)
![SVM Quadratic Kappa Score](./Results/svm_qwk.JPG)
### RFC model (Confusion Matrix)
Note: Performed oversampling, thus total number of samples is greater in comparison to the SVM Confusion Matrix, the goal here is to correctly classify infrequent scores (1 and 6)

![RFC Confusion Matrix](./Results/rfc_confusion_matrix.JPG)
### RFC model (Quadratic Kappa Score)
Note: Much better QWK score in comparison to the SVM model!
![RFC Quadratic Kappa Score](./Results/rfc_qwk.JPG)


## Libraries
* scikit-learn (sklearn)
* imbalanced-learn (imblearn)
* pandas
* numpy
