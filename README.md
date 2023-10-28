# Voice Gender Classification with Support Vector Machines (SVM)

This repository contains code for a machine learning project that classifies gender based on voice characteristics. It uses a Support Vector Machine (SVM) classifier to predict whether a voice belongs to a male or female speaker.

## Dataset

The dataset used in this project is a voice dataset with various acoustic features. It includes the following features:

- `meanfreq`
- `sd`
- `median`
- `Q25`
- `Q75`
- `IQR`
- `skew`
- `kurt`
- `sp.ent`
- `sfm`
- `mode`
- `centroid`
- `meanfun`
- `minfun`
- `maxfun`
- `meandom`
- `mindom`
- `maxdom`
- `dfrange`
- `modindx`
- `label` (target variable)

The target variable, 'label', indicates whether the voice belongs to a male (1) or female (0) speaker.

## Code Overview

- The code begins by loading the dataset using the Pandas library.
- It performs data preprocessing, including label encoding for the 'label' column.
- The data is split into training and testing sets.
- Standard scaling is applied to the features using `StandardScaler`.
- Several SVM models are trained with different kernel types and hyperparameters.
- Model performance is evaluated using accuracy, confusion matrix, and other classification metrics.
- The results are displayed using visualizations and printed metrics.

## Model Performance

The best SVM model achieved an accuracy of approximately 98.42% on the test data. Here are some key performance metrics:

- Accuracy: 98.42%
- Precision: 98.67%
- Recall (Sensitivity): 98.02%
- Specificity: 98.79%
- Classification Error: 1.58%
